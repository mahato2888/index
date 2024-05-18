<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mediretreats</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/assets/owl.carousel.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/assets/owl.theme.default.min.css">
    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/owl.carousel.min.js"></script>
    <script>
        $(document).ready(function() {
            $('.owl-carousel').owlCarousel({
                loop: true,
                margin: 10,
                nav: true,
                responsive: {
                    0: {
                        items: 1
                    },
                    600: {
                        items: 3
                    },
                    1000: {
                        items: 5
                    }
                }
            });
        });

        $(window).on('load', function() {
            $('.page-loader').addClass('loaded');
        });

        document.addEventListener('DOMContentLoaded', function() {
            const menuToggle = document.querySelector('.nav-toggle');
            const navLinks = document.querySelector('.nav-links');

            menuToggle.addEventListener('click', function() {
                navLinks.classList.toggle('nav-active');
            });
        });
    </script>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }

        .page-loader {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #fff;
            z-index: 9999;
            transition: opacity 0.5s ease;
        }

        .page-loader.loaded {
            display: none;
        }

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            padding: 1rem;
            background-color: #333;
            z-index: 1000;
        }

        .nav-links {
            display: flex;
            list-style: none;
            margin-left: auto;
        }

        .nav-links li {
            margin-right: 1rem;
        }

        .nav-links a {
            color: #fff;
            text-decoration: none;
        }

        .nav-toggle {
            display: none;
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .nav-toggle {
                display: block;
                cursor: pointer;
            }

            .nav-toggle span {
                display: block;
                width: 30px;
                height: 3px;
                background-color: #fff;
                margin: 5px auto;
            }

            .nav-active {
                display: flex;
                flex-direction: column;
            }
        }

        .hero, .treatment, .eligibility, .preparation, .post-treatment, .recovery-tips {
            padding: 2rem;
            background-color: #f5f5f5;
            margin-top: 3rem;
        }

        .hero-content, .treatment-content, .eligibility-content, .preparation-content, .post-treatment-content, .recovery-tips-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .btn {
            padding: 0.5rem 1rem;
            background-color: #333;
            color: #fff;
            border: none;
            cursor: pointer;
            margin-top: 1rem;
        }

        .btn:hover {
            background-color: #555;
        }

        /* Card Component Styles */
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f5f5f5;
        }

        .card {
            background-color: #ffffff;
            width: 400px;
            border-radius: 5px;
            padding: 20px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .card-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .card-header h2 {
            margin: 0;
            color: #333333;
        }

        .card-header button {
            background-color: #4c77d4;
            color: #ffffff;
            border: none;
            border-radius: 5px;
            padding: 10px 20px;
            cursor: pointer;
        }

        .card-body {
            margin-bottom: 20px;
        }

        .card-body h3 {
            margin: 0;
            color: #333333;
        }

        .card-body input[type="text"] {
            width: 100%;
            padding: 10px;
            border: 1px solid #cccccc;
            border-radius: 5px;
            margin-bottom: 20px;
        }

        .card-body textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #cccccc;
            border-radius: 5px;
            margin-bottom: 20px;
            resize: none;
        }

        .card-footer {
            display: flex;
            justify-content: flex-end;
        }

        .card-footer button {
            background-color: #4c77d4;
            color: #ffffff;
            border: none;
            border-radius: 5px;
            padding: 10px 20px;
            cursor: pointer;
        }

        .treatment {
            background-image: url("C:\Users\DELL\Desktop\webpage\fav5.jpg");
            /* Add any additional styling here */
        }

    </style>
