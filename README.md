<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>HairMaxx Solutions - Full Width</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#3b82f6',
            secondary: '#10b981',
            dark: '#1e293b',
            light: '#f8fafc'
          }
        }
      }
    };
  </script>
  <style>
    /* Reset default margins and paddings */
    html, body {
      margin: 0 !important;
      padding: 0 !important;
      width: 100vw;
      overflow-x: hidden;
    }

    /* Force full-width behavior */
    .force-full-width {
      width: 100vw;
      margin: 0;
      padding: 0;
      overflow-x: hidden;
    }

    /* Ensure all sections and wrappers span full width */
    section, header, footer, .w-full {
      width: 100vw !important;
      max-width: none !important;
      margin: 0 !important;
      padding: 0 !important;
    }

    /* Add consistent padding to content */
    .content-wrapper {
      padding-left: 16px;
      padding-right: 16px;
      width: 100%;
      box-sizing: border-box;
    }

    /* Center content with max-width where needed */
    .max-w-4xl-centered {
      max-width: 1024px;
      margin-left: auto;
      margin-right: auto;
      width: 100%;
    }

    /* Hero section gradient */
    .hero-gradient {
      background: linear-gradient(135deg, rgba(59, 130, 246, 0.8) 0%, rgba(16, 185, 129, 0.8) 100%);
    }

    /* Hover effect for product cards */
    .product-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
    }

    /* Active state for hair type buttons */
    .hair-type-btn.active {
      background-color: #3b82f6;
      color: white;
    }

    /* Progress bar animation */
    .progress-bar {
      transition: width 0.5s ease-in-out;
    }

    /* Ensure flex layouts use full width */
    .flex-full {
      width: 100%;
      display: flex;
      flex-wrap: wrap;
    }
  </style>
