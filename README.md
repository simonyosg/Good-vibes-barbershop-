
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Good Vibes Barber Shop | Zero Stress. Perfect Fades.</title>
    <meta name="description" content="Good Vibes Barber Shop - Zero Stress. Perfect Fades. More Than a Haircut, It’s a Vibe. Located in Singapore.">
   
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons CDN (for barber tools and social media icons) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
   
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        charcoal: '#1A1A1A',
                        gold: '#C5A358',
                        bronze: '#8B6A45',
                        'dark-gray': '#2C2C2C',
                        'off-white': '#F0F0F0',
                    },
                    fontFamily: {
                        sans: ['Roboto', 'sans-serif'],
                        display: ['Oswald', 'sans-serif'],
                    }
                }
            }
        }
    </script>
   
    <style>
        /* Custom global styles for the industrial dark aesthetic */
        body {
            background-color: #1A1A1A; /* Charcoal background */
            color: #F0F0F0; /* Off-white text */
            font-family: 'Roboto', sans-serif;
            overflow-x: hidden;
        }

        /* Industrial Text Shadow for highlights */
        .text-glow-gold {
            text-shadow: 0 0 8px rgba(197, 163, 88, 0.7), 0 0 2px rgba(197, 163, 88, 0.4);
        }
       
        /* Custom Button Style */
        .btn-gold {
            background-color: #C5A358;
            color: #1A1A1A;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.4);
        }
        .btn-gold:hover {
            background-color: #8B6A45;
            color: #F0F0F0;
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.8);
        }

        /* Hero Section Styling (using a stylized background image/gradient) */
        .hero-bg {
            /* Placeholder image of a moody, industrial barber working */
            background: linear-gradient(rgba(26, 26, 26, 0.85), rgba(26, 26, 26, 0.85)), url('https://images.unsplash.com/photo-1550734005-5f6068d83a1b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1800&q=80');
            background-size: cover;
            background-position: center 30%;
            background-attachment: fixed; /* Parallax effect */
        }

        /* Separator line style */
        .divider-gold {
            width: 80px;
            height: 3px;
            background-color: #C5A358;
            margin: 1rem auto;
            border-radius: 9999px;
        }

        /* Service Card Hover Effect */
        .service-card {
            transition: all 0.3s ease;
            border-left: 5px solid transparent;
            position: relative;
            overflow: hidden;
        }
        .service-card:hover {
            transform: scale(1.02);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.7);
            border-left: 5px solid #C5A358;
        }
    </style>
</head>

