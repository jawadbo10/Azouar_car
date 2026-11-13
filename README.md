<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AZAUAR CAR | كراء السيارات بالناظور</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;900&family=Montserrat:wght@400;600;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" />
  <style>
    :root {
      --brand-red: #8B0000;
      --brand-red-dark: #4A0000;
      --brand-gold: #F5B800;
      --brand-gold-hover: #D9A200;
    }

    body {
      font-family: 'Cairo', sans-serif;
      background-color: #0b0b0d;
      color: #f3f4f6;
      scroll-behavior: smooth;
    }

    html[dir="ltr"] body {
      font-family: 'Montserrat', sans-serif;
    }

    .brand-gradient {
      background: linear-gradient(135deg, #3a0000 0%, #8B0000 50%, #1a0505 100%);
    }

    .gold-gradient {
      background: linear-gradient(135deg, #F5B800 0%, #ffd54f 50%, #d49b00 100%);
    }

    .gold-text {
      background: linear-gradient(to right, #F5B800, #ffe082, #F5B800);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .glass-card {
      background: rgba(24, 24, 28, 0.85);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(245, 184, 0, 0.18);
    }

    .car-card {
      transition: transform 0.35s cubic-bezier(0.22, 1, 0.36, 1), box-shadow 0.35s ease, border-color 0.35s ease;
    }

    .car-card:hover {
      transform: translateY(-8px);
      border-color: #F5B800;
      box-shadow: 0 20px 35px -10px rgba(139, 0, 0, 0.45);
    }

    .lang-btn {
      cursor: pointer;
      touch-action: manipulation;
      user-select: none;
    }

    .lang-btn.active {
      background-color: #F5B800;
      color: #0b0b0d;
      font-weight: 800;
      box-shadow: 0 0 15px rgba(245, 184, 0, 0.5);
    }

    .filter-btn.active {
      background-color: #8B0000;
      border-color: #F5B800;
      color: #ffffff;
    }
  </style>
</head>
<body class="antialiased selection:bg-amber-500 selection:text-black">

  <!-- Top Bar -->
  <div class="bg-[#140202] border-b border-red-900/40 text-xs sm:text-sm py-2 px-4">
    <div class="max-w-7xl mx-auto flex flex-wrap items-center justify-between gap-2">
      <div class="flex items-center gap-4 text-gray-300">
        <a href="tel:+212668221538" dir="ltr" class="flex items-center gap-1.5 hover:text-amber-400 transition">
          <i class="fa-solid fa-phone text-amber-400"></i>
          <span>+212 668-221538</span>
        </a>
        <span class="hidden sm:inline text-gray-600">|</span>
        <span class="hidden sm:flex items-center gap-1.5">
          <i class="fa-solid fa-location-dot text-amber-400"></i>
          <span>Hay Baraka L157 - Nador</span>
        </span>
      </div>
      <div class="flex items-center gap-3">
        <span data-i18n="airportBadge" class="bg-red-900/60 border border-amber-500/40 text-amber-300 px-2.5 py-0.5 rounded-full text-xs font-semibold">
          توصيل مجاني لمطار الناظور العروي ✈️
        </span>
        <a href="https://www.instagram.com/azauar_car?xtok=OG8wa244YTBlazFv" target="_blank" rel="noopener noreferrer" class="text-gray-300 hover:text-amber-400 transition text-base" aria-label="Instagram">
          <i class="fa-brands fa-instagram"></i>
        </a>
      </div>
    </div>
  </div>

  <!-- Navbar -->
  <header class="sticky top-0 z-50 bg-[#0b0b0d]/95 backdrop-blur-md border-b border-white/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between gap-3">
      
      <!-- Logo -->
      <a href="#" class="flex items-center gap-3 group shrink-0">
        <div class="w-12 h-12 rounded-xl brand-gradient border border-amber-400/50 flex items-center justify-center shadow-lg shadow-red-950/60 group-hover:scale-105 transition">
          <svg class="w-8 h-8 text-amber-400" viewBox="0 0 64 40" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M6 26L13 13C15 9.5 18.5 8 22.5 8H41.5C45.5 8 49 9.5 51 13L58 26" stroke="currentColor" stroke-width="3.2" stroke-linecap="round"/>
            <path d="M3 26H61V32C61 33.6569 59.6569 35 58 35H6C4.34315 35 3 33.6569 3 32V26Z" fill="currentColor" fill-opacity="0.2" stroke="currentColor" stroke-width="2.8"/>
            <circle cx="16" cy="34" r="5" fill="#0b0b0d" stroke="currentColor" stroke-width="3"/>
            <circle cx="48" cy="34" r="5" fill="#0b0b0d" stroke="currentColor" stroke-width="3"/>
            <path d="M18 18H46" stroke="currentColor" stroke-width="2.2" stroke-linecap="round"/>
          </svg>
        </div>
        <div>
          <span class="block text-xl sm:text-2xl font-black tracking-wider leading-none">
            <span class="text-amber-400">AZAUAR</span> <span class="text-white">CAR</span>
          </span>
          <span data-i18n="logoSub" class="text-[11px] text-gray-400 tracking-widest uppercase">كراء السيارات بالناظور</span>
        </div>
      </a>

      <!-- Nav Links (Desktop) -->
      <nav class="hidden lg:flex items-center gap-7 text-sm font-semibold">
        <a href="#fleet" data-i18n="navFleet" class="text-gray-200 hover:text-amber-400 transition">أسطول السيارات</a>
        <a href="#services" data-i18n="navServices" class="text-gray-200 hover:text-amber-400 transition">خدماتنا</a>
        <a href="#conditions" data-i18n="navConditions" class="text-gray-200 hover:text-amber-400 transition">شروط الكراء</a>
        <a href="#booking" data-i18n="navBooking" class="text-gray-200 hover:text-amber-400 transition">احجز الآن</a>
        <a href="#contact" data-i18n="navContact" class="text-gray-200 hover:text-amber-400 transition">موقعنا</a>
      </nav>

      <!-- Instant Language Switcher -->
      <div class="flex items-center gap-1.5 bg-zinc-900 p-1 rounded-xl border border-white/15" role="group" aria-label="Language Switcher">
        <button type="button" data-lang="ar" class="lang-btn active px-3 py-1.5 rounded-lg text-xs sm:text-sm font-bold transition">العربية</button>
        <button type="button" data-lang="de" class="lang-btn px-3 py-1.5 rounded-lg text-xs sm:text-sm font-bold text-gray-300 hover:text-white transition">DE</button>
        <button type="button" data-lang="es" class="lang-btn px-3 py-1.5 rounded-lg text-xs sm:text-sm font-bold text-gray-300 hover:text-white transition">ES</button>
      </div>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="relative overflow-hidden brand-gradient border-b border-amber-500/20">
    <div class="absolute inset-0 opacity-15 pointer-events-none" style="background-image: radial-gradient(#F5B800 1px, transparent 1px); background-size: 28px 28px;"></div>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16 sm:py-24 relative z-10">
      <div class="grid lg:grid-cols-12 gap-10 items-center">
        
        <!-- Hero Content -->
        <div class="lg:col-span-7 space-y-6">
          <div class="inline-flex items-center gap-2 bg-black/40 border border-amber-400/40 px-4 py-1.5 rounded-full text-amber-300 text-xs sm:text-sm font-semibold">
            <i class="fa-solid fa-star text-amber-400"></i>
            <span data-i18n="heroTag">الاختيار الأول لكراء السيارات في الناظور والمطار</span>
          </div>

          <h1 data-i18n="heroTitle" class="text-3xl sm:text-5xl lg:text-6xl font-black leading-tight text-white">
            انطلق بكل حرية مع <span class="gold-text">AZAUAR CAR</span> في الناظور
          </h1>

          <p data-i18n="heroDesc" class="text-gray-200 text-base sm:text-lg max-w-2xl leading-relaxed">
            نقدم لك أحدث السيارات الاقتصادية والعائلية بناقل حركة أوتوماتيك ومانيول، مع خدمة التوصيل السريع إلى مطار الناظور العروي وأثمنة تنافسية.
          </p>

          <div class="flex flex-wrap items-center gap-4 pt-2">
            <a href="#booking" class="gold-gradient text-black font-extrabold px-7 py-3.5 rounded-xl shadow-lg shadow-amber-500/20 hover:opacity-95 transition flex items-center gap-2.5 text-sm sm:text-base">
              <i class="fa-brands fa-whatsapp text-xl"></i>
              <span data-i18n="heroCtaPrimary">احجز سيارتك عبر واتساب</span>
            </a>
            <a href="#fleet" class="bg-black/50 hover:bg-black/75 border border-white/20 text-white font-bold px-7 py-3.5 rounded-xl transition text-sm sm:text-base">
              <span data-i18n="heroCtaSecondary">استكشف السيارات</span>
            </a>
          </div>

          <!-- Quick Highlights -->
          <div class="grid grid-cols-3 gap-4 pt-6 border-t border-white/15 max-w-lg">
            <div>
              <span class="block text-xl sm:text-2xl font-black text-amber-400">24/7</span>
              <span data-i18n="statSupport" class="text-xs text-gray-300">خدمة متواصلة</span>
            </div>
            <div>
              <span class="block text-xl sm:text-2xl font-black text-amber-400">0 DH</span>
              <span data-i18n="statAirport" class="text-xs text-gray-300">توصيل للمطار</span>
            </div>
            <div>
              <span class="block text-xl sm:text-2xl font-black text-amber-400">AUTO / MAN</span>
              <span data-i18n="statGear" class="text-xs text-gray-300">أوتوماتيك ومانيول</span>
            </div>
          </div>
        </div>

        <!-- Hero Visual Showcase -->
        <div class="lg:col-span-5">
          <div class="glass-card rounded-3xl p-5 sm:p-6 shadow-2xl relative">
            <div class="flex items-center justify-between mb-4">
              <span class="text-xs font-bold uppercase tracking-wider text-amber-400" data-i18n="featuredLabel">أكثر السيارات طلباً</span>
              <span class="bg-emerald-500/20 text-emerald-300 border border-emerald-500/40 text-xs px-2.5 py-0.5 rounded-full font-semibold" data-i18n="availableNow">متوفرة الآن</span>
            </div>
            <div class="rounded-2xl overflow-hidden bg-zinc-900 border border-white/10 aspect-[16/10]">
              <img src="https://i.ibb.co/fddjV5Jf/essai-renault-clio-e-tech-full-hybrid-restylee-esprit-alpine-citadine-maroc-front.jpg" alt="Renault Clio AZAUAR CAR" class="w-full h-full object-cover" />
            </div>
            <div class="mt-4 flex items-center justify-between">
              <div>
                <h3 class="text-lg font-extrabold text-white">Renault Clio</h3>
                <p class="text-xs text-gray-400" data-i18n="heroCarSpec">أوتوماتيك ومانيول • تكييف • اقتصادية</p>
              </div>
              <a href="#booking" onclick="selectCarForBooking('Renault Clio')" class="bg-red-800 hover:bg-red-700 border border-amber-400/50 text-white text-xs font-bold px-4 py-2.5 rounded-xl transition" data-i18n="bookQuick">
                احجز الآن
              </a>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- Fleet Section -->
  <section id="fleet" class="py-16 sm:py-24 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex flex-col md:flex-row md:items-end justify-between gap-6 mb-12">
      <div>
        <span class="text-amber-400 font-bold text-sm uppercase tracking-wider" data-i18n="fleetSubtitle">سيارات حديثة ومجهزة بالكامل</span>
        <h2 class="text-3xl sm:text-4xl font-black text-white mt-1" data-i18n="fleetTitle">أسطول سيارات AZAUAR CAR</h2>
      </div>

      <!-- Filter Buttons -->
      <div class="flex flex-wrap gap-2">
        <button type="button" onclick="filterFleet('all', this)" class="filter-btn active px-4 py-2 rounded-xl border border-white/15 bg-zinc-900 text-xs sm:text-sm font-bold transition" data-i18n="filterAll">الكل</button>
        <button type="button" onclick="filterFleet('automatic', this)" class="filter-btn px-4 py-2 rounded-xl border border-white/15 bg-zinc-900 text-xs sm:text-sm font-bold transition" data-i18n="filterAuto">أوتوماتيك</button>
        <button type="button" onclick="filterFleet('manual', this)" class="filter-btn px-4 py-2 rounded-xl border border-white/15 bg-zinc-900 text-xs sm:text-sm font-bold transition" data-i18n="filterManual">مانيول</button>
      </div>
    </div>

    <!-- Cars Grid -->
    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
      
      <!-- Car 1: Dacia Duster -->
      <div class="car-card glass-card rounded-3xl overflow-hidden flex flex-col" data-transmission="automatic manual">
        <div class="relative aspect-[16/10] bg-zinc-900 overflow-hidden">
          <img src="https://i.ibb.co/FqqFWj8n/images-18.jpg" alt="Dacia Duster" class="w-full h-full object-cover" />
          <span class="absolute top-3 start-3 bg-black/75 backdrop-blur-md border border-amber-400/50 text-amber-300 text-xs font-bold px-3 py-1 rounded-full">
            SUV • 4x2 / 4x4
          </span>
        </div>
        <div class="p-6 flex-1 flex flex-col justify-between space-y-5">
          <div>
            <div class="flex items-center justify-between">
              <h3 class="text-2xl font-black text-white">Dacia Duster</h3>
              <span class="text-xs bg-red-900/60 text-amber-300 border border-red-700 px-2.5 py-1 rounded-lg font-bold" data-i18n="bothGears">أوتوماتيك / مانيول</span>
            </div>
            <p class="text-gray-400 text-sm mt-2" data-i18n="dusterDesc">سيارة قوية ومريحة مثالية للعائلات والسفر الطويل في جميع الطرقات.</p>
            
            <div class="grid grid-cols-3 gap-2 mt-5 pt-4 border-t border-white/10 text-center text-xs text-gray-300">
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-users text-amber-400 block mb-1"></i>
                <span data-i18n="seats5">5 مقاعد</span>
              </div>
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-gears text-amber-400 block mb-1"></i>
                <span data-i18n="gearShort">أوتو / مانيول</span>
              </div>
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-snowflake text-amber-400 block mb-1"></i>
                <span data-i18n="ac">مكيف</span>
              </div>
            </div>
          </div>

          <a href="#booking" onclick="selectCarForBooking('Dacia Duster')" class="w-full gold-gradient text-black font-extrabold py-3 rounded-xl text-center hover:opacity-95 transition flex items-center justify-center gap-2 text-sm">
            <i class="fa-brands fa-whatsapp text-lg"></i>
            <span data-i18n="reserveCar">احجز هذه السيارة</span>
          </a>
        </div>
      </div>

      <!-- Car 2: Renault Clio -->
      <div class="car-card glass-card rounded-3xl overflow-hidden flex flex-col" data-transmission="automatic manual">
        <div class="relative aspect-[16/10] bg-zinc-900 overflow-hidden">
          <img src="https://i.ibb.co/fddjV5Jf/essai-renault-clio-e-tech-full-hybrid-restylee-esprit-alpine-citadine-maroc-front.jpg" alt="Renault Clio" class="w-full h-full object-cover" />
          <span class="absolute top-3 start-3 bg-black/75 backdrop-blur-md border border-amber-400/50 text-amber-300 text-xs font-bold px-3 py-1 rounded-full">
            Citadine • Moderne
          </span>
        </div>
        <div class="p-6 flex-1 flex flex-col justify-between space-y-5">
          <div>
            <div class="flex items-center justify-between">
              <h3 class="text-2xl font-black text-white">Renault Clio</h3>
              <span class="text-xs bg-red-900/60 text-amber-300 border border-red-700 px-2.5 py-1 rounded-lg font-bold" data-i18n="bothGears">أوتوماتيك / مانيول</span>
            </div>
            <p class="text-gray-400 text-sm mt-2" data-i18n="clioDesc">تصميم عصري وأنيق مع استهلاك منخفض للوقود وسلاسة عالية في القيادة داخل المدينة.</p>
            
            <div class="grid grid-cols-3 gap-2 mt-5 pt-4 border-t border-white/10 text-center text-xs text-gray-300">
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-users text-amber-400 block mb-1"></i>
                <span data-i18n="seats5">5 مقاعد</span>
              </div>
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-gears text-amber-400 block mb-1"></i>
                <span data-i18n="gearShort">أوتو / مانيول</span>
              </div>
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-snowflake text-amber-400 block mb-1"></i>
                <span data-i18n="ac">مكيف</span>
              </div>
            </div>
          </div>

          <a href="#booking" onclick="selectCarForBooking('Renault Clio')" class="w-full gold-gradient text-black font-extrabold py-3 rounded-xl text-center hover:opacity-95 transition flex items-center justify-center gap-2 text-sm">
            <i class="fa-brands fa-whatsapp text-lg"></i>
            <span data-i18n="reserveCar">احجز هذه السيارة</span>
          </a>
        </div>
      </div>

      <!-- Car 3: Opel Corsa -->
      <div class="car-card glass-card rounded-3xl overflow-hidden flex flex-col" data-transmission="automatic manual">
        <div class="relative aspect-[16/10] bg-zinc-900 overflow-hidden">
          <img src="https://i.ibb.co/YT1RSW4C/Screenshot-20261113-203548-Google.jpg" alt="Opel Corsa" class="w-full h-full object-cover" />
          <span class="absolute top-3 start-3 bg-black/75 backdrop-blur-md border border-amber-400/50 text-amber-300 text-xs font-bold px-3 py-1 rounded-full">
            Compacte • Agile
          </span>
        </div>
        <div class="p-6 flex-1 flex flex-col justify-between space-y-5">
          <div>
            <div class="flex items-center justify-between">
              <h3 class="text-2xl font-black text-white">Opel Corsa</h3>
              <span class="text-xs bg-red-900/60 text-amber-300 border border-red-700 px-2.5 py-1 rounded-lg font-bold" data-i18n="bothGears">أوتوماتيك / مانيول</span>
            </div>
            <p class="text-gray-400 text-sm mt-2" data-i18n="corsaDesc">سيارة عملية وموثوقة تجمع بين الراحة والأداء الاقتصادي للتنقل اليومي في الناظور.</p>
            
            <div class="grid grid-cols-3 gap-2 mt-5 pt-4 border-t border-white/10 text-center text-xs text-gray-300">
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-users text-amber-400 block mb-1"></i>
                <span data-i18n="seats5">5 مقاعد</span>
              </div>
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-gears text-amber-400 block mb-1"></i>
                <span data-i18n="gearShort">أوتو / مانيول</span>
              </div>
              <div class="bg-zinc-900/90 p-2 rounded-xl">
                <i class="fa-solid fa-snowflake text-amber-400 block mb-1"></i>
                <span data-i18n="ac">مكيف</span>
              </div>
            </div>
          </div>

          <a href="#booking" onclick="selectCarForBooking('Opel Corsa')" class="w-full gold-gradient text-black font-extrabold py-3 rounded-xl text-center hover:opacity-95 transition flex items-center justify-center gap-2 text-sm">
            <i class="fa-brands fa-whatsapp text-lg"></i>
            <span data-i18n="reserveCar">احجز هذه السيارة</span>
          </a>
        </div>
      </div>

    </div>
  </section>

  <!-- Services & Rental Conditions -->
  <section id="services" class="py-16 bg-zinc-950/90 border-y border-white/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid lg:grid-cols-2 gap-10">
        
        <!-- Services Card -->
        <div class="glass-card rounded-3xl p-7 sm:p-9 space-y-6">
          <div class="w-14 h-14 rounded-2xl brand-gradient border border-amber-400/50 flex items-center justify-center text-amber-400 text-2xl">
            <i class="fa-solid fa-plane-arrival"></i>
          </div>
          <h3 class="text-2xl sm:text-3xl font-black text-white" data-i18n="servicesTitle">خدماتنا المميزة</h3>
          <ul class="space-y-4 text-gray-200">
            <li class="flex items-start gap-3">
              <i class="fa-solid fa-circle-check text-amber-400 mt-1"></i>
              <div>
                <strong class="text-white block" data-i18n="srvAirportTitle">التوصيل والاستلام في مطار الناظور العروي</strong>
                <span class="text-sm text-gray-400" data-i18n="srvAirportDesc">نستقبلك فور وصول رحلتك لتسليمك السيارة بسرعة وبدون أي تأخير.</span>
              </div>
            </li>
            <li class="flex items-start gap-3">
              <i class="fa-solid fa-circle-check text-amber-400 mt-1"></i>
              <div>
                <strong class="text-white block" data-i18n="srvGearTitle">خيارات أوتوماتيك ومانيول</strong>
                <span class="text-sm text-gray-400" data-i18n="srvGearDesc">نوفر سيارات بناقل حركة أوتوماتيك أو يدوي حسب راحتك وتفضيلك في السياقة.</span>
              </div>
            </li>
            <li class="flex items-start gap-3">
              <i class="fa-solid fa-circle-check text-amber-400 mt-1"></i>
              <div>
                <strong class="text-white block" data-i18n="srvCleanTitle">سيارات نظيفة ومفحوصة تقنياً</strong>
                <span class="text-sm text-gray-400" data-i18n="srvCleanDesc">صيانة دورية وتعقيم شامل قبل كل عملية كراء لضمان سلامتك التامة.</span>
              </div>
            </li>
          </ul>
        </div>

        <!-- Conditions Card -->
        <div id="conditions" class="glass-card rounded-3xl p-7 sm:p-9 space-y-6 border-red-800/40">
          <div class="w-14 h-14 rounded-2xl brand-gradient border border-amber-400/50 flex items-center justify-center text-amber-400 text-2xl">
            <i class="fa-solid fa-file-signature"></i>
          </div>
          <h3 class="text-2xl sm:text-3xl font-black text-white" data-i18n="condTitle">الوثائق وشروط الحجز</h3>
          <p class="text-sm text-gray-300" data-i18n="condIntro">لإتمام عقد الكراء بسرعة وسهولة، يرجى توفير الوثائق التالية سارية المفعول:</p>
          
          <div class="grid sm:grid-cols-3 gap-4 pt-2">
            <div class="bg-zinc-900/90 border border-amber-500/25 rounded-2xl p-4 text-center space-y-2">
              <i class="fa-solid fa-id-card text-3xl text-amber-400"></i>
              <h4 class="font-bold text-white text-sm" data-i18n="docLicense">رخصة السياقة</h4>
              <p class="text-xs text-gray-400" data-i18n="docLicenseSub">سارية المفعول</p>
            </div>
            <div class="bg-zinc-900/90 border border-amber-500/25 rounded-2xl p-4 text-center space-y-2">
              <i class="fa-solid fa-passport text-3xl text-amber-400"></i>
              <h4 class="font-bold text-white text-sm" data-i18n="docPassport">جواز السفر</h4>
              <p class="text-xs text-gray-400" data-i18n="docPassportSub">ساري المفعول</p>
            </div>
            <div class="bg-zinc-900/90 border border-amber-500/25 rounded-2xl p-4 text-center space-y-2">
              <i class="fa-solid fa-address-card text-3xl text-amber-400"></i>
              <h4 class="font-bold text-white text-sm" data-i18n="docCin">البطاقة الوطنية</h4>
              <p class="text-xs text-gray-400" data-i18n="docCinSub">للمقيمين بالمغرب</p>
            </div>
          </div>

          <div class="bg-red-950/40 border border-red-800/50 rounded-2xl p-4 text-xs sm:text-sm text-amber-200 flex items-center gap-3">
            <i class="fa-solid fa-circle-info text-amber-400 text-lg shrink-0"></i>
            <span data-i18n="condNote">حجز سريع ومباشر بدون تعقيدات عبر الواتساب أو في مقر الوكالة بحي البركة الناظور.</span>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- Instant WhatsApp Booking Section -->
  <section id="booking" class="py-16 sm:py-24 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="glass-card rounded-3xl p-6 sm:p-10 border border-amber-400/30 shadow-2xl">
      <div class="text-center max-w-2xl mx-auto mb-8">
        <span class="text-amber-400 font-bold text-sm uppercase tracking-wider" data-i18n="bookTag">حجز فوري في أقل من دقيقة</span>
        <h2 class="text-3xl sm:text-4xl font-black text-white mt-1" data-i18n="bookTitle">احجز سيارتك الآن</h2>
        <p class="text-gray-400 text-sm mt-2" data-i18n="bookSub">املأ البيانات أسفله وسيتم تحويل طلبك مباشرة إلى واتساب وكالة AZAUAR CAR لتأكيد الحجز.</p>
      </div>

      <form id="bookingForm" class="grid sm:grid-cols-2 gap-5">
        <div>
          <label class="block text-xs font-bold text-gray-300 mb-2" data-i18n="lblName">الاسم الكامل</label>
          <input type="text" id="clientName" required class="w-full bg-zinc-900 border border-white/15 focus:border-amber-400 rounded-xl px-4 py-3 text-white text-sm outline-none" placeholder="مثال: محمد أمين" />
        </div>

        <div>
          <label class="block text-xs font-bold text-gray-300 mb-2" data-i18n="lblCar">اختر السيارة</label>
          <select id="carSelect" class="w-full bg-zinc-900 border border-white/15 focus:border-amber-400 rounded-xl px-4 py-3 text-white text-sm outline-none">
            <option value="Dacia Duster">Dacia Duster</option>
            <option value="Renault Clio">Renault Clio</option>
            <option value="Opel Corsa">Opel Corsa</option>
          </select>
        </div>

        <div>
          <label class="block text-xs font-bold text-gray-300 mb-2" data-i18n="lblGear">ناقل الحركة</label>
          <select id="gearSelect" class="w-full bg-zinc-900 border border-white/15 focus:border-amber-400 rounded-xl px-4 py-3 text-white text-sm outline-none">
            <option value="Automatic" data-i18n="optAuto">أوتوماتيك (Automatic)</option>
            <option value="Manual" data-i18n="optManual">مانيول (Manual)</option>
          </select>
        </div>

        <div>
          <label class="block text-xs font-bold text-gray-300 mb-2" data-i18n="lblPickup">مكان الاستلام</label>
          <select id="pickupSelect" class="w-full bg-zinc-900 border border-white/15 focus:border-amber-400 rounded-xl px-4 py-3 text-white text-sm outline-none">
            <option value="Nador Airport (Aéroport Nador El Aroui)" data-i18n="optAirport">مطار الناظور العروي</option>
            <option value="Agency - Hay Baraka L157, Nador" data-i18n="optAgency">مقر الوكالة - حي البركة L157 الناظور</option>
          </select>
        </div>

        <div>
          <label class="block text-xs font-bold text-gray-300 mb-2" data-i18n="lblStart">تاريخ البداية</label>
          <input type="date" id="startDate" required class="w-full bg-zinc-900 border border-white/15 focus:border-amber-400 rounded-xl px-4 py-3 text-white text-sm outline-none" />
        </div>

        <div>
          <label class="block text-xs font-bold text-gray-300 mb-2" data-i18n="lblEnd">تاريخ الإرجاع</label>
          <input type="date" id="endDate" required class="w-full bg-zinc-900 border border-white/15 focus:border-amber-400 rounded-xl px-4 py-3 text-white text-sm outline-none" />
        </div>

        <div class="sm:col-span-2 pt-2">
          <button type="submit" class="w-full gold-gradient text-black font-black py-4 rounded-xl shadow-lg shadow-amber-500/20 hover:opacity-95 transition flex items-center justify-center gap-3 text-base cursor-pointer">
            <i class="fa-brands fa-whatsapp text-2xl"></i>
            <span data-i18n="btnSendWhatsapp">إرسال طلب الحجز عبر واتساب</span>
          </button>
        </div>
      </form>
    </div>
  </section>

  <!-- Location & Google Map Section -->
  <section id="contact" class="py-16 bg-zinc-950 border-t border-white/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid lg:grid-cols-12 gap-8 items-stretch">
        
        <!-- Contact Details -->
        <div class="lg:col-span-5 glass-card rounded-3xl p-7 sm:p-8 flex flex-col justify-between space-y-6">
          <div class="space-y-4">
            <span class="text-amber-400 font-bold text-xs uppercase tracking-widest" data-i18n="contactTag">تواصل معنا أو تفضل بزيارتنا</span>
            <h2 class="text-3xl font-black text-white">AZAUAR CAR</h2>
            <p class="text-gray-400 text-sm" data-i18n="contactDesc">نحن رهن إشارتكم طيلة أيام الأسبوع لتقديم أفضل خدمات كراء السيارات في الناظور والمطار.</p>
          </div>

          <div class="space-y-4 text-sm">
            <div class="flex items-start gap-3.5 bg-zinc-900/90 p-4 rounded-2xl border border-white/10">
              <i class="fa-solid fa-location-dot text-amber-400 text-xl mt-0.5"></i>
              <div>
                <span class="block text-xs text-gray-400" data-i18n="addrLabel">عنوان الوكالة</span>
                <strong class="text-white text-base">Hay Baraka L157 - Nador, Maroc</strong>
              </div>
            </div>

            <a href="tel:+212668221538" class="flex items-center gap-3.5 bg-zinc-900/90 p-4 rounded-2xl border border-white/10 hover:border-amber-400 transition">
              <i class="fa-solid fa-phone-volume text-amber-400 text-xl"></i>
              <div>
                <span class="block text-xs text-gray-400" data-i18n="phoneLabel">الهاتف والواتساب</span>
                <strong dir="ltr" class="text-white text-base">+212 668-221538</strong>
              </div>
            </a>

            <a href="https://www.instagram.com/azauar_car?xtok=OG8wa244YTBlazFv" target="_blank" rel="noopener noreferrer" class="flex items-center gap-3.5 bg-zinc-900/90 p-4 rounded-2xl border border-white/10 hover:border-amber-400 transition">
              <i class="fa-brands fa-instagram text-amber-400 text-2xl"></i>
              <div>
                <span class="block text-xs text-gray-400">Instagram</span>
                <strong dir="ltr" class="text-white text-base">@azauar_car</strong>
              </div>
            </a>
          </div>

          <a href="https://www.google.com/maps/search/?api=1&query=Hay+Baraka+L157+Nador+Morocco" target="_blank" rel="noopener noreferrer" class="w-full bg-red-900 hover:bg-red-800 border border-amber-400/50 text-white font-bold py-3.5 rounded-xl text-center transition flex items-center justify-center gap-2 text-sm">
            <i class="fa-solid fa-diamond-turn-right text-amber-400"></i>
            <span data-i18n="openMapsBtn">فتح العنوان في Google Maps</span>
          </a>
        </div>

        <!-- Embedded Google Map -->
        <div class="lg:col-span-7 rounded-3xl overflow-hidden border border-amber-500/30 shadow-2xl min-h-[360px] bg-zinc-900 relative">
          <iframe
            title="AZAUAR CAR Location - Hay Baraka L157 Nador"
            src="https://maps.google.com/maps?q=Hay%20Baraka%20Nador%20Morocco&t=&z=15&ie=UTF8&iwloc=&output=embed"
            class="w-full h-full min-h-[360px] border-0"
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade">
          </iframe>
        </div>

      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-black border-t border-white/10 py-8 px-4 text-center text-xs sm:text-sm text-gray-400">
    <div class="max-w-7xl mx-auto flex flex-col sm:flex-row items-center justify-between gap-4">
      <p>© <span id="year"></span> <strong class="text-amber-400">AZAUAR CAR</strong> - Hay Baraka L157, Nador. <span data-i18n="rights">جميع الحقوق محفوظة.</span></p>
      <div class="flex items-center gap-5">
        <a href="https://wa.me/212668221538" target="_blank" rel="noopener noreferrer" class="hover:text-amber-400 transition">WhatsApp</a>
        <a href="https://www.instagram.com/azauar_car?xtok=OG8wa244YTBlazFv" target="_blank" rel="noopener noreferrer" class="hover:text-amber-400 transition">Instagram</a>
      </div>
    </div>
  </footer>

  <!-- Floating WhatsApp Button -->
  <a href="https://wa.me/212668221538" target="_blank" rel="noopener noreferrer" aria-label="WhatsApp" class="fixed bottom-5 end-5 z-50 w-14 h-14 rounded-full bg-emerald-500 hover:bg-emerald-600 text-white flex items-center justify-center shadow-2xl shadow-emerald-900/60 hover:scale-110 transition">
    <i class="fa-brands fa-whatsapp text-3xl"></i>
  </a>

  <script>
    const translations = {
      ar: {
        dir: "rtl",
        airportBadge: "توصيل مجاني لمطار الناظور العروي ✈️",
        logoSub: "كراء السيارات بالناظور",
        navFleet: "أسطول السيارات",
        navServices: "خدماتنا",
        navConditions: "شروط الكراء",
        navBooking: "احجز الآن",
        navContact: "موقعنا",
        heroTag: "الاختيار الأول لكراء السيارات في الناظور والمطار",
        heroTitle: 'انطلق بكل حرية مع <span class="gold-text">AZAUAR CAR</span> في الناظور',
        heroDesc: "نقدم لك أحدث السيارات الاقتصادية والعائلية بناقل حركة أوتوماتيك ومانيول، مع خدمة التوصيل السريع إلى مطار الناظور العروي وأثمنة تنافسية.",
        heroCtaPrimary: "احجز سيارتك عبر واتساب",
        heroCtaSecondary: "استكشف السيارات",
        statSupport: "خدمة متواصلة",
        statAirport: "توصيل للمطار",
        statGear: "أوتوماتيك ومانيول",
        featuredLabel: "أكثر السيارات طلباً",
        availableNow: "متوفرة الآن",
        heroCarSpec: "أوتوماتيك ومانيول • تكييف • اقتصادية",
        bookQuick: "احجز الآن",
        fleetSubtitle: "سيارات حديثة ومجهزة بالكامل",
        fleetTitle: "أسطول سيارات AZAUAR CAR",
        filterAll: "الكل",
        filterAuto: "أوتوماتيك",
        filterManual: "مانيول",
        bothGears: "أوتوماتيك / مانيول",
        dusterDesc: "سيارة قوية ومريحة مثالية للعائلات والسفر الطويل في جميع الطرقات.",
        clioDesc: "تصميم عصري وأنيق مع استهلاك منخفض للوقود وسلاسة عالية في القيادة داخل المدينة.",
        corsaDesc: "سيارة عملية وموثوقة تجمع بين الراحة والأداء الاقتصادي للتنقل اليومي في الناظور.",
        seats5: "5 مقاعد",
        gearShort: "أوتو / مانيول",
        ac: "مكيف",
        reserveCar: "احجز هذه السيارة",
        servicesTitle: "خدماتنا المميزة",
        srvAirportTitle: "التوصيل والاستلام في مطار الناظور العروي",
        srvAirportDesc: "نستقبلك فور وصول رحلتك لتسليمك السيارة بسرعة وبدون أي تأخير.",
        srvGearTitle: "خيارات أوتوماتيك ومانيول",
        srvGearDesc: "نوفر سيارات بناقل حركة أوتوماتيك أو يدوي حسب راحتك وتفضيلك في السياقة.",
        srvCleanTitle: "سيارات نظيفة ومفحوصة تقنياً",
        srvCleanDesc: "صيانة دورية وتعقيم شامل قبل كل عملية كراء لضمان سلامتك التامة.",
        condTitle: "الوثائق وشروط الحجز",
        condIntro: "لإتمام عقد الكراء بسرعة وسهولة، يرجى توفير الوثائق التالية سارية المفعول:",
        docLicense: "رخصة السياقة",
        docLicenseSub: "سارية المفعول",
        docPassport: "جواز السفر",
        docPassportSub: "ساري المفعول",
        docCin: "البطاقة الوطنية",
        docCinSub: "للمقيمين بالمغرب",
        condNote: "حجز سريع ومباشر بدون تعقيدات عبر الواتساب أو في مقر الوكالة بحي البركة الناظور.",
        bookTag: "حجز فوري في أقل من دقيقة",
        bookTitle: "احجز سيارتك الآن",
        bookSub: "املأ البيانات أسفله وسيتم تحويل طلبك مباشرة إلى واتساب وكالة AZAUAR CAR لتأكيد الحجز.",
        lblName: "الاسم الكامل",
        lblCar: "اختر السيارة",
        lblGear: "ناقل الحركة",
        optAuto: "أوتوماتيك (Automatic)",
        optManual: "مانيول (Manual)",
        lblPickup: "مكان الاستلام",
        optAirport: "مطار الناظور العروي",
        optAgency: "مقر الوكالة - حي البركة L157 الناظور",
        lblStart: "تاريخ البداية",
        lblEnd: "تاريخ الإرجاع",
        btnSendWhatsapp: "إرسال طلب الحجز عبر واتساب",
        contactTag: "تواصل معنا أو تفضل بزيارتنا",
        contactDesc: "نحن رهن إشارتكم طيلة أيام الأسبوع لتقديم أفضل خدمات كراء السيارات في الناظور والمطار.",
        addrLabel: "عنوان الوكالة",
        phoneLabel: "الهاتف والواتساب",
        openMapsBtn: "فتح العنوان في Google Maps",
        rights: "جميع الحقوق محفوظة.",
        namePlaceholder: "مثال: محمد أمين",
        waGreeting: "السلام عليكم وكالة AZAUAR CAR، أرغب في حجز سيارة:"
      },
      de: {
        dir: "ltr",
        airportBadge: "Kostenlose Lieferung zum Flughafen Nador El Aroui ✈️",
        logoSub: "Autovermietung in Nador",
        navFleet: "Fahrzeugflotte",
        navServices: "Services",
        navConditions: "Mietbedingungen",
        navBooking: "Jetzt buchen",
        navContact: "Standort",
        heroTag: "Ihre Nr. 1 Autovermietung in Nador & am Flughafen",
        heroTitle: 'Fahren Sie frei mit <span class="gold-text">AZAUAR CAR</span> in Nador',
        heroDesc: "Moderne Kleinwagen und SUVs mit Automatik- oder Schaltgetriebe, schneller Lieferung zum Flughafen Nador El Aroui und fairen Preisen.",
        heroCtaPrimary: "Per WhatsApp buchen",
        heroCtaSecondary: "Fahrzeuge ansehen",
        statSupport: "Service rund um die Uhr",
        statAirport: "Flughafen-Lieferung",
        statGear: "Automatik & Schaltung",
        featuredLabel: "Beliebtestes Modell",
        availableNow: "Sofort verfügbar",
        heroCarSpec: "Automatik & Schaltung • Klimaanlage • Sparsam",
        bookQuick: "Jetzt buchen",
        fleetSubtitle: "Moderne & gepflegte Fahrzeuge",
        fleetTitle: "AZAUAR CAR Fahrzeugflotte",
        filterAll: "Alle",
        filterAuto: "Automatik",
        filterManual: "Schaltgetriebe",
        bothGears: "Automatik / Schaltung",
        dusterDesc: "Robustes und komfortables SUV, ideal für Familien und lange Reisen auf allen Strecken.",
        clioDesc: "Modernes, elegantes Design mit niedrigem Kraftstoffverbrauch und hohem Fahrkomfort.",
        corsaDesc: "Praktisch, zuverlässig und sparsam – perfekt für den täglichen Stadtverkehr in Nador.",
        seats5: "5 Sitze",
        gearShort: "Auto / Schaltung",
        ac: "Klimaanlage",
        reserveCar: "Dieses Auto buchen",
        servicesTitle: "Unsere Premium-Services",
        srvAirportTitle: "Lieferung & Abholung am Flughafen Nador El Aroui",
        srvAirportDesc: "Wir empfangen Sie direkt nach Ihrer Landung für eine schnelle und reibungslose Fahrzeugübergabe.",
        srvGearTitle: "Automatik- und Schaltgetriebe",
        srvGearDesc: "Wählen Sie flexibel zwischen Automatik- oder Schaltgetriebe ganz nach Ihrem Fahrwunsch.",
        srvCleanTitle: "Geprüfte & gepflegte Fahrzeuge",
        srvCleanDesc: "Regelmäßige Wartung und gründliche Reinigung vor jeder Vermietung für Ihre Sicherheit.",
        condTitle: "Erforderliche Dokumente",
        condIntro: "Für eine schnelle Vertragsabwicklung benötigen Sie folgende gültige Dokumente:",
        docLicense: "Führerschein",
        docLicenseSub: "Gültiger Führerschein",
        docPassport: "Reisepass",
        docPassportSub: "Gültiger Reisepass",
        docCin: "Personalausweis (CIN)",
        docCinSub: "Für Einwohner in Marokko",
        condNote: "Schnelle und unkomplizierte Buchung per WhatsApp oder direkt in unserer Agentur in Hay Baraka, Nador.",
        bookTag: "Sofortbuchung in unter einer Minute",
        bookTitle: "Jetzt Fahrzeug reservieren",
        bookSub: "Füllen Sie das Formular aus – Ihre Anfrage wird direkt an WhatsApp von AZAUAR CAR gesendet.",
        lblName: "Vollständiger Name",
        lblCar: "Fahrzeug wählen",
        lblGear: "Getriebe",
        optAuto: "Automatik (Automatic)",
        optManual: "Schaltgetriebe (Manual)",
        lblPickup: "Abholort",
        optAirport: "Flughafen Nador El Aroui",
        optAgency: "Agentur - Hay Baraka L157, Nador",
        lblStart: "Abholdatum",
        lblEnd: "Rückgabedatum",
        btnSendWhatsapp: "Buchungsanfrage per WhatsApp senden",
        contactTag: "Kontaktieren oder besuchen Sie uns",
        contactDesc: "Wir stehen Ihnen die ganze Woche für erstklassige Autovermietung in Nador und am Flughafen zur Verfügung.",
        addrLabel: "Adresse der Agentur",
        phoneLabel: "Telefon & WhatsApp",
        openMapsBtn: "In Google Maps öffnen",
        rights: "Alle Rechte vorbehalten.",
        namePlaceholder: "z.B. Max Mustermann",
        waGreeting: "Hallo AZAUAR CAR, ich möchte ein Auto mieten:"
      },
      es: {
        dir: "ltr",
        airportBadge: "Entrega gratuita en el Aeropuerto de Nador El Aroui ✈️",
        logoSub: "Alquiler de coches en Nador",
        navFleet: "Nuestra Flota",
        navServices: "Servicios",
        navConditions: "Requisitos",
        navBooking: "Reservar",
        navContact: "Ubicación",
        heroTag: "Tu agencia líder de alquiler de coches en Nador y Aeropuerto",
        heroTitle: 'Conduce con total libertad con <span class="gold-text">AZAUAR CAR</span> en Nador',
        heroDesc: "Coches modernos económicos y SUV con cambio automático y manual, entrega rápida en el Aeropuerto de Nador El Aroui y precios competitivos.",
        heroCtaPrimary: "Reservar por WhatsApp",
        heroCtaSecondary: "Ver vehículos",
        statSupport: "Atención continua",
        statAirport: "Entrega en aeropuerto",
        statGear: "Automático y Manual",
        featuredLabel: "Más solicitado",
        availableNow: "Disponible ahora",
        heroCarSpec: "Automático y Manual • Aire Acondicionado • Económico",
        bookQuick: "Reservar",
        fleetSubtitle: "Vehículos modernos y totalmente equipados",
        fleetTitle: "Flota de AZAUAR CAR",
        filterAll: "Todos",
        filterAuto: "Automático",
        filterManual: "Manual",
        bothGears: "Automático / Manual",
        dusterDesc: "SUV potente y cómodo, ideal para familias y viajes largos por todo tipo de carreteras.",
        clioDesc: "Diseño moderno y elegante con bajo consumo de combustible y gran suavidad al conducir.",
        corsaDesc: "Coche práctico, fiable y económico, perfecto para moverse por Nador con total comodidad.",
        seats5: "5 plazas",
        gearShort: "Auto / Manual",
        ac: "Aire acond.",
        reserveCar: "Reservar este coche",
        servicesTitle: "Nuestros Servicios",
        srvAirportTitle: "Entrega y recogida en el Aeropuerto de Nador El Aroui",
        srvAirportDesc: "Te recibimos a la llegada de tu vuelo para entregarte el coche de forma rápida y sin esperas.",
        srvGearTitle: "Cambio Automático y Manual",
        srvGearDesc: "Disponemos de vehículos con caja automática o manual según tu preferencia de conducción.",
        srvCleanTitle: "Coches limpios y revisados",
        srvCleanDesc: "Mantenimiento periódico y desinfección completa antes de cada alquiler para tu seguridad.",
        condTitle: "Documentación y Requisitos",
        condIntro: "Para formalizar el contrato rápidamente, presenta los siguientes documentos en vigor:",
        docLicense: "Carnet de conducir",
        docLicenseSub: "En vigor",
        docPassport: "Pasaporte",
        docPassportSub: "En vigor",
        docCin: "DNI Marroquí (CIN)",
        docCinSub: "Para residentes en Marruecos",
        condNote: "Reserva rápida y sencilla por WhatsApp o en nuestra oficina en Hay Baraka, Nador.",
        bookTag: "Reserva inmediata en menos de un minuto",
        bookTitle: "Reserva tu coche ahora",
        bookSub: "Completa los datos y tu solicitud se enviará directamente al WhatsApp de AZAUAR CAR.",
        lblName: "Nombre completo",
        lblCar: "Elegir vehículo",
        lblGear: "Transmisión",
        optAuto: "Automático (Automatic)",
        optManual: "Manual (Manual)",
        lblPickup: "Lugar de entrega",
        optAirport: "Aeropuerto de Nador El Aroui",
        optAgency: "Oficina - Hay Baraka L157, Nador",
        lblStart: "Fecha de inicio",
        lblEnd: "Fecha de devolución",
        btnSendWhatsapp: "Enviar reserva por WhatsApp",
        contactTag: "Contáctanos o visítanos",
        contactDesc: "Estamos a tu disposición toda la semana para ofrecerte el mejor alquiler de coches en Nador.",
        addrLabel: "Dirección de la agencia",
        phoneLabel: "Teléfono y WhatsApp",
        openMapsBtn: "Abrir en Google Maps",
        rights: "Todos los derechos reservados.",
        namePlaceholder: "Ej: Carlos García",
        waGreeting: "Hola AZAUAR CAR, me gustaría reservar un coche:"
      }
    };

    let currentLang = "ar";

    function applyLanguage(lang) {
      if (!translations[lang]) return;
      currentLang = lang;
      const t = translations[lang];

      document.documentElement.lang = lang;
      document.documentElement.dir = t.dir;

      document.querySelectorAll("[data-i18n]").forEach((el) => {
        const key = el.getAttribute("data-i18n");
        if (t[key]) {
          el.innerHTML = t[key];
        }
      });

      const nameInput = document.getElementById("clientName");
      if (nameInput) nameInput.placeholder = t.namePlaceholder;

      document.querySelectorAll(".lang-btn").forEach((btn) => {
        if (btn.getAttribute("data-lang") === lang) {
          btn.classList.add("active");
          btn.classList.remove("text-gray-300");
        } else {
          btn.classList.remove("active");
          btn.classList.add("text-gray-300");
        }
      });
    }

    // Immediate touch & click response for language switcher
    document.querySelectorAll(".lang-btn").forEach((btn) => {
      const switchHandler = (e) => {
        e.preventDefault();
        const selectedLang = btn.getAttribute("data-lang");
        applyLanguage(selectedLang);
      };
      btn.addEventListener("click", switchHandler);
      btn.addEventListener("touchend", switchHandler, { passive: false });
    });

    // Fleet filter
    function filterFleet(type, clickedBtn) {
      document.querySelectorAll(".filter-btn").forEach((b) => b.classList.remove("active"));
      clickedBtn.classList.add("active");

      document.querySelectorAll(".car-card").forEach((card) => {
        const trans = card.getAttribute("data-transmission");
        if (type === "all" || trans.includes(type)) {
          card.style.display = "flex";
        } else {
          card.style.display = "none";
        }
      });
    }

    // Pre-select car when clicking "Reserve"
    function selectCarForBooking(carName) {
      const select = document.getElementById("carSelect");
      if (select) select.value = carName;
    }

    // Set default dates
    const today = new Date();
    const tomorrow = new Date(today);
    tomorrow.setDate(tomorrow.getDate() + 3);
    document.getElementById("startDate").valueAsDate = today;
    document.getElementById("endDate").valueAsDate = tomorrow;
    document.getElementById("year").textContent = today.getFullYear();

    // Send booking via WhatsApp
    document.getElementById("bookingForm").addEventListener("submit", function (e) {
      e.preventDefault();
      const t = translations[currentLang];
      const name = document.getElementById("clientName").value.trim();
      const car = document.getElementById("carSelect").value;
      const gear = document.getElementById("gearSelect").value;
      const pickup = document.getElementById("pickupSelect").value;
      const start = document.getElementById("startDate").value;
      const end = document.getElementById("endDate").value;

      const message = `${t.waGreeting}\n` +
        `👤 *${t.lblName}:* ${name}\n` +
        `🚗 *${t.lblCar}:* ${car}\n` +
        `⚙️ *${t.lblGear}:* ${gear}\n` +
        `📍 *${t.lblPickup}:* ${pickup}\n` +
        `📅 *${t.lblStart}:* ${start}\n` +
        `📅 *${t.lblEnd}:* ${end}`;

      const whatsappUrl = `https://wa.me/212668221538?text=${encodeURIComponent(message)}`;
      window.open(whatsappUrl, "_blank", "noopener,noreferrer");
    });
  </script>
</body>
</html>
