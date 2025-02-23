<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Real Estate</title>
    <link rel="stylesheet" href="style.css">
    <style>
        /* Add the background color to the box surrounding the title */
        .properties .title-box {
            background-color: #344e41;
            padding: 20px;
            display: inline-block;
            border-radius: 8px;
        }

        /* Change the color of the title text to white */
        .section-title {
            color: white;
        }

        /* View All Feature */
        .hidden {
            display: none;
        }

        .view-property-btn {
            display: inline-block;
            margin-top: 10px;
            padding: 8px 15px;
            background: var(--primary-color);
            color: var(--white-color);
            text-decoration: none;
            border-radius: var(--border-radius-s);
            transition: 0.3s ease;
        }

        .view-property-btn:hover {
            background: #2b3c32;
        }

        .view-all-container {
            text-align: center;
            margin-top: 20px;
        }

        #viewAllBtn {
            padding: 10px 20px;
            font-size: var(--font-size-m);
            background: var(--primary-color);
            color: var(--white-color);
            border: none;
            border-radius: var(--border-radius-m);
            cursor: pointer;
            transition: 0.3s ease;
        }

        #viewAllBtn:hover {
            background: #2b3c32;
        }
    </style>
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
                                    <option value="Jhapa"> Jhapa</option>
                                    <option value="Lagan"> Lagan</option>
                                </select>
                            </div>
                            <div class="box">
                                <p>Minimum Budget <span>*</span></p>
                                <select name="budget" class="input" required>
                                    <option value="200000-500000">RS 2 Lakh - 5 Lakh</option>
                                    <option value="1000000-2000000">RS 10 Lakh - 20 Lakh</option>
                                    <option value="10000000-50000000">RS 1 Crore - 5 Crore</option>
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
        <p class="section-description">
            Discover stunning homes that match your dreams and budget. From cozy apartments to luxurious villas, 
            find the perfect space to call home.
        </p>

        <div class="property-grid">
            <!-- First three listings (visible by default) -->
            <div class="property-card">
                <img src="home2.webp" alt="Modern House">
                <h3>RS 2,50,00,000</h3>
                <p>Kathmandu</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card">
                <img src="home3.jpg" alt="Luxury Villa">
                <h3>RS 12,00,00,000</h3>
                <p>Pokhara</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card">
                <img src="home1.jpg" alt="City Apartment">
                <h3>RS 3,50,00,000</h3>
                <p>Bhaktapur</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>

            <!-- Hidden properties (shown after clicking "View All") -->
            <div class="property-card hidden">
                <img src="home4.jpg" alt="Suburban Home">
                <h3>RS 4,50,00,000</h3>
                <p>Lalitpur</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card hidden">
                <img src="home5.webp" alt="Cozy Cottage">
                <h3>RS 1,80,00,000</h3>
                <p>Biratnagar</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
            <div class="property-card hidden">
                <img src="home6.jpg" alt="Elegant Mansion">
                <h3>RS 30,00,00,000</h3>
                <p>Kathmandu</p>
                <a href="#" class="view-property-btn">View Property</a>
            </div>
        </div>

        <!-- View All button -->
        <div class="view-all-container">
            <button id="viewAllBtn">View All</button>
        </div>
    </section>
</main>

<script>
document.getElementById("viewAllBtn").addEventListener("click", function() {
    const hiddenCards = document.querySelectorAll(".property-card.hidden");
    hiddenCards.forEach(card => card.classList.remove("hidden"));
    this.style.display = "none"; // Hide the button after clicking
});
</script>

</body>
</html>
