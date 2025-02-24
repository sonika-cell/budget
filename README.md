<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Real Estate</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <nav class="navbar">
        <a href="#" class="nav-logo">
            <h2 class="logo-text">Real Estate</h2>
        </a>
        <ul class="nav-menu">
            <li class="nav-item"><a href="#" class="nav-link">Home</a></li>
            <li class="nav-item"><a href="#" class="nav-link">About</a></li>
            <li class="nav-item"><a href="#properties" class="nav-link">Properties</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Gallery</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Contact Us</a></li>
        </ul>
    </nav>
</header>

<main>
    <section class="hero-section">
        <div class="section-content">
            <div class="hero-details">
                <h2 class="title">Find Your Dream Home</h2>
                <section class="center">
                    <form action="search.html" method="post">
                        <h3>FIND YOUR PERFECT HOME</h3>
                        <div class="box">
                            <p>Enter Location <span>*</span></p>
                            <input type="text" name="location" required maxlength="50" placeholder="Enter city name" class="input">
                        </div>
                        <div class="flex">
                            <div class="box">
                                <p>Property Type <span>*</span></p>
                                <select name="type" class="input" required>
                                    <option value="flat">Flat</option>
                                    <option value="house">House</option>
                                    <option value="land">Land</option>
                                </select>
                            </div>
                            <div class="box">
                                <p>Select City <span>*</span></p>
                                <select name="place" class="input" required>
                                    <option value="Kathmandu">Kathmandu</option>
                                    <option value="Pokhara">Pokhara</option>
                                    <option value="Bhaktapur">Bhaktapur</option>
                                    <option value="Lalitpur">Lalitpur</option>
                                    <option value="Biratnagar">Biratnagar</option>
                                    <option value="Jhapa">Jhapa</option>
                                    <option value="Mustang">Mustang</option>
                                </select>
                            </div>
                        </div>
                        <input type="submit" value="Search Property" name="search" class="btn">
                    </form>
                </section>
            </div>
        </div>
    </section>

    <!-- Properties Section -->
    <section class="properties" id="properties">
        <div class="title-box">
            <h2 class="section-title">LATEST LISTING</h2>
        </div>

        <div class="property-grid">
            <div class="property-card" data-name="home1">
                <img src="home1.jpg" alt="Jhapa Home">
                <h3>RS 3,00,00,000</h3>
                <p>Jhapa</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card" data-name="home2">
                <img src="home2.jpg" alt="Bharatpur Home">
                <h3>RS 4,00,00,000</h3>
                <p>Bharatpur</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card" data-name="home3">
                <img src="home3.jpg" alt="Mustang Home">
                <h3>RS  2,00,00,000</h3>
                <p>Mustang</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card hidden" data-name="home4">
                <img src="home4.jpg" alt="Kathmandu Home">
                <h3>RS 1,50,00,000 </h3>
                <p>Kathmandu</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card hidden" data-name="home5">
                <img src="home5.jpg" alt="Pokhara Home">
                <h3>RS 80,00,000 </h3>
                <p>Pokhara</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card hidden" data-name="home6">
                <img src="home6.webp" alt="Lalitpur Home">
                <h3>RS 60000</h3>
                <p>Lalitpur</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card hidden" data-name="home7">
                <img src="home7.jpeg" alt="Mustang Home">
                <h3>RS  5,00,00,000</h3>
                <p>Mustang</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
        </div>

        <div class="view-all-container">
            <button id="viewAllBtn">View All</button>
        </div>
    </section>
</main>

<script>
document.getElementById("viewAllBtn").addEventListener("click", function() {
    const hiddenCards = document.querySelectorAll(".property-card.hidden");
    hiddenCards.forEach(card => card.classList.remove("hidden"));
    this.style.display = "none";
});

// JavaScript to handle enlarge and blur effects
document.querySelectorAll('.property-card').forEach(card => {
    card.addEventListener('click', function() {
        // Check if the clicked card is already enlarged
        if (this.classList.contains('enlarged')) {
            // If it's enlarged, reset all cards to normal
            document.querySelectorAll('.property-card').forEach(c => {
                c.classList.remove('enlarged');
                c.classList.remove('blurred');
            });
        } else {
            // Otherwise, enlarge the clicked card and blur others
            document.querySelectorAll('.property-card').forEach(c => {
                c.classList.add('blurred'); // Blur all cards
            });
            this.classList.remove('blurred'); // Remove blur from the clicked card
            this.classList.add('enlarged'); // Enlarge the clicked card
        }
    });
});
</script>

</body>
</html>
