# Vacation-Info
Just some relevant data I thought would help
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Family Vacation 2025 - Hideout in the Wood</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;900&family=Luckiest+Guy&family=Pacifico&display=swap" rel="stylesheet">
    <style>
        /* Apply Inter font globally */
        body {
            font-family: 'Inter', sans-serif;
            /* Subtle background pattern */
            background-color: #f9fafb; /* fallback */
            background-image: linear-gradient(45deg, #e5e7eb 25%, transparent 25%), linear-gradient(-45deg, #e5e7eb 25%, transparent 25%), linear-gradient(45deg, transparent 75%, #e5e7eb 75%), linear-gradient(-45deg, transparent 75%, #e5e7eb 75%);
            background-size: 20px 20px;
        }
        /* Smooth scrolling */
        html {
            scroll-behavior: smooth;
        }
        /* Simple fade-in animation */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Simple pulse animation for icon */
        @keyframes pulse {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: 0.8; transform: scale(1.1); }
        }
        .fade-in {
            animation: fadeIn 0.8s ease-out forwards;
        }
        /* Custom gradient for hero */
        .hero-gradient {
            background: linear-gradient(to bottom, rgba(30, 64, 175, 0.85), rgba(17, 24, 39, 0.95)), url('https://placehold.co/1920x1080/334155/e2e8f0?text=Sunrise+over+Lake+Huron+(Placeholder)') center center / cover no-repeat;
            position: relative; /* Needed for absolute positioning of children */
        }
         /* Style for cards */
        .info-card {
            @apply bg-white rounded-lg shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105 p-6 flex flex-col;
        }
         /* Style for golf cards specifically */
         .golf-card {
            @apply bg-white rounded-lg shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105 flex flex-col;
         }
         .golf-card img {
            @apply w-full h-48 object-cover;
         }
         .golf-card .content {
            @apply p-4 flex flex-col flex-grow;
         }
        .golf-card h3, .info-card h3 { /* Shared heading style */
            @apply text-xl font-bold text-blue-800 mb-2;
        }
        .golf-card p, .info-card p { /* Shared paragraph style */
            @apply text-gray-600 text-sm mb-3 flex-grow;
        }
        .golf-card .details, .info-card .details { /* Shared details style */
             @apply text-xs text-gray-500 mb-3 space-y-1; /* Added space-y-1 */
        }
         /* Added style for detail items within golf card */
         .golf-card .detail-item {
             @apply flex items-center;
         }
         .golf-card .detail-item i {
             @apply w-4 text-center mr-2 text-blue-500; /* Icon styling */
         }
         .info-card .icon { /* Icon style for non-golf cards */
            @apply text-4xl text-blue-600 mb-4 text-center;
         }
        .golf-card a, .info-card a { /* Shared link style */
            @apply text-blue-600 hover:text-blue-800 text-sm font-semibold;
        }
        .golf-card .links {
            @apply mt-auto pt-3 border-t border-gray-200 space-y-1; /* Push links to bottom */
        }
        .info-card a {
             @apply mt-auto; /* Push links to bottom */
        }

        /* Section heading style */
        .section-heading {
            @apply text-6xl font-black text-center mb-2 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent;
        }
         .section-heading i {
             @apply text-blue-600; /* Set a solid color for the icon */
         }

        .section-heading-divider {
             @apply w-24 h-1 bg-yellow-400 mx-auto mb-10; /* Added divider */
        }

         /* Warning Box Style */
        .warning-box {
            @apply absolute top-0 right-2 bg-red-500 text-white px-4 py-3 rounded-b-lg shadow-xl text-base z-10;
        }
        .warning-box strong {
            @apply font-bold block;
        }
         .warning-box span {
            @apply text-sm block mt-1 opacity-90;
         }
         .warning-box i {
             @apply mx-1 text-yellow-300;
         }

         /* Countdown Banner Style - UPDATED */
        #countdown-banner {
            font-family: 'Luckiest Guy', cursive;
            /* Added gradient, padding, larger text size */
            @apply bg-gradient-to-r from-teal-200 via-cyan-200 to-sky-200 text-teal-800 p-6 text-center shadow-lg tracking-wider;
        }
         /* Style for the "3rd Annual" title within the banner */
        .annual-title-banner {
            font-family: 'Pacifico', cursive;
             /* Larger size, gradient text, margin bottom */
            @apply text-6xl font-bold bg-gradient-to-r from-orange-500 to-pink-500 bg-clip-text text-transparent mb-4 block;
        }
         /* Countdown text styling */
        .countdown-text {
            @apply text-xl text-teal-700 mb-3; /* Adjusted size */
        }
        #countdown-banner span {
             /* Larger numbers, more padding */
             @apply inline-block mx-1 px-4 py-2 bg-white rounded-lg shadow-md text-teal-900 text-3xl;
        }
        #countdown-banner .icon {
             @apply text-4xl text-teal-600 mx-2 inline-block align-middle; /* Slightly larger icon */
             animation: pulse 2s infinite ease-in-out;
        }

    </style>