<body class="bg-charcoal min-h-screen">

    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-charcoal/95 backdrop-blur-sm shadow-2xl border-b border-dark-gray">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <a href="#" class="text-3xl font-display font-black tracking-widest text-gold uppercase text-glow-gold">
                Good Vibes
            </a>
           
            <nav class="hidden md:flex space-x-10">
                <a href="#about" class="text-off-white hover:text-gold transition duration-200 uppercase text-sm font-medium tracking-wider">About</a>
                <a href="#services" class="text-off-white hover:text-gold transition duration-200 uppercase text-sm font-medium tracking-wider">Services</a>
                <a href="#location" class="text-off-white hover:text-gold transition duration-200 uppercase text-sm font-medium tracking-wider">Location</a>
            </nav>

            <a href="#booking" class="btn-gold px-4 py-2 text-sm font-semibold rounded-lg hidden md:block">
                Book Appointment
            </a>
           
            <!-- Mobile Menu Button (Hamburger) -->
            <button id="mobile-menu-button" class="md:hidden text-off-white focus:outline-none">
                <i class="fas fa-bars text-xl"></i>
            </button>
        </div>

        <!-- Mobile Menu (Hidden by default) -->
        <div id="mobile-menu" class="hidden md:hidden bg-charcoal/95 border-t border-dark-gray">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 flex flex-col items-center">
                <a href="#about" class="block px-3 py-2 rounded-md text-base font-medium text-off-white hover:bg-dark-gray w-full text-center">About</a>
                <a href="#services" class="block px-3 py-2 rounded-md text-base font-medium text-off-white hover:bg-dark-gray w-full text-center">Services</a>
                <a href="#location" class="block px-3 py-2 rounded-md text-base font-medium text-off-white hover:bg-dark-gray w-full text-center">Location</a>
                <a href="#booking" class="btn-gold w-3/4 text-center mt-3 py-2 rounded-lg font-semibold">Book Now</a>
            </div>
        </div>
    </header>

    <!-- 1. Hero Section -->
    <section class="hero-bg h-[90vh] flex items-center justify-center text-center px-4" id="hero">
        <div class="max-w-4xl p-6 bg-charcoal/30 rounded-xl backdrop-blur-sm">
            <h1 class="font-display text-7xl sm:text-8xl md:text-9xl font-black uppercase leading-none text-off-white text-glow-gold">
                Perfect Fades.
            </h1>
            <p class="mt-4 text-xl sm:text-3xl font-light text-gold text-glow-gold tracking-widest">
                Zero Stress. More Than a Haircut, It’s a Vibe.
            </p>
            <a href="#booking" class="btn-gold mt-10 px-12 py-4 text-xl font-bold rounded-full shadow-2xl uppercase tracking-wider transition-transform">
                Book Your Vibe Now <i class="fas fa-arrow-right ml-2"></i>
            </a>
        </div>
    </section>

    <!-- Floating Quick Book Button (Mobile specific) -->
    <a href="#booking" class="fixed bottom-4 right-4 z-40 md:hidden btn-gold px-5 py-3 rounded-full shadow-lg font-bold uppercase text-sm">
        <i class="fas fa-calendar-check mr-2"></i> Book
    </a>


    <!-- 2. About Section -->
    <section id="about" class="py-20 md:py-32 bg-dark-gray border-b border-t border-bronze/10">
        <div class="max-w-5xl mx-auto px-6 grid grid-cols-1 lg:grid-cols-3 gap-10 items-center">
           
            <div class="lg:col-span-1 text-center lg:text-left">
                 <h2 class="text-5xl font-display font-bold uppercase text-gold mb-2 leading-tight">THE GOOD VIBES</h2>
                 <p class="text-xl text-bronze font-light">Zero compromise on quality.</p>
                 <div class="divider-gold mx-auto lg:ml-0"></div>
            </div>

            <div class="lg:col-span-2">
                <p class="mt-6 text-xl text-off-white leading-relaxed tracking-wide">
                    Located conveniently at BLK 360 Yung An Road, we specialize in precision fades and providing a genuinely relaxing atmosphere. We blend classic techniques with modern style, ensuring every client leaves looking sharp and feeling refreshed.
                </p>
                <p class="mt-4 text-xl text-off-white leading-relaxed font-semibold">
                    Whether it's a quick student cut or the full <span class="text-gold">'Good Vibes Experience,'</span> we guarantee zero stress and perfect results every time. Come catch a vibe!
                </p>
            </div>
        </div>
    </section>

    <!-- 3. Services & Booking Menu -->
    <section id="services" class="py-20 md:py-32 bg-charcoal">
        <div class="max-w-7xl mx-auto px-6">
            <h2 class="text-5xl font-display font-black uppercase text-center text-off-white mb-2">Our Service Menu</h2>
            <p class="text-xl text-center text-gold mb-10">Choose Your Vibe. Zero Stress, Maximum Results.</p>
            <div class="divider-gold"></div>

            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 mt-16">
               
                <!-- Service Card HTML Structure (repeated via JS for cleaner code) -->
                <script>
                    const services = [
                        { icon: 'fas fa-cut', title: 'Standard Haircut', duration: '40 mins', price: '35', description: 'A precision cut tailored to your style. Includes wash and finished styling.' },
                        { icon: 'fas fa-graduation-cap', title: 'Student Haircut', duration: '30 mins', price: '25', description: 'Quick and clean fade or trim for students (valid ID required).' },
                        { icon: 'fas fa-user-ninja', title: 'Clean Shave', duration: '30 mins', price: '30', description: 'Traditional hot towel shave for the closest, smoothest finish.' },
                        { icon: 'fas fa-beard', title: 'Beard Trim & Line Up', duration: '30 mins', price: '25', description: 'Shaping, lining, and fading the beard to perfection using professional trimmers.' },
                        { icon: 'fas fa-star-of-life', title: 'Vibes Experience', duration: '60 mins', price: '55', description: 'The perfect combo: Haircut plus a professional Beard Trim or Clean Shave.' },
                        { icon: 'fas fa-crown', title: 'Good Vibes Experience', duration: '75-90 mins', price: '70', description: 'The ultimate treatment: Haircut, Head Massage, Beard/Shave, and a refreshing Facial.' }
                    ];

                    const waxing = [
                        { name: 'Ear Wax', price: '8' },
                        { name: 'Nose Wax', price: '8' }
                    ];

                    function createServiceCard(service) {
                        return `
                        <div class="service-card bg-dark-gray p-6 rounded-xl shadow-xl flex flex-col justify-between">
                            <div>
                                <div class="flex items-center space-x-4 mb-3">
                                    <i class="${service.icon} text-3xl text-gold"></i>
                                    <h3 class="text-2xl font-display font-semibold uppercase text-off-white">${service.title}</h3>
                                </div>
                                <p class="text-bronze text-sm mb-4">${service.duration}</p>
                                <p class="text-off-white text-base">${service.description}</p>
                            </div>
                            <div class="flex justify-between items-end mt-4 pt-4 border-t border-charcoal">
                                <span class="text-3xl font-bold text-gold">$${service.price}</span>
                                <a href="#booking" class="text-sm px-4 py-2 border border-gold text-gold hover:bg-gold hover:text-charcoal transition rounded-lg font-semibold">Book Now</a>
                            </div>
                        </div>
                        `;
                    }
                   
                    services.forEach(service => document.write(createServiceCard(service)));
                </script>

                <!-- 3.3 Waxing Add-ons -->
                <div class="service-card bg-dark-gray p-6 rounded-xl shadow-xl lg:col-span-3">
                    <h3 class="text-3xl font-display font-semibold uppercase text-gold mb-4 border-b border-charcoal pb-2">
                         <i class="fas fa-hand-holding-medical text-2xl mr-3"></i> Quick Add-ons
                    </h3>
                    <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mt-4">
                        <script>
                            waxing.forEach(item => {
                                document.write(`
                                    <div class="flex justify-between p-4 bg-charcoal rounded-lg shadow-inner border border-bronze/30">
                                        <span class="text-off-white font-medium">${item.name}</span>
                                        <span class="text-xl font-bold text-gold">$${item.price}</span>
                                    </div>
                                `);
                            });
                        </script>
                    </div>
                </div>

            </div>
        </div>
    </section>
   
    <!-- 4. Booking System Integration (Simulated) -->
    <section id="booking" class="py-20 bg-dark-gray border-t border-b border-bronze/10">
        <div class="max-w-5xl mx-auto px-6 text-center">
            <h2 class="text-5xl font-display font-bold uppercase text-gold mb-4">Book Your Appointment</h2>
            <div class="divider-gold"></div>
           
            <p class="text-xl text-off-white mb-8">Our integrated mobile-friendly booking system ensures zero hassle. Select your service, date, and preferred barber below.</p>

            <!-- Simulated Embedded Calendar Widget -->
            <div class="bg-charcoal p-4 rounded-xl shadow-2xl h-[500px] flex items-center justify-center relative overflow-hidden border border-gold/50">
                <p class="text-2xl text-bronze italic">
                    [Integrated Mobile-Friendly Calendar & Booking System]
                </p>
                <!-- Clickable overlay to simulate linking to the external booking system -->
                <div class="absolute inset-0 flex items-center justify-center opacity-0 hover:opacity-100 transition duration-500 bg-charcoal/80">
                    <a href="https://app.goodvibesbarbersg.com/booking" target="_blank" class="btn-gold px-8 py-4 text-xl font-bold rounded-lg shadow-xl uppercase">
                        Launch Booking Portal
                    </a>
                </div>
            </div>

            <p class="mt-6 text-sm text-bronze italic">
                Automated SMS and Email reminders will be sent 24 hours prior to your confirmation.
            </p>
           
            <!-- Staging Link Requirement -->
            <div class="mt-12 p-6 bg-charcoal rounded-lg border border-bronze shadow-lg">
                <h4 class="text-2xl font-semibold text-gold mb-2">Mobile Staging Link for Testing:</h4>
                <p class="text-lg text-off-white">
                    <i class="fas fa-mobile-alt mr-3"></i> Before launch, please test responsiveness here:
                    <a href="https://staging.goodvibesbarbersg.com/mobile-test" target="_blank" class="text-gold hover:text-off-white underline font-medium transition">www.GoodVibesBarberSG.com/staging</a>
                </p>
            </div>
        </div>
    </section>

    <!-- 5. Location & Contact Footer -->
    <footer id="location" class="py-20 bg-charcoal">
        <div class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-2 gap-12 border-t border-dark-gray pt-10">
           
            <!-- Google Map -->
            <div>
                <h4 class="text-3xl font-display font-bold text-gold uppercase mb-4">Find The Shop</h4>
                <p class="text-lg text-off-white mb-4">BLK 360 YUNG AN ROAD #04-101, SINGAPORE 610360</p>
                <div class="h-80 bg-dark-gray rounded-xl shadow-2xl border border-bronze/50 overflow-hidden">
                    <!-- Embedded Google Map for Singapore address -->
                    <iframe
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3988.5866164214535!2d103.71444157467664!3d1.3934305986877002!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31da0c54157ef22b%3A0x86604a11c1d8848d!2s360%20Yung%20An%20Rd%2C%20Singapore%20610360!5e0!3m2!1sen!2ssg!4v1704288000000!5m2!1sen!2ssg"
                        width="100%"
                        height="100%"
                        style="border:0;"
                        allowfullscreen=""
                        loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
            </div>
           
            <!-- Contact Info & Hours -->
            <div class="space-y-6">
                <h4 class="text-3xl font-display font-bold text-gold uppercase mb-4">Get in Touch</h4>
               
                <div class="space-y-3">
                    <p class="flex items-center text-xl text-off-white">
                        <i class="fas fa-clock text-2xl text-bronze w-8"></i>
                        <span class="font-bold mr-2">Hours:</span> Mon – Sat, 11:00 AM – 8:00 PM
                    </p>
                    <p class="flex items-center text-xl text-off-white">
                        <i class="fas fa-calendar-times text-2xl text-red-500 w-8"></i>
                        <span class="font-bold mr-2">Closed:</span> Sundays
                    </p>
                    <p class="flex items-center text-xl text-off-white">
                        <i class="fas fa-phone-alt text-2xl text-bronze w-8"></i>
                        <a href="tel:+6587273741" class="hover:text-gold transition">+65 8727 3741</a>
                    </p>
                    <p class="flex items-center text-xl text-off-white">
                        <i class="fas fa-envelope text-2xl text-bronze w-8"></i>
                        <a href="mailto:pasposip@gmail.com" class="hover:text-gold transition">pasposip@gmail.com</a>
                    </p>
                </div>
               
                <!-- Social Media -->
                <div class="pt-6">
                    <h5 class="text-xl font-display font-semibold text-off-white mb-3">Follow The Vibe:</h5>
                    <div class="flex space-x-6">
                        <a href="https://www.instagram.com/GoodVibesBarberShop" target="_blank" class="text-off-white hover:text-gold transition duration-200 text-3xl transform hover:scale-110">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" target="_blank" class="text-off-white hover:text-gold transition duration-200 text-3xl transform hover:scale-110">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="https://www.GoodVibesBarberSG.com" target="_blank" class="text-off-white hover:text-gold transition duration-200 text-3xl transform hover:scale-110">
                            <i class="fas fa-globe"></i>
                        </a>
                    </div>
                </div>
            </div>
           
        </div>
       
        <!-- Copyright Bar -->
        <div class="max-w-7xl mx-auto px-6 mt-16 pt-8 border-t border-dark-gray text-center">
            <p class="text-sm text-bronze">
                &copy; 2024 Good Vibes Barber Shop (www.GoodVibesBarberSG.com). All Rights Reserved. Designed with Good Vibes.
            </p>
        </div>
    </footer>

    <!-- JavaScript for Mobile Menu Functionality -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const menuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            const navLinks = mobileMenu.querySelectorAll('a');

            menuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });
           
            // Close mobile menu when a link is clicked (smooth scrolling)
            navLinks.forEach(link => {
                link.addEventListener('click', () => {
                    // Slight delay to allow smooth scroll to start before hiding
                    setTimeout(() => {
                        mobileMenu.classList.add('hidden');
                    }, 300);
                });
            });
        });
    </script>
</body>
</html>