</head>
<body class="bg-light font-sans">
  <div class="force-full-width">
    <!-- Header -->
    <header class="bg-white shadow-md sticky top-0 z-50">
      <div class="content-wrapper flex justify-between items-center py-3">
        <div class="flex items-center space-x-2">
          <i class="fas fa-cut text-primary text-2xl"></i>
          <h1 class="text-xl font-bold text-dark">HairMaxx <span class="text-primary">Solutions</span></h1>
        </div>
        <nav class="hidden md:flex space-x-8">
          <a href="#causes" class="text-dark hover:text-primary transition">Causes</a>
          <a href="#solutions" class="text-dark hover:text-primary transition">Solutions</a>
          <a href="#products" class="text-dark hover:text-primary transition">Products</a>
          <a href="#faq" class="text-dark hover:text-primary transition">FAQ</a>
        </nav>
        <button class="md:hidden text-dark" id="menu-toggle">
          <i class="fas fa-bars text-2xl"></i>
        </button>
      </div>
      <div class="md:hidden hidden bg-white py-2 content-wrapper shadow-md" id="mobile-menu">
        <a href="#causes" class="block py-2 text-dark hover:text-primary transition">Causes</a>
        <a href="#solutions" class="block py-2 text-dark hover:text-primary transition">Solutions</a>
        <a href="#products" class="block py-2 text-dark hover:text-primary transition">Products</a>
        <a href="#faq" class="block py-2 text-dark hover:text-primary transition">FAQ</a>
      </div>
    </header>

    <!-- Hero Section -->
    <section class="hero-gradient text-white py-16 md:py-24">
      <div class="content-wrapper flex-full flex-col md:flex-row items-center">
        <div class="md:w-1/2 mb-8 md:mb-0">
          <h1 class="text-4xl md:text-5xl font-bold mb-4">Maximize Your Hair Growth Potential</h1>
          <p class="text-xl mb-8">Discover science-backed solutions and top-rated products to combat hair loss effectively.</p>
          <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
            <a href="#products" class="bg-white text-primary font-bold py-3 px-6 rounded-full hover:bg-opacity-90 transition text-center">Shop Recommended Products</a>
            <a href="#quiz" class="bg-transparent border-2 border-white text-white font-bold py-3 px-6 rounded-full hover:bg-white hover:text-primary transition text-center">Take Hair Quiz</a>
          </div>
        </div>
        <div class="md:w-1/2 flex justify-center">
          <img src="https://media.istockphoto.com/id/1368004438/photo/shot-of-a-couple-enjoying-a-day-at-the-beach.jpg?s=612x612&w=0&k=20&c=hMi6N-u6baFHC-P8C-8X_5iFshdPPicx7BCrBGM8ARc=" alt="Happy couple" class="max-w-full h-auto">
        </div>
      </div>
    </section>

    <!-- Hair Loss Stats -->
    <section class="py-12 bg-white">
      <div class="content-wrapper">
        <h2 class="text-3xl font-bold text-center text-dark mb-12">Understanding Hair Loss</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div class="bg-light p-6 rounded-lg shadow text-center">
            <div class="text-primary text-5xl font-bold mb-2">50%</div>
            <h3 class="text-xl font-semibold mb-2">Of Men by Age 50</h3>
            <p class="text-gray-600">Experience noticeable hair loss according to the American Hair Loss Association.</p>
          </div>
          <div class="bg-light p-6 rounded-lg shadow text-center">
            <div class="text-primary text-5xl font-bold mb-2">40%</div>
            <h3 class="text-xl font-semibold mb-2">Of Women</h3>
            <p class="text-gray-600">Show visible signs of hair loss by age 40, often due to hormonal changes.</p>
          </div>
          <div class="bg-light p-6 rounded-lg shadow text-center">
            <div class="text-primary text-5xl font-bold mb-2">100+</div>
            <h3 class="text-xl font-semibold mb-2">Hairs Daily</h3>
            <p class="text-gray-600">Losing 100-150 hairs per day is normal. More than that may indicate a problem.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Causes Section -->
    <section id="causes" class="py-16 bg-gray-50">
      <div class="content-wrapper">
        <h2 class="text-3xl font-bold text-center text-dark mb-4">Common Causes of Hair Loss</h2>
        <p class="text-center text-gray-600 max-w-2xl mx-auto mb-12">Understanding the root cause is the first step toward effective treatment.</p>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div class="bg-white p-6 rounded-lg shadow hover:shadow-md transition">
            <div class="bg-primary bg-opacity-10 w-12 h-12 rounded-full flex items-center justify-center mb-4">
              <i class="fas fa-dna text-primary text-xl"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Genetics (Androgenetic Alopecia)</h3>
            <p class="text-gray-600">The most common cause, affecting both men and women. It's hereditary and often develops gradually.</p>
          </div>
          <div class="bg-white p-6 rounded-lg shadow hover:shadow-md transition">
            <div class="bg-primary bg-opacity-10 w-12 h-12 rounded-full flex items-center justify-center mb-4">
              <i class="fas fa-stress text-primary text-xl"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Hormonal Changes</h3>
            <p class="text-gray-600">Pregnancy, menopause, thyroid problems, and other hormonal imbalances can cause temporary or permanent hair loss.</p>
          </div>
          <div class="bg-white p-6 rounded-lg shadow hover:shadow-md transition">
            <div class="bg-primary bg-opacity-10 w-12 h-12 rounded-full flex items-center justify-center mb-4">
              <i class="fas fa-pills text-primary text-xl"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Medical Conditions & Medications</h3>
            <p class="text-gray-600">Alopecia areata, scalp infections, and drugs for cancer, arthritis, depression can lead to hair loss.</p>
          </div>
          <div class="bg-white p-6 rounded-lg shadow hover:shadow-md transition">
            <div class="bg-primary bg-opacity-10 w-12 h-12 rounded-full flex items-center justify-center mb-4">
              <i class="fas fa-heartbeat text-primary text-xl"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Nutritional Deficiencies</h3>
            <p class="text-gray-600">Lack of protein, iron, zinc, vitamin D, and other nutrients can affect hair growth cycles.</p>
          </div>
          <div class="bg-white p-6 rounded-lg shadow hover:shadow-md transition">
            <div class="bg-primary bg-opacity-10 w-12 h-12 rounded-full flex items-center justify-center mb-4">
              <i class="fas fa-brain text-primary text-xl"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Stress & Trauma</h3>
            <p class="text-gray-600">Physical or emotional stress can trigger temporary hair shedding (telogen effluvium).</p>
          </div>
          <div class="bg-white p-6 rounded-lg shadow hover:shadow-md transition">
            <div class="bg-primary bg-opacity-10 w-12 h-12 rounded-full flex items-center justify-center mb-4">
              <i class="fas fa-cut text-primary text-xl"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Hairstyling & Treatments</h3>
            <p class="text-gray-600">Tight hairstyles, harsh chemicals, and excessive heat can cause traction alopecia.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Solutions Section -->
    <section id="solutions" class="py-16 bg-white">
      <div class="content-wrapper">
        <h2 class="text-3xl font-bold text-center text-dark mb-4">Effective Solutions for Hair Loss</h2>
        <p class="text-center text-gray-600 max-w-2xl mx-auto mb-12">From medical treatments to lifestyle changes, explore proven methods to combat hair loss.</p>
        <div class="flex flex-col md:flex-row mb-12 bg-gray-50 rounded-lg overflow-hidden">
          <div class="md:w-1/2 p-8">
            <h3 class="text-2xl font-semibold mb-4">Medical Treatments</h3>
            <div class="space-y-4">
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 mt-1 flex-shrink-0">1</div>
                <div>
                  <h4 class="font-semibold">Minoxidil (Rogaine)</h4>
                  <p class="text-gray-600">Over-the-counter topical treatment that stimulates hair follicles and slows hair loss.</p>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 mt-1 flex-shrink-0">2</div>
                <div>
                  <h4 class="font-semibold">Finasteride (Propecia)</h4>
                  <p class="text-gray-600">Prescription pill for men that blocks the hormone responsible for hair loss.</p>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 mt-1 flex-shrink-0">3</div>
                <div>
                  <h4 class="font-semibold">Low-Level Laser Therapy</h4>
                  <p class="text-gray-600">FDA-cleared devices that use light energy to stimulate hair growth.</p>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 mt-1 flex-shrink-0">4</div>
                <div>
                  <h4 class="font-semibold">Platelet-Rich Plasma (PRP)</h4>
                  <p class="text-gray-600">Injection treatment using your own blood's growth factors to stimulate follicles.</p>
                </div>
              </div>
            </div>
          </div>
          <div class="md:w-1/2 bg-primary bg-opacity-10 p-8">
            <h3 class="text-2xl font-semibold mb-4">Natural & Lifestyle Approaches</h3>
            <div class="space-y-4">
              <div class="flex items-start">
                <div class="bg-secondary text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 mt-1 flex-shrink-0">1</div>
                <div>
                  <h4 class="font-semibold">Nutrition Optimization</h4>
                  <p class="text-gray-600">Ensure adequate protein, iron, zinc, biotin, and vitamins D, E, and B complex.</p>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-secondary text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 mt-1 flex-shrink-0">2</div>
                <div>
                  <h4 class="font-semibold">Scalp Massage</h4>
                  <p class="text-gray-600">Improves circulation and may promote hair thickness when done regularly.</p>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-secondary text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 mt-1 flex-shrink-0">3</div>
                <div>
                  <h4 class="font-semibold">Stress Management</h4>
                  <p class="text-gray-600">Yoga, meditation, and adequate sleep can help reduce stress-related hair loss.</p>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-secondary text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 mt-1 flex-shrink-0">4</div>
                <div>
                  <h4 class="font-semibold">Gentle Hair Care</h4>
                  <p class="text-gray-600">Avoid tight hairstyles, limit heat styling, and use mild, nourishing hair products.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="bg-gray-50 rounded-lg p-8">
          <h3 class="text-2xl font-semibold mb-6 text-center">Hair Growth Timeline</h3>
          <div class="max-w-4xl mx-auto">
            <div class="flex justify-between mb-2">
              <span class="text-sm font-medium">0 Months</span>
              <span class="text-sm font-medium">3 Months</span>
              <span class="text-sm font-medium">6 Months</span>
              <span class="text-sm font-medium">12+ Months</span>
            </div>
            <div class="w-full bg-gray-200 rounded-full h-4 mb-6">
              <div class="progress-bar bg-primary h-4 rounded-full" style="width: 0%" id="progress-bar"></div>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
              <div class="text-center">
                <div class="bg-white p-3 rounded-lg shadow mb-2">
                  <i class="fas fa-search text-primary text-2xl"></i>
                </div>
                <p class="text-sm">Diagnosis & Treatment Begins</p>
              </div>
              <div class="text-center">
                <div class="bg-white p-3 rounded-lg shadow mb-2">
                  <i class="fas fa-leaf text-primary text-2xl"></i>
                </div>
                <p class="text-sm">Reduced Shedding</p>
              </div>
              <div class="text-center">
                <div class="bg-white p-3 rounded-lg shadow mb-2">
                  <i class="fas fa-seedling text-primary text-2xl"></i>
                </div>
                <p class="text-sm">New Hair Growth</p>
              </div>
              <div class="text-center">
                <div class="bg-white p-3 rounded-lg shadow mb-2">
                  <i class="fas fa-award text-primary text-2xl"></i>
                </div>
                <p class="text-sm">Full Results Visible</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Products Section -->
    <section id="products" class="py-16 bg-gray-50">
      <div class="content-wrapper">
        <h2 class="text-3xl font-bold text-center text-dark mb-4">Top-Rated Hair Loss Products</h2>
        <p class="text-center text-gray-600 max-w-2xl mx-auto mb-12">These Amazon products have helped thousands combat hair loss effectively.</p>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div class="bg-white rounded-lg shadow-md overflow-hidden product-card transition duration-300">
            <div class="relative">
              <img src="https://encrypted-tbn2.gstatic.com/shopping?q=tbn9GcTYz5U8NZG_guR-cwzwm63Dzxw7ornk2-zCpBpxrWOOxFBr8QgNTCTJmD-A-uklFieU9jLZ8UX5Fe31vxtbc061ncXRK3YHKSkZ7TpfQHjxXM3ccrLzUS2JIF8sziiaq5rzh1kA_m415gM&usqp=CAc" alt="Minoxidil Foam" class="w-full h-64 object-contain">
              <div class="absolute top-2 right-2 bg-primary text-white text-xs font-bold px-2 py-1 rounded">ESSENTIAL OIL</div>
            </div>
            <div class="p-6">
              <h3 class="text-xl font-semibold mb-2">Seven Minerals Pumpkin Seed Oil</h3>
              <div class="flex items-center mb-2">
                <div class="flex text-yellow-400">
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star-half-alt"></i>
                </div>
                <span class="text-gray-600 ml-2">143 reviews</span>
              </div>
              <p class="text-gray-600 mb-4">Rich in vitamins and nutrients, this Organic Pumpkin Seed Oil for hair deeply moisturizes, strengthens, and promotes hair growth.</p>
              <div class="flex justify-between items-center">
                <span class="text-xl font-bold text-dark">$24.95</span>
                <a href="https://amzn.to/4mbapHh" target="_blank" class="bg-primary text-white px-4 py-2 rounded hover:bg-blue-600 transition">View on Amazon</a>
              </div>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow-md overflow-hidden product-card transition duration-300">
            <div class="relative">
              <img src="https://m.media-amazon.com/images/I/71PbwAYEOFL._AC_UL320_.jpg" alt="Women's Rogaine" class="w-full h-64 object-contain">
              <div class="absolute top-2 right-2 bg-secondary text-white text-xs font-bold px-2 py-1 rounded">HERB</div>
            </div>
            <div class="p-6">
              <h3 class="text-xl font-semibold mb-2">Extra Strength Saw Palmetto Extract</h3>
              <div class="flex items-center mb-2">
                <div class="flex text-yellow-400">
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                </div>
                <span class="text-gray-600 ml-2">10,653 reviews</span>
              </div>
              <p class="text-gray-600 mb-4">Designed for both Men & Women, our extract of saw palmetto berries may block 5-alpha-reductase, an enzyme that converts testosterone to DHT.</p>
              <div class="flex justify-between items-center">
                <span class="text-xl font-bold text-dark">$12.99</span>
                <a href="https://amzn.to/4k8mIlS" target="_blank" class="bg-primary text-white px-4 py-2 rounded hover:bg-blue-600 transition">View on Amazon</a>
              </div>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow-md overflow-hidden product-card transition duration-300">
            <div class="relative">
              <img src="https://m.media-amazon.com/images/I/618yn5srweL.jpg" alt="Hair Growth Vitamins" class="w-full h-64 object-contain">
              <div class="absolute top-2 right-2 bg-primary text-white text-xs font-bold px-2 py-1 rounded">TECHNOLOGY</div>
            </div>
            <div class="p-6">
              <h3 class="text-xl font-semibold mb-2">Titanium Microneedles Derma Roller</h3>
              <div class="flex items-center mb-2">
                <div class="flex text-yellow-400">
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                </div>
                <span class="text-gray-600 ml-2">288 reviews</span>
              </div>
              <p class="text-gray-600 mb-4">This titanium derma roller for hair growth gently stimulates the scalp with fine needles, improving circulation and supporting healthier, fuller-looking hair.</p>
              <div class="flex justify-between items-center">
                <span class="text-xl font-bold text-dark">$9.99</span>
                <a href="https://amzn.to/3GSFAXS" target="_blank" class="bg-primary text-white px-4 py-2 rounded hover:bg-blue-600 transition">View on Amazon</a>
              </div>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow-md overflow-hidden product-card transition duration-300">
            <div class="relative">
              <img src="https://m.media-amazon.com/images/I/61CxI4PidHL._AC_UL320_.jpg" alt="Laser Cap" class="w-full h-64 object-contain">
              <div class="absolute top-2 right-2 bg-secondary text-white text-xs font-bold px-2 py-1 rounded">SUPPLEMENT</div>
            </div>
            <div class="p-6">
              <h3 class="text-xl font-semibold mb-2">Biotin 10000mcg Supplement</h3>
              <div class="flex items-center mb-2">
                <div class="flex text-yellow-400">
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star-half-alt"></i>
                </div>
                <span class="text-gray-600 ml-2">686 reviews</span>
              </div>
              <p class="text-gray-600 mb-4">Biotin softgels expertly crafted to nurture your hair, skin, and nails, helping you radiate confidence.</p>
              <div class="flex justify-between items-center">
                <span class="text-xl font-bold text-dark">$9.79</span>
                <a href="https://amzn.to/3ZeZ2US" target="_blank" class="bg-primary text-white px-4 py-2 rounded hover:bg-blue-600 transition">View on Amazon</a>
              </div>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow-md overflow-hidden product-card transition duration-300">
            <div class="relative">
              <img src="https://m.media-amazon.com/images/I/71bMtJeNGHL._AC_UL320_.jpg" alt="DHT Blocker Shampoo" class="w-full h-64 object-contain">
              <div class="absolute top-2 right-2 bg-primary text-white text-xs font-bold px-2 py-1 rounded">SHAMPOO</div>
            </div>
            <div class="p-6">
              <h3 class="text-xl font-semibold mb-2">PURA D'OR Hair Thinning Therapy Shampoo</h3>
              <div class="flex items-center mb-2">
                <div class="flex text-yellow-400">
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star-half-alt"></i>
                </div>
                <span class="text-gray-600 ml-2">29,319 reviews</span>
              </div>
              <p class="text-gray-600 mb-4">Gold standard shampoo with DHT blockers, biotin, and natural ingredients to reduce hair thinning.</p>
              <div class="flex justify-between items-center">
                <span class="text-xl font-bold text-dark">$29.99</span>
                <a href="https://amzn.to/4klc7Ex" target="_blank" class="bg-primary text-white px-4 py-2 rounded hover:bg-blue-600 transition">View on Amazon</a>
              </div>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow-md overflow-hidden product-card transition duration-300">
            <div class="relative">
              <img src="https://encrypted-tbn2.gstatic.com/shopping?q=tbn9GcSpqFUGAFomdR-2deE0Fo7YBHTUV0itbx3aCMfLZCNmDCPrnQ7eJaRzbXW81iAX1y-WGH8bjhYsQJr5NWLwsUSD1HJWuvVVGwbSICvg9nP4WGZwUozwUe6OK_J5GGxLqnSwT9tuUx6WCg&usqp=CAc" alt="Scalp Massager" class="w-full h-64 object-contain">
              <div class="absolute top-2 right-2 bg-secondary text-white text-xs font-bold px-2 py-1 rounded">TOOL</div>
            </div>
            <div class="p-6">
              <h3 class="text-xl font-semibold mb-2">Silicone Scalp Massager</h3>
              <div class="flex items-center mb-2">
                <div class="flex text-yellow-400">
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                  <i class="fas fa-star"></i>
                </div>
                <span class="text-gray-600 ml-2">1,211 reviews</span>
              </div>
              <p class="text-gray-600 mb-4">Gentle silicone bristles stimulate blood flow to hair follicles while cleansing the scalp.</p>
              <div class="flex justify-between items-center">
                <span class="text-xl font-bold text-dark">$6.99</span>
                <a href="https://amzn.to/4mcDy55" target="_blank" class="bg-primary text-white px-4 py-2 rounded hover:bg-blue-600 transition">View on Amazon</a>
              </div>
            </div>
          </div>
        </div>
        <div class="mt-12 text-center">
          <a href="https://www.amazon.com/s?k=natural+hair+loss+treatment&crid=3NLEVMB1EEKI7&sprefix=natural+hair+loss+%2Caps%2C217&ref=nb_sb_ss_p13n-pd-dpltr-ranker_1_18" target="_blank" class="inline-block bg-dark text-white px-6 py-3 rounded-lg hover:bg-opacity-90 transition">View More Natural Hair Growth Products</a>
        </div>
      </div>
    </section>

    <!-- Hair Quiz Section -->
    <section id="quiz" class="py-16 bg-white">
      <div class="content-wrapper max-w-4xl-centered">
        <h2 class="text-3xl font-bold text-center text-dark mb-4">Personalized Hair Loss Solution Finder</h2>
        <p class="text-center text-gray-600 mb-12">Answer a few questions to get customized product recommendations.</p>
        <div class="bg-gray-50 rounded-lg p-8">
          <div class="mb-8">
            <div class="flex justify-between mb-2">
              <span class="text-sm font-medium">Progress</span>
              <span class="text-sm font-medium" id="quiz-progress">1/5</span>
            </div>
            <div class="w-full bg-gray-200 rounded-full h-2">
              <div class="bg-primary h-2 rounded-full" style="width: 20%" id="quiz-progress-bar"></div>
            </div>
          </div>
          <div id="quiz-container">
            <div class="quiz-step active" data-step="1">
              <h3 class="text-xl font-semibold mb-6">1. What is your primary hair loss concern?</h3>
              <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="thinning">
                  <h4 class="font-medium mb-1">General Thinning</h4>
                  <p class="text-sm text-gray-600">Overall reduction in hair density</p>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="receding">
                  <h4 class="font-medium mb-1">Receding Hairline</h4>
                  <p class="text-sm text-gray-600">Hairline moving backward</p>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="bald-spots">
                  <h4 class="font-medium mb-1">Bald Spots</h4>
                  <p class="text-sm text-gray-600">Circular patches of hair loss</p>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="excessive-shedding">
                  <h4 class="font-medium mb-1">Excessive Shedding</h4>
                  <p class="text-sm text-gray-600">Losing more hair than usual</p>
                </button>
              </div>
            </div>
            <div class="quiz-step hidden" data-step="2">
              <h3 class="text-xl font-semibold mb-6">2. How long have you been experiencing hair loss?</h3>
              <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="less-than-6">
                  <h4 class="font-medium mb-1">Less than 6 months</h4>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="6-12">
                  <h4 class="font-medium mb-1">6-12 months</h4>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="1-3">
                  <h4 class="font-medium mb-1">1-3 years</h4>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="more-than-3">
                  <h4 class="font-medium mb-1">More than 3 years</h4>
                </button>
              </div>
            </div>
            <div class="quiz-step hidden" data-step="3">
              <h3 class="text-xl font-semibold mb-6">3. What is your gender?</h3>
              <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="male">
                  <h4 class="font-medium mb-1">Male</h4>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="female">
                  <h4 class="font-medium mb-1">Female</h4>
                </button>
              </div>
            </div>
            <div class="quiz-step hidden" data-step="4">
              <h3 class="text-xl font-semibold mb-6">4. Have you tried any hair loss treatments before?</h3>
              <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="yes-medical">
                  <h4 class="font-medium mb-1">Yes, medical treatments</h4>
                  <p class="text-sm text-gray-600">Minoxidil, Finasteride, etc.</p>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="yes-natural">
                  <h4 class="font-medium mb-1">Yes, natural remedies</h4>
                  <p class="text-sm text-gray-600">Essential oils, supplements</p>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="no">
                  <h4 class="font-medium mb-1">No, this is my first time</h4>
                </button>
              </div>
            </div>
            <div class="quiz-step hidden" data-step="5">
              <h3 class="text-xl font-semibold mb-6">5. What's your budget for hair loss solutions?</h3>
              <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="under-50">
                  <h4 class="font-medium mb-1">Under $50</h4>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="50-100">
                  <h4 class="font-medium mb-1">$50-$100</h4>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="100-200">
                  <h4 class="font-medium mb-1">$100-$200</h4>
                </button>
                <button class="hair-type-btn border-2 border-gray-200 rounded-lg p-4 text-left hover:border-primary transition" data-answer="over-200">
                  <h4 class="font-medium mb-1">Over $200</h4>
                </button>
              </div>
            </div>
            <div class="quiz-step hidden" id="quiz-results">
              <h3 class="text-xl font-semibold mb-6">Your Personalized Recommendations</h3>
              <div class="bg-white p-6 rounded-lg shadow mb-6">
                <h4 class="font-bold text-lg mb-3">Based on your answers, we recommend:</h4>
                <div id="recommendation-content">
                </div>
              </div>
              <div class="text-center">
                <button id="retake-quiz" class="bg-gray-200 text-dark px-6 py-2 rounded-lg hover:bg-gray-300 transition">Retake Quiz</button>
              </div>
            </div>
          </div>
          <div class="flex justify-between mt-8">
            <button id="quiz-prev" class="bg-gray-200 text-dark px-6 py-2 rounded-lg hover:bg-gray-300 transition hidden">Previous</button>
            <button id="quiz-next" class="bg-primary text-white px-6 py-2 rounded-lg hover:bg-blue-600 transition ml-auto">Next</button>
          </div>
        </div>
      </div>
    </section>

    <!-- FAQ Section -->
    <section id="faq" class="py-16 bg-gray-50">
      <div class="content-wrapper max-w-4xl-centered">
        <h2 class="text-3xl font-bold text-center text-dark mb-12">Frequently Asked Questions</h2>
        <div class="space-y-4">
          <div class="bg-white rounded-lg shadow overflow-hidden">
            <button class="faq-toggle w-full text-left p-6 flex justify-between items-center">
              <h3 class="text-lg font-semibold">How can I tell if I'm losing too much hair?</h3>
              <i class="fas fa-chevron-down text-primary transition-transform"></i>
            </button>
            <div class="faq-content px-6 pb-6 hidden">
              <p class="text-gray-600">It's normal to lose 50-150 hairs per day. Signs of excessive hair loss include:</p>
              <ul class="list-disc pl-5 mt-2 space-y-1 text-gray-600">
                <li>More hair than usual in your brush, shower drain, or pillow</li>
                <li>Visible thinning or widening part</li>
                <li>Receding hairline or bald spots</li>
                <li>Hair that comes out easily when gently pulled</li>
              </ul>
              <p class="mt-3 text-gray-600">If you're concerned, consult a dermatologist for proper diagnosis.</p>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow overflow-hidden">
            <button class="faq-toggle w-full text-left p-6 flex justify-between items-center">
              <h3 class="text-lg font-semibold">What's the difference between male and female pattern hair loss?</h3>
              <i class="fas fa-chevron-down text-primary transition-transform"></i>
            </button>
            <div class="faq-content px-6 pb-6 hidden">
              <p class="text-gray-600">While both are forms of androgenetic alopecia (hereditary hair loss), they present differently:</p>
              <div class="grid md:grid-cols-2 gap-6 mt-4">
                <div>
                  <h4 class="font-semibold text-primary mb-2">Male Pattern Baldness</h4>
                  <ul class="list-disc pl-5 space-y-1 text-gray-600">
                    <li>Typically begins with receding hairline at temples</li>
                    <li>Progresses to thinning at the crown</li>
                    <li>Often results in horseshoe-shaped hair pattern</li>
                    <li>Can begin as early as late teens</li>
                  </ul>
                </div>
                <div>
                  <h4 class="font-semibold text-primary mb-2">Female Pattern Hair Loss</h4>
                  <ul class="list-disc pl-5 space-y-1 text-gray-600">
                    <li>Usually begins with widening part</li>
                    <li>General thinning over the entire scalp</li>
                    <li>Hairline typically remains intact</li>
                    <li>Often begins around menopause but can start earlier</li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow overflow-hidden">
            <button class="faq-toggle w-full text-left p-6 flex justify-between items-center">
              <h3 class="text-lg font-semibold">How long does it take to see results from hair loss treatments?</h3>
              <i class="fas fa-chevron-down text-primary transition-transform"></i>
            </button>
            <div class="faq-content px-6 pb-6 hidden">
              <p class="text-gray-600">Hair growth is a slow process, and results vary by treatment:</p>
              <ul class="list-disc pl-5 mt-2 space-y-1 text-gray-600">
                <li><strong>Minoxidil:</strong> 3-6 months for reduced shedding, 6-12 months for visible regrowth</li>
                <li><strong>Finasteride:</strong> 3-6 months to stop hair loss, 6-12 months for regrowth</li>
                <li><strong>Laser therapy:</strong> 3-6 months for reduced shedding, 6-12 months for thickening</li>
                <li><strong>Nutritional supplements:</strong> 3-6 months for improved hair quality</li>
              </ul>
              <p class="mt-3 text-gray-600">Consistency is key—most treatments require ongoing use to maintain results.</p>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow overflow-hidden">
            <button class="faq-toggle w-full text-left p-6 flex justify-between items-center">
              <h3 class="text-lg font-semibold">Are there any side effects to common hair loss treatments?</h3>
              <i class="fas fa-chevron-down text-primary transition-transform"></i>
            </button>
            <div class="faq-content px-6 pb-6 hidden">
              <p class="text-gray-600">Possible side effects vary by treatment:</p>
              <div class="grid md:grid-cols-2 gap-6 mt-4">
                <div>
                  <h4 class="font-semibold text-primary mb-2">Minoxidil (Rogaine)</h4>
                  <ul class="list-disc pl-5 space-y-1 text-gray-600">
                    <li>Scalp irritation or dryness</li>
                    <li>Temporary increased shedding when first starting</li>
                    <li>Unwanted facial hair (in women)</li>
                  </ul>
                </div>
                <div>
                  <h4 class="font-semibold text-primary mb-2">Finasteride (Propecia)</h4>
                  <ul class="list-disc pl-5 space-y-1 text-gray-600">
                    <li>Decreased libido (rare)</li>
                    <li>Erectile dysfunction (rare)</li>
                    <li>Not approved for women of childbearing age</li>
                  </ul>
                </div>
              </div>
              <p class="mt-4 text-gray-600">Natural treatments typically have fewer side effects but may be less effective.</p>
            </div>
          </div>
          <div class="bg-white rounded-lg shadow overflow-hidden">
            <button class="faq-toggle w-full text-left p-6 flex justify-between items-center">
              <h3 class="text-lg font-semibold">Can hair loss be reversed naturally without medication?</h3>
              <i class="fas fa-chevron-down text-primary transition-transform"></i>
            </button>
            <div class="faq-content px-6 pb-6 hidden">
              <p class="text-gray-600">While natural methods may help, their effectiveness depends on the cause of hair loss:</p>
              <ul class="list-disc pl-5 mt-2 space-y-1 text-gray-600">
                <li><strong>Nutrition:</strong> Correcting deficiencies in iron, protein, biotin, zinc, and vitamin D can improve hair health</li>
                <li><strong>Scalp massage:</strong> May increase blood flow to follicles</li>
                <li><strong>Essential oils:</strong> Some studies suggest rosemary oil may be as effective as minoxidil for some types of hair loss</li>
                <li><strong>Stress reduction:</strong> Can help with stress-related shedding</li>
              </ul>
              <p class="mt-3 text-gray-600">For genetic hair loss, natural methods may slow progression but typically can't fully reverse it.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Newsletter -->
    <section class="py-12 bg-primary text-white">
      <div class="content-wrapper max-w-4xl-centered text-center">
        <h2 class="text-3xl font-bold mb-4">Stay Updated on Hair Loss Solutions</h2>
        <p class="text-xl mb-8">Subscribe to receive the latest research, product reviews, and exclusive discounts.</p>
        <div class="flex flex-col sm:flex-row max-w-md mx-auto sm:max-w-xl">
          <input type="email" placeholder="Your email address" class="flex-grow px-4 py-3 rounded sm:rounded-r-none mb-2 sm:mb-0 text-dark">
          <button type="button" class="bg-dark text-white px-6 py-3 rounded sm:rounded-l-none hover:bg-opacity-90 transition">Subscribe</button>
        </div>
        <p class="text-sm mt-4 opacity-80">We respect your privacy. Unsubscribe at any time.</p>
      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white py-12">
      <div class="content-wrapper">
        <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
          <div>
            <div class="flex items-center space-x-2 mb-4">
              <i class="fas fa-cut text-primary text-2xl"></i>
              <h3 class="text-xl font-bold">HairMaxx<span class="text-primary">Solutions</span></h3>
            </div>
            <p class="text-gray-400">Providing science-backed information and product recommendations to help you combat hair loss effectively.</p>
          </div>
          <div>
            <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
            <ul class="space-y-2">
              <li><a href="#causes" class="text-gray-400 hover:text-white transition">Causes of Hair Loss</a></li>
              <li><a href="#solutions" class="text-gray-400 hover:text-white transition">Treatment Options</a></li>
              <li><a href="#products" class="text-gray-400 hover:text-white transition">Recommended Products</a></li>
              <li><a href="#faq" class="text-gray-400 hover:text-white transition">FAQ</a></li>
            </ul>
          </div>
          <div>
            <h4 class="text-lg font-semibold mb-4">Resources</h4>
            <ul class="space-y-2">
              <li><a href="#" class="text-gray-400 hover:text-white transition">Hair Loss Studies</a></li>
              <li><a href="#" class="text-gray-400 hover:text-white transition">Expert Interviews</a></li>
              <li><a href="#" class="text-gray-400 hover:text-white transition">Success Stories</a></li>
              <li><a href="#" class="text-gray-400 hover:text-white transition">Blog</a></li>
            </ul>
          </div>
          <div>
            <h4 class="text-lg font-semibold mb-4">Connect</h4>
            <div class="flex space-x-4 mb-4">
              <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-facebook-f"></i></a>
              <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-twitter"></i></a>
              <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-instagram"></i></a>
              <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-pinterest"></i></a>
            </div>
            <p class="text-gray-400">Email: info@haircaresolutions.com</p>
          </div>
        </div>
        <div class="border-t border-gray-800 mt-8 pt-8 flex flex-col md:flex-row justify-between items-center">
          <p class="text-gray-400 mb-4 md:mb-0">© 2025 HairMaxx Solutions. All rights reserved.</p>
          <div class="flex space-x-6">
            <a href="#" class="text-gray-400 hover:text-white transition">Privacy Policy</a>
            <a href="#" class="text-gray-400 hover:text-white transition">Terms of Service</a>
            <a href="#" class="text-gray-400 hover:text-white transition">Disclaimer</a>
          </div>
        </div>
      </div>
    </footer>

    <script>
      // Mobile menu toggle
      document.getElementById('menu-toggle').addEventListener('click', function() {
        const menu = document.getElementById('mobile-menu');
        menu.classList.toggle('hidden');
      });

      // FAQ toggle functionality
      document.querySelectorAll('.faq-toggle').forEach(button => {
        button.addEventListener('click', function() {
          const content = this.nextElementSibling;
          const icon = this.querySelector('i');
          content.classList.toggle('hidden');
          if (content.classList.contains('hidden')) {
            icon.classList.remove('rotate-180');
          } else {
            icon.classList.add('rotate-180');
          }
        });
      });

      // Hair quiz functionality
      const quizSteps = document.querySelectorAll('.quiz-step');
      const nextButton = document.getElementById('quiz-next');
      const prevButton = document.getElementById('quiz-prev');
      const progressBar = document.getElementById('quiz-progress-bar');
      const progressText = document.getElementById('quiz-progress');
      const hairTypeBtns = document.querySelectorAll('.hair-type-btn');
      const retakeQuizBtn = document.getElementById('retake-quiz');
      let currentStep = 1;
      const totalSteps = 5;
      const answers = {};

      function updateProgress() {
        const progressPercent = (currentStep / totalSteps) * 100;
        progressBar.style.width = `${progressPercent}%`;
        progressText.textContent = `${currentStep}/${totalSteps}`;
        if (currentStep > 1) {
          prevButton.classList.remove('hidden');
        } else {
          prevButton.classList.add('hidden');
        }
        if (currentStep === totalSteps) {
          nextButton.textContent = 'Get Results';
        } else {
          nextButton.textContent = 'Next';
        }
      }

      function showStep(step) {
        quizSteps.forEach(stepElement => {
          stepElement.classList.add('hidden');
          stepElement.classList.remove('active');
        });
        const currentStepElement = document.querySelector(`.quiz-step[data-step="${step}"]`);
        currentStepElement.classList.remove('hidden');
        currentStepElement.classList.add('active');
        updateProgress();
      }

      nextButton.addEventListener('click', function() {
        if (currentStep === totalSteps) {
          showResults();
        } else {
          currentStep++;
          showStep(currentStep);
        }
      });

      prevButton.addEventListener('click', function() {
        currentStep--;
        showStep(currentStep);
      });

      hairTypeBtns.forEach(btn => {
        btn.addEventListener('click', function() {
          const currentStepElement = document.querySelector(`.quiz-step[data-step="${currentStep}"]`);
          currentStepElement.querySelectorAll('.hair-type-btn').forEach(button => {
            button.classList.remove('active', 'border-primary', 'bg-primary', 'text-white');
            button.classList.add('border-gray-200');
          });
          this.classList.add('active', 'border-primary', 'bg-primary', 'text-white');
          this.classList.remove('border-gray-200');
          const questionKey = `question${currentStep}`;
          answers[questionKey] = this.dataset.answer;
        });
      });

      retakeQuizBtn.addEventListener('click', function() {
        currentStep = 1;
        showStep(currentStep);
        document.getElementById('quiz-results').classList.add('hidden');
        nextButton.classList.remove('hidden');
        prevButton.classList.add('hidden');
      });

      function showResults() {
        quizSteps.forEach(step => {
          step.classList.add('hidden');
          step.classList.remove('active');
        });
        const resultsElement = document.getElementById('quiz-results');
        resultsElement.classList.remove('hidden');
        resultsElement.classList.add('active');
        nextButton.classList.add('hidden');
        const recommendationContent = document.getElementById('recommendation-content');
        let recommendationHTML = '';
        if (answers.question3 === 'male') {
          recommendationHTML = `
            <div class="space-y-4">
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-8 h-8 flex items-center justify-center mr-3 mt-1 flex-shrink-0">1</div>
                <div>
                  <h4 class="font-bold">Men's Rogaine 5% Minoxidil Foam</h4>
                  <p class="text-gray-600">Our top pick for men with hereditary hair loss. Easy to apply and clinically proven to regrow hair.</p>
                  <a href="https://www.amazon.com/Rogaine-Minoxidil-Regrowth-Treatment-2-11-Ounce/dp/B0026HDURA/" target="_blank" class="text-primary hover:underline inline-block mt-2">View on Amazon</a>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-8 h-8 flex items-center justify-center mr-3 mt-1 flex-shrink-0">2</div>
                <div>
                  <h4 class="font-bold">PURA D'OR Anti-Thinning Shampoo</h4>
                  <p class="text-gray-600">Gentle, DHT-blocking shampoo that helps reduce hair thinning while cleansing your scalp.</p>
                  <a href="https://www.amazon.com/PURA-DOR-Hair-Thinning-Therapy-Shampoo/dp/B005CQMV3A/" target="_blank" class="text-primary hover:underline inline-block mt-2">View on Amazon</a>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-8 h-8 flex items-center justify-center mr-3 mt-1 flex-shrink-0">3</div>
                <div>
                  <h4 class="font-bold">Nutrafol Men's Hair Growth Supplement</h4>
                  <p class="text-gray-600">Comprehensive nutritional support with clinically effective ingredients for men's hair health.</p>
                  <a href="https://www.amazon.com/Nutrafol-Men-Hair-Growth-Supplement/dp/B01N7KQ8Q3/" target="_blank" class="text-primary hover:underline inline-block mt-2">View on Amazon</a>
                </div>
              </div>
            </div>
          `;
        } else {
          recommendationHTML = `
            <div class="space-y-4">
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-8 h-8 flex items-center justify-center mr-3 mt-1 flex-shrink-0">1</div>
                <div>
                  <h4 class="font-bold">Women's Rogaine 5% Minoxidil Solution</h4>
                  <p class="text-gray-600">The only FDA-approved topical treatment clinically proven to regrow hair in women.</p>
                  <a href="https://www.amazon.com/Rogaine-Womens-Hair-Regrowth-Treatment/dp/B001ECQ6Z2/" target="_blank" class="text-primary hover:underline inline-block mt-2">View on Amazon</a>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-8 h-8 flex items-center justify-center mr-3 mt-1 flex-shrink-0">2</div>
                <div>
                  <h4 class="font-bold">Nutrafol Women's Hair Growth Supplement</h4>
                  <p class="text-gray-600">Doctor-recommended supplement that targets root causes of hair thinning in women.</p>
                  <a href="https://www.amazon.com/Nutrafol-Women-Hair-Growth-Supplement/dp/B01N7KQ8Q3/" target="_blank" class="text-primary hover:underline inline-block mt-2">View on Amazon</a>
                </div>
              </div>
              <div class="flex items-start">
                <div class="bg-primary text-white rounded-full w-8 h-8 flex items-center justify-center mr-3 mt-1 flex-shrink-0">3</div>
                <div>
                  <h4 class="font-bold">MAXSOFT Scalp Massager Shampoo Brush</h4>
                  <p class="text-gray-600">Gentle silicone bristles stimulate blood flow to hair follicles while cleansing your scalp.</p>
                  <a href="https://www.amazon.com/MAXSOFT-Scalp-Massager-Shampoo-Brush/dp/B07G9JQ5B4/" target="_blank" class="text-primary hover:underline inline-block mt-2">View on Amazon</a>
                </div>
              </div>
            </div>
          `;
        }
        recommendationContent.innerHTML = recommendationHTML;
      }

      window.addEventListener('load', function() {
        setTimeout(() => {
          const progressBar = document.getElementById('progress-bar');
          progressBar.style.width = '100%';
        }, 300);
      });
    </script>
  </div>
</body>
</html>