</head>
<body class="bg-gray-50 text-gray-700">

    <header class="bg-white shadow-md sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-3 flex justify-between items-center">
            <div class="text-lg font-bold text-blue-800"><i class="fas fa-tree mr-2 text-green-600"></i>Family Vacation 2025 - Hideout in the Wood</div>
            <div class="space-x-4 text-sm hidden md:block">
                <a href="#about" class="text-gray-600 hover:text-blue-700">About</a>
                <a href="#explore" class="text-gray-600 hover:text-blue-700">Explore</a>
                <a href="#taste" class="text-gray-600 hover:text-blue-700">Taste</a>
                <a href="#attractions" class="text-gray-600 hover:text-blue-700">Attractions</a>
                <a href="#golf" class="text-gray-600 hover:text-blue-700">Golf</a>
                <a href="#plan" class="text-gray-600 hover:text-blue-700">Plan</a>
            </div>
            <div class="md:hidden">
                <button class="text-gray-600 focus:outline-none">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
        </nav>
    </header>

    <section id="countdown-banner" class="fade-in" style="animation-delay: 0.1s;">
        <h2 class="annual-title-banner">3rd Annual</h2>
        <div class="countdown-text">
            <i class="fas fa-calendar-alt icon"></i> Trip Countdown:
            <span id="days">--</span> D :
            <span id="hours">--</span> H :
            <span id="minutes">--</span> M :
            <span id="seconds">--</span> S
            until Aug 17th!
            <i class="fas fa-campground icon"></i>
        </div>
    </section>

    <section class="hero-gradient text-white py-24 px-6 text-center fade-in min-h-[60vh] flex flex-col justify-center items-center">
        <div class="warning-box">
             <i class="fas fa-dollar-sign"></i> <strong>Payment is Due by July 18th*</strong>
            <span>Pay Justin Please</span>
             <i class="fas fa-money-bill-wave"></i> </div>

        <h1 class="text-5xl font-black mb-4">Your Lakeside Woods Escape</h1>
        <p class="text-xl mb-8 max-w-3xl mx-auto">Discover the beauty of the Sunrise Coast. Relax <i class="fas fa-couch text-yellow-300"></i>, explore <i class="fas fa-binoculars text-yellow-300"></i>, and make memories <i class="fas fa-camera-retro text-yellow-300"></i> at The Woods of Au Sable near Oscoda, Michigan.</p>
        <a href="#explore" class="bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-3 px-6 rounded-lg transition duration-300">Start Exploring</a>
    </section>

    <main class="container mx-auto px-6 py-12">

        <section id="about" class="mb-16 fade-in" style="animation-delay: 0.2s;">
            <h2 class="section-heading"><i class="fas fa-home mr-2"></i>About The Property</h2>
            <div class="section-heading-divider"></div>
            <div class="bg-white p-8 rounded-lg shadow-lg text-center max-w-4xl mx-auto">
                 <h3 class="text-2xl font-bold text-blue-800 mb-3">Hideout in the Wood</h3>
                <p class="mb-4 text-gray-600"><i class="fas fa-map-marker-alt mr-2 text-blue-600"></i>2557 North Old US Hwy 23, Au Sable Twp, MI 48750</p>
                <p class="text-sm text-gray-500">Nestled near the shores of Lake Huron and the banks of the Au Sable River, this getaway offers a perfect base for exploring the natural beauty and attractions of the Oscoda and Tawas areas. Ideal for families and adventurers alike. Get ready to relax, grill <i class="fas fa-fire-burner text-orange-500"></i>, and have fun!</p>
                <img src="https://placehold.co/600x400/a5f3fc/0c4a6e?text=Cozy+Cabin+Vibes+(Placeholder)" alt="Placeholder image suggesting a cozy rental property" class="mt-6 rounded-lg shadow-md mx-auto" onerror="this.src='https://placehold.co/600x400/cccccc/999999?text=Image+Not+Available'; this.alt='Image Not Available'">
            </div>
        </section>

        <section id="explore" class="mb-16 fade-in" style="animation-delay: 0.4s;">
             <h2 class="section-heading"><i class="fas fa-hiking mr-2"></i>Explore & Experience</h2>
             <div class="section-heading-divider"></div>
            <p class="text-center text-gray-600 mb-10 max-w-3xl mx-auto">From serene river paddles to thrilling hikes and lakeside relaxation, adventure awaits just minutes away.</p>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="info-card">
                    <i class="fas fa-umbrella-beach icon"></i>
                    <h3>Lake Huron Beaches</h3>
                    <p>Enjoy swimming, sunbathing, and sandcastles on the beautiful "Sunrise Coast".</p>
                    <p class="details">Nearest Access: < 5 mins | Oscoda Beach Park: ~5-10 mins | Tawas Point SP: ~20-25 mins</p>
                    <a href="#beach-details">More Beach Info <i class="fas fa-arrow-right ml-1"></i></a>
                </div>
                <div class="info-card">
                     <i class="fas fa-water icon"></i>
                    <h3>Au Sable River Fun</h3>
                    <p>Famous for canoeing, kayaking, tubing, and scenic beauty. Rentals available locally.</p>
                     <p class="details">Oscoda Canoe Rental: ~5-10 mins</p>
                     <a href="tel:9897399040">Call Oscoda Canoe Rental <i class="fas fa-phone ml-1"></i></a>
                </div>
                 <div class="info-card">
                     <i class="fas fa-hiking icon"></i>
                    <h3>Hiking Adventures</h3>
                    <p>Explore diverse trails like Highbanks, Eagle Run, and Corsair through the Huron National Forest.</p>
                    <p class="details">Access Points: ~10-25 mins drive</p>
                    <a href="https://oscoda.com/project/trails/" target="_blank">View Trail Info <i class="fas fa-external-link-alt ml-1"></i></a>
                </div>
                 <div class="info-card">
                     <i class="fas fa-ship icon"></i>
                    <h3>AuSable River Queen</h3>
                    <p>Relax on a scenic paddlewheel boat tour down the majestic Au Sable River.</p>
                     <p class="details">Departure Point: ~10-15 mins drive</p>
                     <a href="https://www.ausableriverqueen.com/" target="_blank">Visit Website <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
                 <div class="info-card">
                     <i class="fas fa-beer-mug-empty icon"></i>
                    <h3>Local Brews & Bites</h3>
                    <p>Unwind at Wiltse's Brew Pub or grab a bite at local spots like the Office Lounge & Grill.</p>
                     <p class="details">Wiltse's / Office Lounge: ~5-10 mins</p>
                     <a href="#taste">See Food Options <i class="fas fa-arrow-right ml-1"></i></a>
                 </div>
                 <div class="info-card bg-yellow-50 border border-yellow-200">
                      <i class="fas fa-info-circle icon text-yellow-600"></i>
                     <h3>ATV/E-Bike Rentals</h3>
                     <p>Note: Dedicated ATV/ORV and E-Bike rentals are not readily available directly in Oscoda (< 35 min). Rentals may be found further afield.</p>
                     <p class="details">Check areas like Mio or West Branch.</p>
                     <span class="text-sm text-yellow-700 mt-auto">Plan Accordingly</span>
                 </div>
            </div>
        </section>

        <section id="taste" class="mb-16 fade-in" style="animation-delay: 0.6s;">
             <h2 class="section-heading"><i class="fas fa-utensils mr-2"></i>Taste of the Sunrise Coast</h2>
             <div class="section-heading-divider"></div>
             <p class="text-center text-gray-600 mb-10 max-w-3xl mx-auto">From local brews and pizza to fresh BBQ and finer dining, find flavors to satisfy every craving.</p>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                 <div class="info-card border-2 border-yellow-400">
                     <i class="fas fa-trophy icon text-yellow-600"></i> <h3>Route 23 BBQ (Local Fav!)</h3>
                    <p>Highly recommended spot in East Tawas known for brisket, ribs, pulled pork, and homemade sides.</p>
                     <p class="details">Drive: ~15-20 mins | Casual BBQ</p>
                     <a href="https://route23bbq.com/" target="_blank">Visit Website <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
                <div class="info-card">
                     <i class="fas fa-beer-mug-empty icon"></i>
                    <h3>Wiltse's Brew Pub</h3>
                    <p>Family restaurant with pub fare (burgers, sandwiches, dinners) and their own craft brews.</p>
                     <p class="details">Drive: ~5-10 mins | Pub Food/Brewery</p>
                     <a href="http://places.singleplatform.com/wiltses-brew-and-family-restaurant/menu" target="_blank">View Menu Snippet <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
                 <div class="info-card">
                    <i class="fas fa-pizza-slice icon"></i>
                    <h3>G's Pizzeria</h3>
                    <p>Popular spot for pizza, pocket pizzas, salads, wings, and some entrees.</p>
                     <p class="details">Drive: ~5-10 mins | Pizza/Casual</p>
                     <a href="https://order.toasttab.com/online/g-s-pizzeria-oscoda-5226-us-23" target="_blank">Order Online/Menu <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
                 <div class="info-card">
                     <i class="fas fa-concierge-bell icon"></i>
                    <h3>Tait's Bill of Fare</h3>
                    <p>Considered a finer dining option for the area, likely featuring steaks and seafood like local perch.</p>
                    <p class="details">Drive: ~5-10 mins | Finer Dining</p>
                    <span class="text-sm text-gray-500 mt-auto">No online menu found</span>
                 </div>
                <div class="info-card">
                    <i class="fas fa-hamburger icon"></i>
                    <h3>Office Lounge & Grill</h3>
                    <p>Local bar and grill likely serving typical casual American fare.</p>
                    <p class="details">Drive: ~5-10 mins | Bar & Grill</p>
                    <span class="text-sm text-gray-500 mt-auto">No confirmed menu found</span>
                </div>
                 <div class="info-card bg-green-50 border border-green-200">
                    <i class="fas fa-fire-burner icon text-green-600"></i>
                    <h3>Grill Master Zone</h3>
                    <p>Don't forget the charcoal! Perfect spot for grilling up some burgers or steaks after a day of exploring.</p>
                    <p class="details">Location: Your awesome rental!</p>
                    <span class="text-sm text-green-700 mt-auto">Enjoy the Outdoors!</span>
                 </div>
            </div>
        </section>

        <section id="attractions" class="mb-16 fade-in bg-blue-50 p-8 rounded-lg shadow-inner" style="animation-delay: 0.8s;">
             <h2 class="section-heading"><i class="fas fa-binoculars mr-2"></i>Nearby Attractions (< 35 Mins)</h2>
             <div class="section-heading-divider"></div>
             <p class="text-center text-gray-600 mb-10 max-w-3xl mx-auto">Explore historic lighthouses, breathtaking natural springs, aviation history, and prime wildlife viewing areas.</p>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                 <div class="info-card">
                    <i class="fas fa-leaf icon"></i>
                    <h3>Iargo Springs</h3>
                    <p>Sacred Native American site with stunning Au Sable River views, boardwalks, and natural springs.</p>
                    <p class="details">Drive: ~20-25 mins</p>
                    <a href="https://www.fs.usda.gov/recarea/hmnf/recarea/?recid=18711" target="_blank">Learn More <i class="fas fa-external-link-alt ml-1"></i></a>
                </div>
                <div class="info-card">
                     <i class="fas fa-monument icon"></i>
                    <h3>Lumberman's Monument</h3>
                    <p>Visitor center interpreting logging history with displays, trails, and scenic overlooks.</p>
                     <p class="details">Drive: ~20-25 mins</p>
                     <a href="https://www.fs.usda.gov/recarea/hmnf/recarea/?recid=18534" target="_blank">Learn More <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
                 <div class="info-card">
                     <i class="fas fa-broadcast-tower icon"></i>
                    <h3>Tawas Point Lighthouse</h3>
                    <p>Iconic Victorian-era lighthouse on Lake Huron within Tawas Point State Park. Tours often available.</p>
                     <p class="details">Drive: ~20-25 mins | Seasonal</p>
                     <a href="https://www.michigan.gov/dnr/places/state-parks/tawas-point" target="_blank">Park Info <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
                 <div class="info-card">
                     <i class="fas fa-broadcast-tower icon"></i>
                    <h3>Sturgeon Point Lighthouse</h3>
                    <p>Historic 1870 lighthouse north of Oscoda with keeper's quarters and maritime museum.</p>
                     <p class="details">Drive: ~30-35 mins | Seasonal</p>
                     <a href="https://alconahistoricalsociety.com/sturgeon-point-lighthouse/" target="_blank">Learn More <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
                <div class="info-card">
                     <i class="fas fa-plane icon"></i>
                    <h3>Wurtsmith Air Museum</h3>
                    <p>Explore aviation history and military aircraft on the grounds of the former Air Force Base.</p>
                     <p class="details">Drive: ~10-15 mins | Seasonal (Weekends)</p>
                     <a href="https://www.wurtsmithairmuseum.net/" target="_blank">Visit Website <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
                 <div class="info-card">
                     <i class="fas fa-binoculars icon"></i> <h3>Tuttle Marsh Wildlife Area</h3>
                    <p>5000-acre wetland ideal for birdwatching (eagles, swans, waterfowl) and wildlife viewing.</p>
                     <p class="details">Drive: ~15-20 mins</p>
                     <a href="https://www.michigan.gov/dnr/places/state-wildlife-areas/southeast-lp/tuttle-marsh" target="_blank">Learn More <i class="fas fa-external-link-alt ml-1"></i></a>
                 </div>
            </div>
        </section>

        <section id="golf" class="mb-16 fade-in" style="animation-delay: 1.0s;">
             <h2 class="section-heading"><i class="fas fa-golf-ball-tee mr-2"></i>Tee Time Nearby</h2>
             <div class="section-heading-divider"></div>
             <p class="text-center text-gray-600 mb-10 max-w-3xl mx-auto">Hit the links at scenic courses along the Sunrise Coast. Plenty of chances to shoot a great round!</p>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="golf-card">
                    <img src="https://placehold.co/600x400/166534/ecfdf5?text=Lakewood+Shores:+The+Gailes+(Placeholder)" alt="Placeholder image of Lakewood Shores golf course" onerror="this.src='https://placehold.co/600x400/cccccc/999999?text=Image+Not+Available'; this.alt='Image Not Available'">
                    <div class="content">
                        <h3>Lakewood Shores Resort</h3>
                        <p>Resort offering multiple courses with varied designs, including the unique Scottish links-style "Gailes".</p>
                        <div class="details">
                           <div class="detail-item"><i class="fas fa-map-marker-alt"></i> Oscoda, MI</div>
                           <div class="detail-item"><i class="fas fa-clock"></i> Est. Time: ~10-15 min</div>
                           <div class="detail-item"><i class="fas fa-star"></i> Rating: 4.5 Stars (Resort)</div>
                           <div class="detail-item"><i class="fas fa-dollar-sign"></i> Est. Price: ~$50 - $100+</div>
                        </div>
                        <div class="links">
                            <a href="https://lakewoodshores.com/golf/" target="_blank">Visit Website <i class="fas fa-external-link-alt ml-1"></i></a><br>
                            <span class="text-xs text-gray-400">Drone footage not readily found.</span>
                        </div>
                    </div>
                </div>
                <div class="golf-card">
                     <img src="https://placehold.co/600x400/7f1d1d/fef2f2?text=Red+Hawk+GC:+Rolling+Hills+(Placeholder)" alt="Placeholder image of Red Hawk golf course" onerror="this.src='https://placehold.co/600x400/cccccc/999999?text=Image+Not+Available'; this.alt='Image Not Available'">
                     <div class="content">
                        <h3>Red Hawk Golf Club</h3>
                        <p>Well-regarded public course located just west of East Tawas, known for good conditions.</p>
                         <div class="details">
                            <div class="detail-item"><i class="fas fa-map-marker-alt"></i> East Tawas, MI</div>
                            <div class="detail-item"><i class="fas fa-clock"></i> Est. Time: ~15-20 min</div>
                            <div class="detail-item"><i class="fas fa-star"></i> Rating: 4.6 Stars</div>
                            <div class="detail-item"><i class="fas fa-dollar-sign"></i> Est. Price: ~$45 - $60</div>
                        </div>
                        <div class="links">
                             <a href="https://www.redhawkgolf.net/" target="_blank">Visit Website <i class="fas fa-external-link-alt ml-1"></i></a><br>
                             <a href="https://www.youtube.com/watch?v=cnq5gIAebBk" target="_blank">Drone Flyover <i class="fas fa-video ml-1"></i></a> <span class="text-xs text-gray-400">(Link may be unavailable)</span>
                        </div>
                    </div>
                </div>
                 <div class="golf-card bg-red-50 border border-red-200">
                     <img src="https://placehold.co/600x400/991b1b/fef2f2?text=White+Deer+CC:+Up+North+Golf+(Placeholder)" alt="Placeholder image of White Deer Country Club" onerror="this.src='https://placehold.co/600x400/cccccc/999999?text=Image+Not+Available'; this.alt='Image Not Available'">
                     <div class="content">
                        <h3 class="text-red-800">White Deer Country Club</h3>
                        <p>Course located further inland near Hale. Note the longer estimated drive time.</p>
                         <div class="details text-red-600">
                            <div class="detail-item"><i class="fas fa-map-marker-alt"></i> Hale, MI</div>
                            <div class="detail-item"><i class="fas fa-clock"></i> Est. Time: ~35-45 min <strong>(> 30min)</strong></div>
                            <div class="detail-item"><i class="fas fa-star"></i> Rating: 4.4 Stars</div>
                            <div class="detail-item"><i class="fas fa-dollar-sign"></i> Est. Price: ~$35 - $45</div>
                        </div>
                         <div class="links">
                             <a href="http://whitedeercc.com/" target="_blank" class="text-red-600 hover:text-red-800">Visit Website <i class="fas fa-external-link-alt ml-1"></i></a><br>
                             <span class="text-xs text-red-400">Drone footage not readily found.</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

         <section id="beach-details" class="mb-16 fade-in" style="animation-delay: 1.1s;">
             <h2 class="section-heading"><i class="fas fa-umbrella-beach mr-2"></i>Lake Huron Beach Access</h2>
             <div class="section-heading-divider"></div>
             <p class="text-center text-gray-600 mb-10 max-w-3xl mx-auto">The rental is just moments from the Lake Huron shore. Here are some specific public access points:</p>
             <ul class="list-disc list-inside max-w-2xl mx-auto space-y-2 text-gray-600 bg-white p-6 rounded-lg shadow-lg">
                <li><strong>Direct Access:</strong> Small access points may be directly across US-23 (< 5 min walk/drive).</li>
                <li><strong>Oscoda Beach Park:</strong> Main town beach with pier, playground, facilities (~5-10 min drive North).</li>
                <li><strong>Three Mile Beach Park / Huron Sunrise Park:</strong> Natural beach setting (~10-15 min drive North).</li>
                <li><strong>Tawas City / East Tawas Beaches:</strong> Public beaches along US-23 through towns (~15-20 min drive South).</li>
                <li><strong>Tawas Point State Park Beach:</strong> Scenic beach within the state park (~20-25 min drive South).</li>
             </ul>
        </section>

        <section id="plan" class="mb-16 fade-in" style="animation-delay: 1.2s;">
             <h2 class="section-heading"><i class="fas fa-map-signs mr-2"></i>Plan Your Stay</h2>
             <div class="section-heading-divider"></div>
            <div class="grid md:grid-cols-2 gap-8">
                <div class="bg-white p-6 rounded-lg shadow-lg">
                    <h3 class="text-xl font-bold text-blue-800 mb-3"><i class="fas fa-car mr-2"></i>Getting Here</h3>
                    <p class="text-sm text-gray-600"><strong>From Allendale, MI (Approx):</strong></p>
                    <ul class="list-disc list-inside text-sm text-gray-600 ml-4">
                        <li>One Way: ~3.75 - 4 hours</li>
                        <li>Round Trip: ~7.5 - 8 hours</li>
                    </ul>
                     <p class="text-xs text-gray-500 mt-2">*(Drive times are estimates)*</p>
                </div>
                 <div class="bg-white p-6 rounded-lg shadow-lg">
                    <h3 class="text-xl font-bold text-blue-800 mb-3"><i class="fas fa-gas-pump mr-2"></i><i class="fas fa-shopping-cart mr-2"></i>Essentials</h3>
                    <p class="text-sm text-gray-600 mb-2">Gas stations and full grocery stores are readily available in Oscoda town (~5-10 min drive).</p>
                    <p class="text-xs text-gray-600"><strong>Nearest Grocery:</strong> Roger's Family Foods (~5.1 mi), Family Fare (~5.8 mi)</p>
                    <p class="text-xs text-gray-600"><strong>Nearest Gas:</strong> Admiral (~4.9 mi), Marathon (~5.2 mi), Shell (~5.3 mi)</p>
                </div>
            </div>
        </section>

    </main>

    <footer class="bg-gray-800 text-gray-300 text-center py-6 text-sm">
        <p>© 2025 Family Vacation - Hideout in the Wood Info. Created with assistance from AI.</p>
        <p>Please verify all details (hours, pricing, availability) before visiting.</p>
    </footer>

    <script>
        // Set the date we're counting down to
        const countDownDate = new Date("Aug 17, 2025 00:00:00").getTime();

        // Get elements to display the countdown
        const daysEl = document.getElementById("days");
        const hoursEl = document.getElementById("hours");
        const minutesEl = document.getElementById("minutes");
        const secondsEl = document.getElementById("seconds");
        const countdownBanner = document.getElementById("countdown-banner");


        // Update the count down every 1 second
        const countdownInterval = setInterval(function() {

            // Get today's date and time
            const now = new Date().getTime();

            // Find the distance between now and the count down date
            const distance = countDownDate - now;

            // Time calculations for days, hours, minutes and seconds
            const days = Math.floor(distance / (1000 * 60 * 60 * 24));
            const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((distance % (1000 * 60)) / 1000);

            // Display the result in the elements, checking if elements exist first
            if (daysEl && hoursEl && minutesEl && secondsEl) {
                daysEl.innerHTML = days < 10 ? '0' + days : days;
                hoursEl.innerHTML = hours < 10 ? '0' + hours : hours;
                minutesEl.innerHTML = minutes < 10 ? '0' + minutes : minutes;
                secondsEl.innerHTML = seconds < 10 ? '0' + seconds : seconds;
            } else {
                 // Clear interval if elements aren't found to prevent errors
                 // console.error("Countdown elements not found.");
                 // clearInterval(countdownInterval); // Optional: stop if elements missing
            }


            // If the count down is finished, write some text
            if (distance < 0) {
                clearInterval(countdownInterval);
                 if(countdownBanner) {
                    countdownBanner.innerHTML = "The Trip is Here! Have Fun!";
                 }
            }
        }, 1000);

         // Simple mobile menu toggle placeholder (requires more implementation)
         const menuButton = document.querySelector('header nav button');
         if (menuButton) {
            menuButton.addEventListener('click', () => {
                alert('Mobile menu toggle needs implementation!');
            });
         }

    </script>

</body>
</html>