</head>
<body>
    <!-- Page Loader -->
    <div class="page-loader">
        <div class="loader"></div>
    </div>

    <!-- Header Section -->
    <header>
        <nav class="navbar">
            <div class="logo">AAFIYA MEDIRETREATS</div>
            <ul class="nav-links">
                <li><a href="#">Home</a></li>
                <li><a href="#">About Us</a></li>
                <li><a href="#">Treatments</a></li>
                <li><a href="#">Destinations</a></li>
                <li><a href="#">Hospitals</a></li>
                <li><a href="#">FAQs</a></li>
                <li><a href="#">Blog</a></li>
            </ul>
            <div class="mobile-nav">
                <button class="nav-toggle">
                    <span></span>
                    <span></span>
                    <span></span>
                </button>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Healing Globally...</h1>
            <p>Second Medical Opinion | Book Consultation</p>
            <button class="btn">Call Us On: 985 896 2222</button>
            <button class="btn">Email Us On: info@mediretreats.com</button>
        </div>
    </section>

    <!-- Treatment Section -->
    <section class="treatment">
        <div class="treatment-content">
            <h2>Total Knee Replacement</h2>
            <p>Total knee replacement is a surgery to remove and replace the whole damaged knee joint with an artifical joint.</p>
            <button class="btn">Enquire Now</button>
        </div>
    </section>

    <!-- Eligibility Section -->
    <section class="eligibility">
        <div class="eligibility-content">
            <h2>Eligibility For Treatment</h2>
            <p></p>
            <ul>
                <li>The BMI (body mass index) is 40 or more</li>
                <li>Your BMI is 30 or more with severe weight-related health conditions like type-2 diabetes and high blood pressure</li>
                <li>You are willing to make permanent changes in the lifestyle</li>
            </ul>
        </div>
    </section>

    <!-- Preparation Section -->
    <section class="preparation">
        <div class="preparation-content">
            <h2>Preparation Before Treatment</h2>
            <p></p>
            <ul>
                <li>The BMI (body mass index) is 40 or more</li>
                <li>Your BMI is 30 or more with severe weight-related health conditions like type-2 diabetes and high blood pressure</li>
                <li>You are willing to make permanent changes in the lifestyle</li>
            </ul>
        </div>
    </section>

    <!-- Post-Treatment Section -->
    <section class="post-treatment">
        <div class="post-treatment-content">
            <h2>Post-Treatment Care</h2>
            <p></p>
            <ul>
                <li>The BMI (body mass index) is 40 or more</li>
                <li>Your BMI is 30 or more with severe weight-related health conditions like type-2 diabetes and high blood pressure</li>
                <li>You are willing to make permanent changes in the lifestyle</li>
            </ul>
        </div>
    </section>

    <!-- Recovery Tips Section -->
    <section class="recovery-tips">
        <div class="recovery-tips-content">
            <h2>Recovery Tips</h2>
            <p></p>
            <ul>
                <li>The BMI (body mass index) is 40 or more</li>
                <li>Your BMI is 30 or more with severe weight-related health conditions like type-2 diabetes and high blood pressure</li>
                <li>You are willing to make permanent changes in the lifestyle</li>
            </ul>
        </div>
    </section>

     <!-- Eligibility Section -->
     <section class="eligibility">
        <div class="eligibility-content">
            <h2>Eligibility For Treatment</h2>
            <p></p>
            <ul>
                <li>The BMI (body mass index) is 40 or more</li>
                <li>Your BMI is 30 or more with severe weight-related health conditions like type-2 diabetes and high blood pressure
                <li>You are willing to make permanent changes in the lifest</li>

    <!-- Gallery Section -->
    <section id="gallery">
        <div class="owl-carousel">
            <div class="item"><img src="C:\Users\DELL\Desktop\webpage\back.jpg" alt="Image 1"></div>
            <div class="item"><img src="C:\Users\DELL\Desktop\webpage\22.jpeg" alt="Image 2"></div>
            <div class="item"><img src="C:\Users\DELL\Desktop\webpage\23.jpeg" alt="Image 3"></div>
            <div class="item"><img src="C:\Users\DELL\Desktop\webpage\24.jpeg" alt="Image 4"></div>
            <div class="item"><img src="C:\Users\DELL\Desktop\webpage\23.jpeg" alt="Image 5"></div>
        </div>
    </section>

    <!-- Card Section -->
    <section class="container">
        <div class="card">
            <div class="card-header">
                <h2>Card Title</h2>
                <button>Button</button>
            </div>
            <div class="card-body">
                <h3>NAME</h3>
                <input type="text" placeholder="Text Input">
                <h4>ENAIL</h4>
                <input type="text" placeholder="Text Input">
                <h4>PHONENUMBER</h4>
                <input type="text" placeholder="Text Input">
                <h4>DESCRIBE YOUR RECQUIREMENT</h4>
                <textarea rows="4" placeholder="Textarea"></textarea>
            </div>
            <div class="card-footer">
                <button>Submit</button>
            </div>
        </div>
    </section>
</body>
</html>
