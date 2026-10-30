<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Danang Car Cheap Travel - Thuê Xe Tự Lái & Du Lịch Đà Nẵng | DVDL Đức Võ</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <!-- Google Fonts: Roboto / Inter chuẩn Flatsome -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc;
            color: #1e293b;
            overflow-x: hidden;
        }
        /* Chuẩn khung Flatsome Container 1200px */
        .flatsome-container {
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
            padding-left: 12px;
            padding-right: 12px;
        }
        /* Tiêu đề Section kiểu Flatsome Title */
        .section-title-container {
            margin-bottom: 1.5rem;
        }
        .section-title-main {
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 2px solid #e2e8f0;
            padding-bottom: 10px;
        }
        .section-title-main h2 {
            position: relative;
            font-weight: 800;
            text-transform: uppercase;
            color: #b91c1c;
            letter-spacing: 0.02em;
        }
        .section-title-main h2::after {
            content: "";
            position: absolute;
            bottom: -12px;
            left: 0;
            width: 100%;
            height: 3px;
            background-color: #dc2626;
        }
        /* Hiệu ứng nút nổi Liên hệ */
        @keyframes pulse-ring {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(220, 38, 38, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 12px rgba(220, 38, 38, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(220, 38, 38, 0); }
        }
        .pulse-btn {
            animation: pulse-ring 2s infinite;
        }
        /* Ẩn thanh cuộn ngang cho danh mục trên điện thoại */
        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <!-- ================= TOP BAR (ĐƠN GIẢN CHUẨN FLATSOME) ================= -->
    <div class="bg-red-800 text-white text-xs sm:text-sm py-2">
        <div class="flatsome-container flex flex-wrap items-center justify-between gap-2">
            <div class="flex items-center gap-4">
                <span><i class="fa-solid fa-location-dot text-yellow-400 mr-1.5"></i>17 Lê Đại, Hòa Cường, Đà Nẵng</span>
                <span class="hidden md:inline text-red-300">|</span>
                <span class="hidden md:inline"><i class="fa-solid fa-clock text-yellow-400 mr-1.5"></i>Phục vụ 24/24 - Giao xe tận nơi</span>
            </div>
            <div class="flex items-center gap-4 ml-auto">
                <a href="https://danangcarcheaptravel.com" class="hover:text-yellow-300 transition hidden sm:inline">
                    <i class="fa-solid fa-globe text-yellow-400 mr-1"></i>danangcarcheaptravel.com
                </a>
                <a href="https://www.facebook.com/danang.car.cheap.travel.2025/" target="_blank" rel="noopener noreferrer" class="hover:text-yellow-300 transition">
                    <i class="fa-brands fa-facebook mr-1"></i>Fanpage
                </a>
                <a href="tel:0905548767" class="font-bold text-yellow-300 hover:underline">
                    <i class="fa-solid fa-phone-volume mr-1"></i>0905.548.767
                </a>
            </div>
        </div>
    </div>

    <!-- ================= HEADER MAIN & NAVIGATION ================= -->
    <header class="bg-white shadow-sm sticky top-0 z-40 border-b border-slate-200">
        <div class="flatsome-container py-2.5 flex items-center justify-between gap-3">
            
            <!-- Nút Menu Mobile -->
            <button id="mobileMenuBtn" class="lg:hidden p-2.5 text-slate-700 hover:text-red-700 border border-slate-200 rounded-lg" aria-label="Mở danh mục">
                <i class="fa-solid fa-bars text-xl"></i>
            </button>

            <!-- LOGO DVDL ĐỨC VÕ (Tích hợp trực tiếp từ ảnh logo gốc & SVG sắc nét) -->
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-14 h-14 sm:w-16 sm:h-16 flex-shrink-0 rounded-full overflow-hidden border-2 border-yellow-500 shadow-md bg-red-800 relative flex items-center justify-center">
                    <img src="logo.jpg" alt="DVDL Đức Võ - Danang Car Cheap Travel" class="w-full h-full object-cover" onerror="this.style.display='none'; document.getElementById('svgLogoFallback').style.display='block';">
                    <!-- SVG tái tạo đúng mẫu Logo DVDL Đức Võ khi xem trực tiếp -->
                    <svg id="svgLogoFallback" style="display:none;" viewBox="0 0 200 200" class="w-full h-full">
                        <defs>
                            <radialGradient id="goldGrad" cx="50%" cy="50%" r="50%">
                                <stop offset="0%" stop-color="#fef08a"/>
                                <stop offset="70%" stop-color="#eab308"/>
                                <stop offset="100%" stop-color="#a16207"/>
                            </radialGradient>
                            <path id="topArc" d="M 22,100 A 78,78 0 1,1 178,100" />
                            <path id="bottomArc" d="M 178,100 A 78,78 0 1,1 22,100" />
                        </defs>
                        <circle cx="100" cy="100" r="98" fill="url(#goldGrad)" stroke="#713f12" stroke-width="3"/>
                        <circle cx="100" cy="100" r="88" fill="#991b1b" stroke="#fde047" stroke-width="2"/>
                        <circle cx="100" cy="100" r="65" fill="#dc2626" stroke="#facc15" stroke-width="2"/>
                        <path d="M 38,110 A 65,65 0 0,0 162,110 Z" fill="#facc15"/>
                        <text fill="#ffffff" font-size="9.5" font-weight="800" text-anchor="middle">
                            <textPath href="#topArc" startOffset="50%">NHẬN HỢP ĐỒNG THAM QUAN - DU LỊCH - CƯỚI HỎI</textPath>
                        </text>
                        <text fill="#fef08a" font-size="9" font-weight="800" text-anchor="middle">
                            <textPath href="#bottomArc" startOffset="50%">ĐƯA ĐÓN SÂN BAY &amp; CÁC TỈNH ★ PHỤC VỤ 24/24 ★</textPath>
                        </text>
                        <text x="100" y="54" text-anchor="middle" fill="#fde047" font-size="11">★★★★★</text>
                        <text x="100" y="74" text-anchor="middle" fill="#ffffff" stroke="#fde047" stroke-width="0.6" font-size="16" font-weight="900">DVDL ĐỨC VÕ</text>
                        <text x="100" y="86" text-anchor="middle" fill="#fef9c3" font-size="7.5" font-weight="700">Uy Tín - An Toàn - Nhanh Chóng</text>
                        <rect x="52" y="92" width="96" height="22" rx="11" fill="#450a0a" stroke="#fde047" stroke-width="1.5"/>
                        <text x="100" y="107" text-anchor="middle" fill="#fde047" font-size="13" font-weight="900">0905548767</text>
                        <text x="100" y="142" text-anchor="middle" font-size="22">🚘🚐🚌</text>
                    </svg>
                </div>
                <div>
                    <div class="text-base sm:text-xl font-extrabold text-red-700 tracking-tight leading-tight uppercase">
                        DANANG CAR CHEAP TRAVEL
                    </div>
                    <div class="text-xs sm:text-sm font-semibold text-slate-600">
                        DVDL ĐỨC VÕ • <span class="text-amber-600">danangcarcheaptravel.com</span>
                    </div>
                </div>
            </a>

            <!-- MENU DESKTOP -->
            <nav class="hidden lg:flex items-center gap-1 xl:gap-2 font-semibold text-sm text-slate-700">
                <a href="#trang-chu" class="px-3 py-2 rounded-lg text-red-700 bg-red-50">TRANG CHỦ</a>
                <a href="#xe-4-cho" class="px-3 py-2 rounded-lg hover:text-red-700 hover:bg-slate-100 transition">XE TỰ LÁI 4 CHỖ</a>
                <a href="#xe-7-cho" class="px-3 py-2 rounded-lg hover:text-red-700 hover:bg-slate-100 transition">XE TỰ LÁI 7 CHỖ</a>
                <a href="#xe-ban-tai" class="px-3 py-2 rounded-lg hover:text-red-700 hover:bg-slate-100 transition">XE BÁN TẢI</a>
                <a href="#xe-du-lich" class="px-3 py-2 rounded-lg hover:text-red-700 hover:bg-slate-100 transition">XE CÓ TÀI 4-7-16 CHỖ</a>
                <a href="#thu-tuc" class="px-3 py-2 rounded-lg hover:text-red-700 hover:bg-slate-100 transition">THỦ TỤC THUÊ XE</a>
                <a href="#ban-do" class="px-3 py-2 rounded-lg hover:text-red-700 hover:bg-slate-100 transition">BẢN ĐỒ & LIÊN HỆ</a>
            </nav>

            <!-- NÚT HOTLINE HEADER -->
            <div class="flex items-center gap-2">
                <a href="tel:0905548767" class="bg-red-700 hover:bg-red-800 text-white font-bold px-3.5 py-2.5 rounded-lg text-xs sm:text-sm flex items-center gap-2 shadow-sm transition">
                    <i class="fa-solid fa-phone-volume text-yellow-300"></i>
                    <div class="text-left leading-tight">
                        <span class="block text-[10px] font-normal text-red-100 hidden sm:block">Đặt xe 24/24</span>
                        <span>0905.548.767</span>
                    </div>
                </a>
            </div>
        </div>

        <!-- THANH DANH MỤC NHANH TRÊN ĐIỆN THOẠI & MÁY TÍNH (Tối ưu hiển thị đẹp, dễ bấm) -->
        <div class="bg-slate-100 border-t border-slate-200 py-2">
            <div class="flatsome-container flex items-center gap-2 overflow-x-auto no-scrollbar">
                <a href="#xe-4-cho" class="flex-shrink-0 flex items-center gap-1.5 bg-white border border-slate-300 hover:border-red-600 hover:text-red-700 px-3 py-1.5 rounded-lg text-xs sm:text-sm font-semibold text-slate-700 transition">
                    <i class="fa-solid fa-car text-red-600"></i> Thuê Xe 4 Chỗ
                </a>
                <a href="#xe-7-cho" class="flex-shrink-0 flex items-center gap-1.5 bg-white border border-slate-300 hover:border-red-600 hover:text-red-700 px-3 py-1.5 rounded-lg text-xs sm:text-sm font-semibold text-slate-700 transition">
                    <i class="fa-solid fa-van-shuttle text-red-600"></i> Thuê Xe 7 Chỗ
                </a>
                <a href="#xe-ban-tai" class="flex-shrink-0 flex items-center gap-1.5 bg-white border border-slate-300 hover:border-red-600 hover:text-red-700 px-3 py-1.5 rounded-lg text-xs sm:text-sm font-semibold text-slate-700 transition">
                    <i class="fa-solid fa-truck-pickup text-red-600"></i> Thuê Xe Bán Tải
                </a>
                <a href="#xe-du-lich" class="flex-shrink-0 flex items-center gap-1.5 bg-white border border-slate-300 hover:border-red-600 hover:text-red-700 px-3 py-1.5 rounded-lg text-xs sm:text-sm font-semibold text-slate-700 transition">
                    <i class="fa-solid fa-bus text-red-600"></i> Xe Hợp Đồng 4-7-16 Chỗ
                </a>
                <a href="#xe-du-lich" class="flex-shrink-0 flex items-center gap-1.5 bg-white border border-slate-300 hover:border-red-600 hover:text-red-700 px-3 py-1.5 rounded-lg text-xs sm:text-sm font-semibold text-slate-700 transition">
                    <i class="fa-solid fa-plane-arrival text-red-600"></i> Đưa Đón Sân Bay
                </a>
                <a href="#xe-du-lich" class="flex-shrink-0 flex items-center gap-1.5 bg-white border border-slate-300 hover:border-red-600 hover:text-red-700 px-3 py-1.5 rounded-lg text-xs sm:text-sm font-semibold text-slate-700 transition">
                    <i class="fa-solid fa-heart text-red-600"></i> Xe Cưới Hỏi
                </a>
            </div>
        </div>

        <!-- MENU DRAWER MOBILE -->
        <div id="mobileMenuDrawer" class="hidden lg:hidden bg-white border-t border-slate-200 px-4 py-3 space-y-2 shadow-lg">
            <a href="#trang-chu" class="block py-2 px-3 rounded-lg font-semibold text-red-700 bg-red-50">Trang Chủ</a>
            <a href="#xe-4-cho" class="block py-2 px-3 rounded-lg font-semibold text-slate-700 hover:bg-slate-100">Thuê Xe Tự Lái 4 Chỗ</a>
            <a href="#xe-7-cho" class="block py-2 px-3 rounded-lg font-semibold text-slate-700 hover:bg-slate-100">Thuê Xe Tự Lái 7 Chỗ</a>
            <a href="#xe-ban-tai" class="block py-2 px-3 rounded-lg font-semibold text-slate-700 hover:bg-slate-100">Thuê Xe Tự Lái Bán Tải</a>
            <a href="#xe-du-lich" class="block py-2 px-3 rounded-lg font-semibold text-slate-700 hover:bg-slate-100">Xe Du Lịch Có Tài 4 - 7 - 16 Chỗ & Sân Bay</a>
            <a href="#thu-tuc" class="block py-2 px-3 rounded-lg font-semibold text-slate-700 hover:bg-slate-100">Quy Trình & Thủ Tục Thuê Xe</a>
            <a href="#ban-do" class="block py-2 px-3 rounded-lg font-semibold text-slate-700 hover:bg-slate-100">Bản Đồ & Liên Hệ (17 Lê Đại)</a>
        </div>
    </header>

    <!-- ================= SLIDER 2 ẢNH BANNER TỰ TRƯỢT (FLATSOME SLIDER) ================= -->
    <section id="trang-chu" class="relative bg-slate-900 overflow-hidden">
        <div class="relative h-[280px] sm:h-[380px] md:h-[460px] w-full" id="bannerSlider">
            
            <!-- BANNER 1: THUÊ XE TỰ LÁI & DU LỊCH ĐÀ NẴNG -->
            <div class="banner-slide absolute inset-0 transition-opacity duration-700 opacity-100 z-10">
                <img src="https://images.unsplash.com/photo-1549399542-7e3f8b79c341?auto=format&fit=crop&w=1600&q=80" 
                     alt="Danang Car Cheap Travel Banner 1" 
                     class="w-full h-full object-cover object-center opacity-45"
                     onerror="this.src='https://placehold.co/1600x600/7f1d1d/fef08a?text=DANANG+CAR+CHEAP+TRAVEL'">
                <div class="absolute inset-0 bg-gradient-to-r from-red-950/90 via-red-900/70 to-transparent"></div>
                <div class="flatsome-container h-full flex items-center relative z-20">
                    <div class="max-w-2xl text-white space-y-3 sm:space-y-4">
                        <div class="text-yellow-400 font-bold text-xs sm:text-base uppercase tracking-wider">
                            DVDL ĐỨC VÕ - DANANGCARCHEAPTRAVEL.COM
                        </div>
                        <h1 class="text-2xl sm:text-4xl md:text-5xl font-extrabold leading-tight">
                            THUÊ XE TỰ LÁI & CÓ TÀI <br>
                            <span class="text-yellow-400">4 - 7 - 16 CHỖ ĐÀ NẴNG</span>
                        </h1>
                        <p class="text-xs sm:text-base text-slate-200 leading-relaxed">
                            Xe đời mới 2022 - 2025 sạch sẽ, giao xe tận nơi miễn phí tại Sân bay & Khách sạn Đà Nẵng. Thủ tục nhanh gọn trong 5 phút, phục vụ uy tín 24/24.
                        </p>
                        <div class="pt-1 flex flex-wrap gap-3">
                            <a href="tel:0905548767" class="bg-yellow-500 hover:bg-yellow-400 text-slate-950 font-extrabold px-5 py-2.5 sm:px-6 sm:py-3 rounded-lg text-xs sm:text-sm transition shadow">
                                <i class="fa-solid fa-phone mr-1.5"></i>GỌI NGAY: 0905.548.767
                            </a>
                            <a href="https://zalo.me/0905548767" target="_blank" rel="noopener noreferrer" class="bg-white/15 hover:bg-white/25 text-white border border-white/40 font-bold px-5 py-2.5 sm:px-6 sm:py-3 rounded-lg text-xs sm:text-sm transition">
                                <i class="fa-solid fa-comment-dots mr-1.5"></i>TƯ VẤN QUA ZALO
                            </a>
                        </div>
                    </div>
                </div>
            </div>

            <!-- BANNER 2: HỢP ĐỒNG THAM QUAN - CƯỚI HỎI - SÂN BAY 24/24 -->
            <div class="banner-slide absolute inset-0 transition-opacity duration-700 opacity-0 z-0">
                <img src="https://images.unsplash.com/photo-1503376780353-7e6692767b70?auto=format&fit=crop&w=1600&q=80" 
                     alt="Danang Car Cheap Travel Banner 2" 
                     class="w-full h-full object-cover object-center opacity-45"
                     onerror="this.src='https://placehold.co/1600x600/1e293b/fef08a?text=DVDL+DUC+VO+0905548767'">
                <div class="absolute inset-0 bg-gradient-to-r from-slate-950/90 via-red-950/75 to-transparent"></div>
                <div class="flatsome-container h-full flex items-center relative z-20">
                    <div class="max-w-2xl text-white space-y-3 sm:space-y-4">
                        <div class="text-yellow-400 font-bold text-xs sm:text-base uppercase tracking-wider">
                            UY TÍN - AN TOÀN - NHANH CHÓNG • PHỤC VỤ 24/24
                        </div>
                        <h2 class="text-2xl sm:text-4xl md:text-5xl font-extrabold leading-tight">
                            NHẬN HỢP ĐỒNG THAM QUAN <br>
                            <span class="text-yellow-400">DU LỊCH - CƯỚI HỎI - SÂN BAY</span>
                        </h2>
                        <p class="text-xs sm:text-base text-slate-200 leading-relaxed">
                            Chuyên tuyến Đà Nẵng - Hội An - Bà Nà Hills - Huế & đi các tỉnh. Địa chỉ: 17 Lê Đại, Hòa Cường, Đà Nẵng. Cam kết giá rẻ, không phát sinh chi phí ẩn.
                        </p>
                        <div class="pt-1 flex flex-wrap gap-3">
                            <a href="tel:0905548767" class="bg-red-600 hover:bg-red-500 text-white font-extrabold px-5 py-2.5 sm:px-6 sm:py-3 rounded-lg text-xs sm:text-sm transition shadow">
                                <i class="fa-solid fa-car-side mr-1.5"></i>ĐẶT XE: 0905.548.767
                            </a>
                            <a href="#ban-do" class="bg-yellow-500 hover:bg-yellow-400 text-slate-950 font-bold px-5 py-2.5 sm:px-6 sm:py-3 rounded-lg text-xs sm:text-sm transition">
                                <i class="fa-solid fa-location-dot mr-1.5"></i>XEM BẢN ĐỒ 17 LÊ ĐẠI
                            </a>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Nút điều hướng Slider -->
            <button onclick="changeSlide(-1)" class="absolute left-3 top-1/2 -translate-y-1/2 z-30 w-9 h-9 sm:w-11 sm:h-11 rounded-full bg-black/40 hover:bg-red-700 text-white flex items-center justify-center transition" aria-label="Slide trước">
                <i class="fa-solid fa-chevron-left"></i>
            </button>
            <button onclick="changeSlide(1)" class="absolute right-3 top-1/2 -translate-y-1/2 z-30 w-9 h-9 sm:w-11 sm:h-11 rounded-full bg-black/40 hover:bg-red-700 text-white flex items-center justify-center transition" aria-label="Slide tiếp">
                <i class="fa-solid fa-chevron-right"></i>
            </button>

            <!-- Dots chỉ báo Slide -->
            <div class="absolute bottom-3 left-1/2 -translate-x-1/2 z-30 flex gap-2">
                <button onclick="goToSlide(0)" class="slide-dot w-8 h-2.5 rounded-full bg-yellow-400 transition-all" aria-label="Banner 1"></button>
                <button onclick="goToSlide(1)" class="slide-dot w-2.5 h-2.5 rounded-full bg-white/60 transition-all" aria-label="Banner 2"></button>
            </div>
        </div>
    </section>

    <!-- ================= DANH MỤC SẢN PHẨM & DỊCH VỤ (CHUẨN ĐẸP TRÊN PC & MOBILE) ================= -->
    <section class="py-8 bg-white border-b border-slate-200">
        <div class="flatsome-container">
            <div class="section-title-container">
                <div class="section-title-main">
                    <h2 class="text-lg sm:text-xl">DANH MỤC DỊCH VỤ THUÊ XE</h2>
                    <span class="text-xs sm:text-sm text-slate-500 hidden sm:inline">Chọn danh mục xe phù hợp với hành trình của bạn</span>
                </div>
            </div>

            <!-- Chia 2 cột trên điện thoại, 5 cột trên máy tính -->
            <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 gap-3 sm:gap-4">
                <a href="#xe-4-cho" class="group bg-slate-50 hover:bg-red-50 border border-slate-200 hover:border-red-500 rounded-xl p-4 text-center transition flex flex-col items-center">
                    <div class="w-12 h-12 rounded-full bg-red-100 text-red-700 flex items-center justify-center text-xl mb-2.5 group-hover:bg-red-700 group-hover:text-white transition">
                        <i class="fa-solid fa-car"></i>
                    </div>
                    <h3 class="font-bold text-slate-800 group-hover:text-red-700 text-sm sm:text-base">Xe Tự Lái 4 Chỗ</h3>
                    <p class="text-xs text-slate-500 mt-1">Chỉ từ 500.000đ/ngày</p>
                </a>

                <a href="#xe-7-cho" class="group bg-slate-50 hover:bg-red-50 border border-slate-200 hover:border-red-500 rounded-xl p-4 text-center transition flex flex-col items-center">
                    <div class="w-12 h-12 rounded-full bg-red-100 text-red-700 flex items-center justify-center text-xl mb-2.5 group-hover:bg-red-700 group-hover:text-white transition">
                        <i class="fa-solid fa-van-shuttle"></i>
                    </div>
                    <h3 class="font-bold text-slate-800 group-hover:text-red-700 text-sm sm:text-base">Xe Tự Lái 7 Chỗ</h3>
                    <p class="text-xs text-slate-500 mt-1">Chỉ từ 700.000đ/ngày</p>
                </a>

                <a href="#xe-ban-tai" class="group bg-slate-50 hover:bg-red-50 border border-slate-200 hover:border-red-500 rounded-xl p-4 text-center transition flex flex-col items-center">
                    <div class="w-12 h-12 rounded-full bg-red-100 text-red-700 flex items-center justify-center text-xl mb-2.5 group-hover:bg-red-700 group-hover:text-white transition">
                        <i class="fa-solid fa-truck-pickup"></i>
                    </div>
                    <h3 class="font-bold text-slate-800 group-hover:text-red-700 text-sm sm:text-base">Xe Tự Lái Bán Tải</h3>
                    <p class="text-xs text-slate-500 mt-1">Mạnh mẽ, đa địa hình</p>
                </a>

                <a href="#xe-du-lich" class="group bg-slate-50 hover:bg-red-50 border border-slate-200 hover:border-red-500 rounded-xl p-4 text-center transition flex flex-col items-center">
                    <div class="w-12 h-12 rounded-full bg-red-100 text-red-700 flex items-center justify-center text-xl mb-2.5 group-hover:bg-red-700 group-hover:text-white transition">
                        <i class="fa-solid fa-bus"></i>
                    </div>
                    <h3 class="font-bold text-slate-800 group-hover:text-red-700 text-sm sm:text-base">Xe Có Tài 4-7-16 Chỗ</h3>
                    <p class="text-xs text-slate-500 mt-1">Tham quan, Du lịch, Tỉnh</p>
                </a>

                <a href="#xe-du-lich" class="col-span-2 sm:col-span-1 group bg-slate-50 hover:bg-red-50 border border-slate-200 hover:border-red-500 rounded-xl p-4 text-center transition flex flex-col items-center">
                    <div class="w-12 h-12 rounded-full bg-red-100 text-red-700 flex items-center justify-center text-xl mb-2.5 group-hover:bg-red-700 group-hover:text-white transition">
                        <i class="fa-solid fa-plane-departure"></i>
                    </div>
                    <h3 class="font-bold text-slate-800 group-hover:text-red-700 text-sm sm:text-base">Sân Bay & Xe Cưới Hỏi</h3>
                    <p class="text-xs text-slate-500 mt-1">Đưa đón tận nơi 24/24</p>
                </a>
            </div>
        </div>
    </section>

    <!-- ================= DANH MỤC 1: THUÊ XE TỰ LÁI 4 CHỖ (2 CỘT MOBILE, 4 CỘT PC) ================= -->
    <section id="xe-4-cho" class="py-8 sm:py-10">
        <div class="flatsome-container">
            <div class="section-title-container">
                <div class="section-title-main">
                    <h2 class="text-base sm:text-xl">THUÊ XE TỰ LÁI 4 CHỖ ĐÀ NẴNG</h2>
                    <a href="tel:0905548767" class="text-xs sm:text-sm font-semibold text-red-700 hover:underline">
                        Gọi tư vấn: 0905.548.767 <i class="fa-solid fa-angle-right ml-1"></i>
                    </a>
                </div>
            </div>

            <!-- Grid 2 cột trên điện thoại (grid-cols-2), 4 cột trên máy tính (lg:grid-cols-4), không nhãn dán -->
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-5" id="grid-4-cho"></div>
        </div>
    </section>

    <!-- ================= DANH MỤC 2: THUÊ XE TỰ LÁI 7 CHỖ (2 CỘT MOBILE, 4 CỘT PC) ================= -->
    <section id="xe-7-cho" class="py-8 sm:py-10 bg-white border-y border-slate-200">
        <div class="flatsome-container">
            <div class="section-title-container">
                <div class="section-title-main">
                    <h2 class="text-base sm:text-xl">THUÊ XE TỰ LÁI 7 CHỖ &amp; CUV/SUV</h2>
                    <a href="tel:0905548767" class="text-xs sm:text-sm font-semibold text-red-700 hover:underline">
                        Gọi tư vấn: 0905.548.767 <i class="fa-solid fa-angle-right ml-1"></i>
                    </a>
                </div>
            </div>

            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-5" id="grid-7-cho"></div>
        </div>
    </section>

    <!-- ================= DANH MỤC 3: THUÊ XE TỰ LÁI BÁN TẢI (2 CỘT MOBILE, 4 CỘT PC) ================= -->
    <section id="xe-ban-tai" class="py-8 sm:py-10">
        <div class="flatsome-container">
            <div class="section-title-container">
                <div class="section-title-main">
                    <h2 class="text-base sm:text-xl">THUÊ XE TỰ LÁI BÁN TẢI</h2>
                    <a href="tel:0905548767" class="text-xs sm:text-sm font-semibold text-red-700 hover:underline">
                        Gọi tư vấn: 0905.548.767 <i class="fa-solid fa-angle-right ml-1"></i>
                    </a>
                </div>
            </div>

            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-5" id="grid-ban-tai"></div>
        </div>
    </section>

    <!-- ================= DANH MỤC 4: HỢP ĐỒNG DU LỊCH CÓ TÀI 4-7-16 CHỖ & CƯỚI HỎI ================= -->
    <section id="xe-du-lich" class="py-8 sm:py-10 bg-white border-y border-slate-200">
        <div class="flatsome-container">
            <div class="section-title-container">
                <div class="section-title-main">
                    <h2 class="text-base sm:text-xl">XE HỢP ĐỒNG THAM QUAN - DU LỊCH - CƯỚI HỎI - SÂN BAY</h2>
                    <a href="tel:0905548767" class="text-xs sm:text-sm font-semibold text-red-700 hover:underline">
                        Phục vụ 24/24 <i class="fa-solid fa-angle-right ml-1"></i>
                    </a>
                </div>
            </div>

            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-5" id="grid-du-lich"></div>
        </div>
    </section>

    <!-- ================= QUY TRÌNH & THỦ TỤC THUÊ XE (MẪU TOÀN CẦU VÀNG) ================= -->
    <section id="thu-tuc" class="py-8 sm:py-10">
        <div class="flatsome-container">
            <div class="section-title-container">
                <div class="section-title-main">
                    <h2 class="text-base sm:text-xl">QUY TRÌNH &amp; THỦ TỤC THUÊ XE ĐÀ NẴNG</h2>
                </div>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
                <div class="bg-white p-5 rounded-xl border border-slate-200">
                    <div class="w-10 h-10 rounded-lg bg-red-700 text-white font-bold flex items-center justify-center mb-3">1</div>
                    <h3 class="font-bold text-slate-800 text-base mb-1.5">Chuẩn bị giấy tờ</h3>
                    <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                        Chỉ cần CCCD gắn chip (hoặc Passport) và Giấy phép lái xe hạng B1 trở lên hợp lệ.
                    </p>
                </div>
                <div class="bg-white p-5 rounded-xl border border-slate-200">
                    <div class="w-10 h-10 rounded-lg bg-red-700 text-white font-bold flex items-center justify-center mb-3">2</div>
                    <h3 class="font-bold text-slate-800 text-base mb-1.5">Chọn xe &amp; Lịch trình</h3>
                    <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                        Liên hệ Hotline/Zalo <strong>0905.548.767</strong> để chọn dòng xe 4-7-16 chỗ và thời gian nhận xe.
                    </p>
                </div>
                <div class="bg-white p-5 rounded-xl border border-slate-200">
                    <div class="w-10 h-10 rounded-lg bg-red-700 text-white font-bold flex items-center justify-center mb-3">3</div>
                    <h3 class="font-bold text-slate-800 text-base mb-1.5">Ký hợp đồng &amp; Nhận xe</h3>
                    <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                        Nhận xe tại <strong>17 Lê Đại, Hòa Cường</strong> hoặc giao xe tận nơi tại Sân bay, Khách sạn Đà Nẵng.
                    </p>
                </div>
                <div class="bg-white p-5 rounded-xl border border-slate-200">
                    <div class="w-10 h-10 rounded-lg bg-red-700 text-white font-bold flex items-center justify-center mb-3">4</div>
                    <h3 class="font-bold text-slate-800 text-base mb-1.5">Trả xe &amp; Thanh toán</h3>
                    <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                        Nhân viên hỗ trợ nhận lại xe nhanh gọn, minh bạch, hỗ trợ kỹ thuật xuyên suốt 24/24.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= ĐƯA ẢNH MAP & BẢN ĐỒ RA NGOÀI TRANG CHỦ ================= -->
    <section id="ban-do" class="py-8 sm:py-10 bg-white border-t border-slate-200">
        <div class="flatsome-container">
            <div class="section-title-container">
                <div class="section-title-main">
                    <h2 class="text-base sm:text-xl">ĐỊA CHỈ &amp; BẢN ĐỒ ĐƯỜNG ĐI</h2>
                    <a href="https://maps.app.goo.gl/DW8HgefYWRvuhmQ29" target="_blank" rel="noopener noreferrer" class="text-xs sm:text-sm font-bold text-red-700 hover:underline">
                        <i class="fa-solid fa-map-location-dot mr-1"></i>Mở Google Maps chỉ đường
                    </a>
                </div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-stretch">
                <!-- Cột Thông tin & Ảnh Sơ Đồ Bản Đồ Trực Quan -->
                <div class="lg:col-span-5 bg-slate-50 border border-slate-200 rounded-xl p-5 flex flex-col justify-between space-y-4">
                    <div class="space-y-3">
                        <h3 class="text-lg font-extrabold text-red-700 uppercase">
                            DANANG CAR CHEAP TRAVEL - DVDL ĐỨC VÕ
                        </h3>
                        <p class="text-sm text-slate-600">
                            Chuyên cho thuê xe tự lái 4 - 7 chỗ, bán tải và nhận hợp đồng xe du lịch 4 - 7 - 16 chỗ tham quan, cưới hỏi, đưa đón sân bay &amp; đi các tỉnh phục vụ 24/24.
                        </p>
                        <div class="space-y-2 text-sm text-slate-700 pt-1">
                            <p class="flex items-start gap-2.5">
                                <i class="fa-solid fa-location-dot text-red-600 mt-1 w-4 text-center"></i>
                                <span><strong>Địa chỉ:</strong> 17 Lê Đại, Phường Hòa Cường, TP. Đà Nẵng</span>
                            </p>
                            <p class="flex items-center gap-2.5">
                                <i class="fa-solid fa-phone-volume text-red-600 w-4 text-center"></i>
                                <span><strong>Hotline/Zalo:</strong> <a href="tel:0905548767" class="text-red-700 font-bold hover:underline">0905.548.767</a></span>
                            </p>
                            <p class="flex items-center gap-2.5">
                                <i class="fa-solid fa-globe text-red-600 w-4 text-center"></i>
                                <span><strong>Website:</strong> <a href="https://danangcarcheaptravel.com" class="text-blue-600 hover:underline">danangcarcheaptravel.com</a></span>
                            </p>
                            <p class="flex items-center gap-2.5">
                                <i class="fa-brands fa-facebook text-red-600 w-4 text-center"></i>
                                <span><strong>Fanpage:</strong> <a href="https://www.facebook.com/danang.car.cheap.travel.2025/" target="_blank" rel="noopener noreferrer" class="text-blue-600 hover:underline">fb.com/danang.car.cheap.travel.2025</a></span>
                            </p>
                        </div>
                    </div>

                    <!-- Hình ảnh Map trực quan ngoài trang chủ (Click mở trực tiếp link Google Maps) -->
                    <a href="https://maps.app.goo.gl/DW8HgefYWRvuhmQ29" target="_blank" rel="noopener noreferrer" class="block group relative rounded-xl overflow-hidden border-2 border-red-200 hover:border-red-600 transition shadow-sm">
                        <svg viewBox="0 0 600 240" class="w-full h-auto block bg-slate-100">
                            <!-- Nền bản đồ đường phố Hòa Cường, Đà Nẵng -->
                            <rect width="600" height="240" fill="#e2e8f0"/>
                            <path d="M 0,50 L 600,50 M 0,120 L 600,120 M 0,190 L 600,190 M 120,0 L 120,240 M 300,0 L 300,240 M 470,0 L 470,240" stroke="#ffffff" stroke-width="14"/>
                            <path d="M 0,120 L 600,120 M 300,0 L 300,240" stroke="#fde047" stroke-width="4" stroke-dasharray="10,6"/>
                            <rect x="135" y="62" width="150" height="45" rx="6" fill="#cbd5e1"/>
                            <rect x="315" y="132" width="140" height="45" rx="6" fill="#bbf7d0"/>
                            <text x="210" y="114" font-size="11" font-weight="700" fill="#475569">Đường Lê Đại - Hòa Cường</text>
                            <!-- Điểm ghim 17 Lê Đại -->
                            <circle cx="300" cy="120" r="26" fill="rgba(220,38,38,0.2)"/>
                            <circle cx="300" cy="120" r="9" fill="#dc2626" stroke="#ffffff" stroke-width="3"/>
                            <path d="M 300,112 C 286,92 282,74 300,62 C 318,74 314,92 300,112 Z" fill="#dc2626"/>
                            <circle cx="300" cy="80" r="5" fill="#fef08a"/>
                            <!-- Hộp thông tin ghim -->
                            <rect x="160" y="14" width="280" height="40" rx="8" fill="#991b1b"/>
                            <text x="300" y="32" text-anchor="middle" fill="#fef08a" font-size="12" font-weight="800">17 LÊ ĐẠI, HÒA CƯỜNG, ĐÀ NẴNG</text>
                            <text x="300" y="47" text-anchor="middle" fill="#ffffff" font-size="10">Nhấn để mở ứng dụng Google Maps chỉ đường</text>
                        </svg>
                        <div class="bg-red-700 text-white text-center py-2 text-xs sm:text-sm font-bold group-hover:bg-red-800 transition">
                            <i class="fa-solid fa-diamond-turn-right mr-1.5"></i>XEM TRÊN GOOGLE MAPS (17 LÊ ĐẠI, HÒA CƯỜNG)
                        </div>
                    </a>
                </div>

                <!-- Cột Google Maps Iframe trực tiếp ngoài trang chủ -->
                <div class="lg:col-span-7 rounded-xl overflow-hidden border border-slate-200 shadow-sm min-h-[320px] sm:min-h-[400px] relative bg-slate-100">
                    <iframe 
                        title="Bản đồ 17 Lê Đại, Hòa Cường, Đà Nẵng"
                        src="https://www.google.com/maps?q=17+L%C3%AA+%C4%90%E1%BA%A1i,+H%C3%B2a+C%C6%B0%E1%BB%9Dng,+%C4%90%C3%A0+N%E1%BA%B5ng&output=embed" 
                        class="w-full h-full min-h-[320px] sm:min-h-[400px] border-0" 
                        allowfullscreen="" 
                        loading="lazy" 
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= FOOTER (CHUẨN FLATSOME) ================= -->
    <footer class="bg-slate-900 text-slate-300 pt-10 pb-24 sm:pb-10 mt-auto">
        <div class="flatsome-container grid grid-cols-1 md:grid-cols-3 gap-8 pb-8 border-b border-slate-800">
            <div>
                <h3 class="text-white font-extrabold text-base uppercase mb-3">
                    DANANG CAR CHEAP TRAVEL - DVDL ĐỨC VÕ
                </h3>
                <p class="text-sm text-slate-400 leading-relaxed mb-3">
                    Đơn vị uy tín chuyên cho thuê xe tự lái 4 - 7 chỗ, xe bán tải và nhận hợp đồng tham quan, du lịch, cưới hỏi, đưa đón sân bay và đi các tỉnh phục vụ 24/24 tại Đà Nẵng.
                </p>
                <p class="text-xs text-yellow-400 font-semibold">
                    Uy Tín - An Toàn - Nhanh Chóng - Phục Vụ 24/24
                </p>
            </div>

            <div>
                <h3 class="text-white font-extrabold text-base uppercase mb-3">
                    DANH MỤC DỊCH VỤ
                </h3>
                <ul class="space-y-2 text-sm">
                    <li><a href="#xe-4-cho" class="hover:text-yellow-400 transition"><i class="fa-solid fa-angle-right mr-2 text-red-500"></i>Thuê Xe Tự Lái 4 Chỗ Đà Nẵng</a></li>
                    <li><a href="#xe-7-cho" class="hover:text-yellow-400 transition"><i class="fa-solid fa-angle-right mr-2 text-red-500"></i>Thuê Xe Tự Lái 7 Chỗ Đà Nẵng</a></li>
                    <li><a href="#xe-ban-tai" class="hover:text-yellow-400 transition"><i class="fa-solid fa-angle-right mr-2 text-red-500"></i>Thuê Xe Tự Lái Bán Tải</a></li>
                    <li><a href="#xe-du-lich" class="hover:text-yellow-400 transition"><i class="fa-solid fa-angle-right mr-2 text-red-500"></i>Hợp Đồng Xe Du Lịch 4 - 7 - 16 Chỗ</a></li>
                    <li><a href="#xe-du-lich" class="hover:text-yellow-400 transition"><i class="fa-solid fa-angle-right mr-2 text-red-500"></i>Xe Cưới Hỏi &amp; Đưa Đón Sân Bay 24/24</a></li>
                </ul>
            </div>

            <div>
                <h3 class="text-white font-extrabold text-base uppercase mb-3">
                    THÔNG TIN LIÊN HỆ
                </h3>
                <ul class="space-y-2.5 text-sm">
                    <li><i class="fa-solid fa-location-dot text-red-500 mr-2"></i>Địa chỉ: 17 Lê Đại, Hòa Cường, Đà Nẵng</li>
                    <li><i class="fa-solid fa-phone text-red-500 mr-2"></i>Hotline/Zalo: <a href="tel:0905548767" class="text-yellow-400 font-bold">0905.548.767</a></li>
                    <li><i class="fa-solid fa-globe text-red-500 mr-2"></i>Website: <a href="https://danangcarcheaptravel.com" class="hover:text-white">danangcarcheaptravel.com</a></li>
                    <li><i class="fa-brands fa-facebook text-red-500 mr-2"></i>Fanpage: <a href="https://www.facebook.com/danang.car.cheap.travel.2025/" target="_blank" rel="noopener noreferrer" class="hover:text-white">Danang Car Cheap Travel</a></li>
                    <li><i class="fa-solid fa-map-pin text-red-500 mr-2"></i>Google Map: <a href="https://maps.app.goo.gl/DW8HgefYWRvuhmQ29" target="_blank" rel="noopener noreferrer" class="text-yellow-400 hover:underline">Xem đường đi</a></li>
                </ul>
            </div>
        </div>
        <div class="flatsome-container pt-6 text-center text-xs text-slate-500">
            © 2026 Bản quyền thuộc về <strong>danangcarcheaptravel.com</strong> (DVDL Đức Võ - 0905.548.767). Thiết kế tối ưu UX Builder Flatsome.
        </div>
    </footer>

    <!-- ================= CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE) ================= -->
    <div class="fixed bottom-4 left-4 z-50 flex flex-col gap-3">
        <!-- Nút Facebook Fanpage -->
        <a href="https://www.facebook.com/danang.car.cheap.travel.2025/" target="_blank" rel="noopener noreferrer" 
           class="flex items-center gap-2.5 bg-blue-600 hover:bg-blue-700 text-white px-3.5 py-2.5 rounded-full shadow-lg transition transform hover:scale-105">
            <span class="w-8 h-8 rounded-full bg-white text-blue-600 flex items-center justify-center text-lg font-bold">
                <i class="fa-brands fa-facebook-f"></i>
            </span>
            <span class="font-bold text-xs sm:text-sm pr-1">Chat Facebook</span>
        </a>

        <!-- Nút Zalo -->
        <a href="https://zalo.me/0905548767" target="_blank" rel="noopener noreferrer" 
           class="flex items-center gap-2.5 bg-sky-500 hover:bg-sky-600 text-white px-3.5 py-2.5 rounded-full shadow-lg transition transform hover:scale-105">
            <span class="w-8 h-8 rounded-full bg-white text-sky-600 flex items-center justify-center text-xs font-black tracking-tighter">
                Zalo
            </span>
            <span class="font-bold text-xs sm:text-sm pr-1">Zalo: 0905.548.767</span>
        </a>

        <!-- Nút Hotline Nổi Bật -->
        <a href="tel:0905548767" 
           class="pulse-btn flex items-center gap-2.5 bg-red-600 hover:bg-red-700 text-white px-4 py-2.5 rounded-full shadow-xl transition transform hover:scale-105">
            <span class="w-8 h-8 rounded-full bg-yellow-400 text-red-800 flex items-center justify-center text-base font-bold">
                <i class="fa-solid fa-phone-volume"></i>
            </span>
            <div class="text-left leading-tight pr-1">
                <span class="block text-[10px] text-yellow-200 font-medium">Gọi đặt xe 24/24</span>
                <span class="font-extrabold text-sm sm:text-base">0905.548.767</span>
            </div>
        </a>
    </div>

    <!-- ================= MODAL ĐẶT XE NHANH ================= -->
    <div id="bookingModal" class="fixed inset-0 bg-black/60 z-50 hidden items-center justify-center p-4">
        <div class="bg-white rounded-xl max-w-md w-full p-6 relative shadow-2xl">
            <button onclick="closeModal()" class="absolute top-3 right-3 w-8 h-8 rounded-full bg-slate-100 hover:bg-slate-200 text-slate-600 flex items-center justify-center">
                <i class="fa-solid fa-xmark"></i>
            </button>
            <h3 class="text-lg font-extrabold text-red-700 uppercase mb-1">Đặt Thuê Xe Nhanh</h3>
            <p id="modalCarName" class="text-sm font-bold text-slate-700 mb-4">Dòng xe: Toyota Vios</p>
            <form onsubmit="submitBooking(event)" class="space-y-3 text-sm">
                <div>
                    <label class="block font-semibold text-slate-700 mb-1">Họ và tên quý khách *</label>
                    <input type="text" required placeholder="Nhập họ tên của bạn" class="w-full border border-slate-300 rounded-lg px-3 py-2 focus:outline-none focus:border-red-600">
                </div>
                <div>
                    <label class="block font-semibold text-slate-700 mb-1">Số điện thoại / Zalo *</label>
                    <input type="tel" required placeholder="Nhập số điện thoại liên hệ" class="w-full border border-slate-300 rounded-lg px-3 py-2 focus:outline-none focus:border-red-600">
                </div>
                <div class="grid grid-cols-2 gap-2">
                    <div>
                        <label class="block font-semibold text-slate-700 mb-1">Ngày nhận xe</label>
                        <input type="date" class="w-full border border-slate-300 rounded-lg px-2.5 py-2 focus:outline-none focus:border-red-600">
                    </div>
                    <div>
                        <label class="block font-semibold text-slate-700 mb-1">Hình thức thuê</label>
                        <select class="w-full border border-slate-300 rounded-lg px-2.5 py-2 focus:outline-none focus:border-red-600">
                            <option>Thuê tự lái</option>
                            <option>Có tài xế</option>
                            <option>Đưa đón sân bay</option>
                            <option>Hợp đồng cưới hỏi</option>
                        </select>
                    </div>
                </div>
                <div id="bookingSuccessMsg" class="hidden bg-green-50 border border-green-300 text-green-800 p-3 rounded-lg text-xs font-semibold">
                    Đã ghi nhận yêu cầu! Quý khách có thể gọi trực tiếp 0905.548.767 hoặc nhấn nút Zalo bên dưới để nhận xe ngay.
                </div>
                <div class="pt-2 flex gap-2">
                    <button type="submit" class="flex-1 bg-red-700 hover:bg-red-800 text-white font-bold py-2.5 rounded-lg transition">
                        GỬI YÊU CẦU ĐẶT XE
                    </button>
                    <a href="tel:0905548767" class="bg-yellow-500 hover:bg-yellow-400 text-slate-950 font-bold px-4 py-2.5 rounded-lg flex items-center justify-center">
                        <i class="fa-solid fa-phone mr-1"></i>Gọi ngay
                    </a>
                </div>
            </form>
        </div>
    </div>

    <!-- ================= JAVASCRIPT DỮ LIỆU SẢN PHẨM & TƯƠNG TÁC ================= -->
    <script>
        // Dữ liệu xe thực tế theo mẫu thuexetulaidanang.com & DVDL Đức Võ (Không nhãn dán ở trang chủ)
        const cars4Cho = [
            {
                name: "Thuê Xe Kia Morning Tự Lái",
                gear: "Tự động",
                seats: "4 chỗ",
                year: "2022",
                price: "600.000 VNĐ",
                image: "https://images.unsplash.com/photo-1541899481282-d53bffe3c35d?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Hyundai Grand i10",
                gear: "Tự động",
                seats: "4 chỗ",
                year: "2023",
                price: "600.000 VNĐ",
                image: "https://images.unsplash.com/photo-1552519507-da3b142c6e3d?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe VinFast Fadil Tự Lái",
                gear: "Tự động",
                seats: "4 chỗ",
                year: "2022",
                price: "650.000 VNĐ",
                image: "https://images.unsplash.com/photo-1580273916550-e323be2ae537?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Toyota Vios Tự Lái",
                gear: "Tự động",
                seats: "4 chỗ",
                year: "2024",
                price: "800.000 VNĐ",
                image: "https://images.unsplash.com/photo-1621007947382-bb3c3994e3fb?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Hyundai Accent",
                gear: "Tự động",
                seats: "4 chỗ",
                year: "2024",
                price: "800.000 VNĐ",
                image: "https://images.unsplash.com/photo-1619767886558-efdc259cde1a?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Honda City RS",
                gear: "Tự động",
                seats: "4 chỗ",
                year: "2023",
                price: "850.000 VNĐ",
                image: "https://images.unsplash.com/photo-1609521263047-f8f205293f24?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Mazda 3 Luxury",
                gear: "Tự động",
                seats: "4 chỗ",
                year: "2023",
                price: "900.000 VNĐ",
                image: "https://images.unsplash.com/photo-1555215695-3004980ad54e?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Kia K3 Premium",
                gear: "Tự động",
                seats: "4 chỗ",
                year: "2024",
                price: "900.000 VNĐ",
                image: "https://images.unsplash.com/photo-1617788138017-80ad40651399?auto=format&fit=crop&w=700&q=80"
            }
        ];

        const cars7Cho = [
            {
                name: "Thuê Xe Mitsubishi Xpander",
                gear: "Tự động",
                seats: "7 chỗ",
                year: "2024",
                price: "900.000 VNĐ",
                image: "https://images.unsplash.com/photo-1533473359331-0135ef1b58bf?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Toyota Veloz Cross",
                gear: "Tự động",
                seats: "7 chỗ",
                year: "2023",
                price: "900.000 VNĐ",
                image: "https://images.unsplash.com/photo-1519641471654-76ce0107ad1b?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Toyota Innova",
                gear: "Số sàn / AT",
                seats: "7 chỗ",
                year: "2022",
                price: "900.000 VNĐ",
                image: "https://images.unsplash.com/photo-1563720223185-11003d516935?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Mazda CX-5 Deluxe",
                gear: "Tự động",
                seats: "5 chỗ CUV",
                year: "2024",
                price: "1.000.000 VNĐ",
                image: "https://images.unsplash.com/photo-1549399542-7e3f8b79c341?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Honda CR-V L",
                gear: "Tự động",
                seats: "7 chỗ",
                year: "2023",
                price: "1.100.000 VNĐ",
                image: "https://images.unsplash.com/photo-1568844293986-8d0400bd4745?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Toyota Fortuner",
                gear: "Tự động",
                seats: "7 chỗ",
                year: "2023",
                price: "1.200.000 VNĐ",
                image: "https://images.unsplash.com/photo-1503376780353-7e6692767b70?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Ford Everest Titanium",
                gear: "Tự động",
                seats: "7 chỗ",
                year: "2024",
                price: "1.300.000 VNĐ",
                image: "https://images.unsplash.com/photo-1606664515524-ed2f786a0bd6?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Kia Carnival Luxury",
                gear: "Tự động",
                seats: "7 chỗ VIP",
                year: "2024",
                price: "2.000.000 VNĐ",
                image: "https://images.unsplash.com/photo-1549317661-bd32c8ce0db2?auto=format&fit=crop&w=700&q=80"
            }
        ];

        const carsBanTai = [
            {
                name: "Thuê Xe Bán Tải Ford Ranger",
                gear: "Tự động",
                seats: "5 chỗ",
                year: "2023",
                price: "1.100.000 VNĐ",
                image: "https://images.unsplash.com/photo-1559416523-140ddc3d238c?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Mitsubishi Triton",
                gear: "Tự động",
                seats: "5 chỗ",
                year: "2023",
                price: "1.000.000 VNĐ",
                image: "https://images.unsplash.com/photo-1519641471654-76ce0107ad1b?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Toyota Hilux 4x4",
                gear: "Tự động",
                seats: "5 chỗ",
                year: "2022",
                price: "1.000.000 VNĐ",
                image: "https://images.unsplash.com/photo-1533473359331-0135ef1b58bf?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Thuê Xe Nissan Navara Pro4X",
                gear: "Tự động",
                seats: "5 chỗ",
                year: "2023",
                price: "1.000.000 VNĐ",
                image: "https://images.unsplash.com/photo-1606664515524-ed2f786a0bd6?auto=format&fit=crop&w=700&q=80"
            }
        ];

        const carsDuLich = [
            {
                name: "Xe 16 Chỗ Ford Transit Có Tài",
                gear: "Có tài xế",
                seats: "16 chỗ",
                year: "2024",
                price: "Theo lịch trình",
                image: "https://images.unsplash.com/photo-1544620347-c4fd4a3d5957?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Xe 16 Chỗ Hyundai Solati",
                gear: "Có tài xế",
                seats: "16 chỗ",
                year: "2024",
                price: "Theo lịch trình",
                image: "https://images.unsplash.com/photo-1570125909232-eb263c188f7e?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Xe Đưa Đón Sân Bay & Đi Tỉnh",
                gear: "Phục vụ 24/24",
                seats: "4 - 7 - 16 chỗ",
                year: "2024",
                price: "Từ 250.000 VNĐ",
                image: "https://images.unsplash.com/photo-1449965408869-eaa3f722e40d?auto=format&fit=crop&w=700&q=80"
            },
            {
                name: "Xe Hoa Cưới Hỏi Đà Nẵng",
                gear: "Có tài xế",
                seats: "4 - 7 - 16 chỗ",
                year: "2024",
                price: "Báo giá trọn gói",
                image: "https://images.unsplash.com/photo-1511919884226-fd3cad34687c?auto=format&fit=crop&w=700&q=80"
            }
        ];

        // Hàm render Product Box chuẩn Flatsome (Hoàn toàn KHÔNG có nhãn dán/sticker trên ảnh)
        function renderProductGrid(containerId, list) {
            const container = document.getElementById(containerId);
            if (!container) return;
            container.innerHTML = list.map(item => `
                <div class="bg-white border border-slate-200 rounded-xl overflow-hidden shadow-sm hover:shadow-md transition flex flex-col justify-between">
                    <div>
                        <div class="aspect-[16/10] w-full overflow-hidden bg-slate-100">
                            <img src="${item.image}" 
                                 alt="${item.name}" 
                                 class="w-full h-full object-cover hover:scale-105 transition duration-300"
                                 onerror="this.src='https://placehold.co/600x400/e2e8f0/991b1b?text=DVDL+DUC+VO'">
                        </div>
                        <div class="p-3 sm:p-4">
                            <h3 class="font-bold text-slate-800 text-xs sm:text-base line-clamp-2 min-h-[2.25rem] sm:min-h-[2.75rem] hover:text-red-700 transition">
                                ${item.name}
                            </h3>
                            <ul class="mt-2 space-y-1 text-[11px] sm:text-xs text-slate-600 border-t border-slate-100 pt-2">
                                <li class="flex justify-between"><span>Số:</span> <strong class="text-slate-800">${item.gear}</strong></li>
                                <li class="flex justify-between"><span>Loại xe:</span> <strong class="text-slate-800">${item.seats}</strong></li>
                                <li class="flex justify-between"><span>Đời xe:</span> <strong class="text-slate-800">${item.year}</strong></li>
                                <li class="flex justify-between"><span>Thuê tháng:</span> <strong class="text-slate-700">Thương lượng</strong></li>
                            </ul>
                            <div class="mt-2.5 pt-2 border-t border-slate-100">
                                <span class="block text-[10px] sm:text-xs text-slate-500">Giá thuê ngày:</span>
                                <span class="text-sm sm:text-lg font-extrabold text-red-700">${item.price}</span>
                            </div>
                        </div>
                    </div>
                    <div class="p-3 sm:p-4 pt-0 grid grid-cols-2 gap-1.5 sm:gap-2">
                        <button onclick="openBookingModal('${item.name}')" class="bg-red-700 hover:bg-red-800 text-white font-bold py-2 px-2 rounded-lg text-[11px] sm:text-xs uppercase transition text-center">
                            Thuê nhanh
                        </button>
                        <a href="tel:0905548767" class="bg-slate-100 hover:bg-slate-200 text-slate-800 font-bold py-2 px-2 rounded-lg text-[11px] sm:text-xs uppercase transition text-center flex items-center justify-center">
                            Gọi ngay
                        </a>
                    </div>
                </div>
            `).join('');
        }

        // Khởi tạo danh sách xe
        renderProductGrid('grid-4-cho', cars4Cho);
        renderProductGrid('grid-7-cho', cars7Cho);
        renderProductGrid('grid-ban-tai', carsBanTai);
        renderProductGrid('grid-du-lich', carsDuLich);

        // Slider 2 Banner tự trượt
        let currentSlide = 0;
        const slides = document.querySelectorAll('.banner-slide');
        const dots = document.querySelectorAll('.slide-dot');

        function showSlide(index) {
            currentSlide = (index + slides.length) % slides.length;
            slides.forEach((slide, i) => {
                if (i === currentSlide) {
                    slide.classList.remove('opacity-0', 'z-0');
                    slide.classList.add('opacity-100', 'z-10');
                } else {
                    slide.classList.remove('opacity-100', 'z-10');
                    slide.classList.add('opacity-0', 'z-0');
                }
            });
            dots.forEach((dot, i) => {
                if (i === currentSlide) {
                    dot.classList.add('w-8', 'bg-yellow-400');
                    dot.classList.remove('w-2.5', 'bg-white/60');
                } else {
                    dot.classList.remove('w-8', 'bg-yellow-400');
                    dot.classList.add('w-2.5', 'bg-white/60');
                }
            });
        }

        function changeSlide(step) {
            showSlide(currentSlide + step);
        }

        function goToSlide(index) {
            showSlide(index);
        }

        // Tự động trượt mỗi 4.5 giây
        setInterval(() => {
            changeSlide(1);
        }, 4500);

        // Menu Mobile Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mobileMenuDrawer = document.getElementById('mobileMenuDrawer');
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenuDrawer.classList.toggle('hidden');
        });

        // Modal Đặt xe nhanh
        function openBookingModal(carName) {
            document.getElementById('modalCarName').textContent = 'Dòng xe: ' + carName;
            document.getElementById('bookingSuccessMsg').classList.add('hidden');
            const modal = document.getElementById('bookingModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function closeModal() {
            const modal = document.getElementById('bookingModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        function submitBooking(e) {
            e.preventDefault();
            document.getElementById('bookingSuccessMsg').classList.remove('hidden');
        }
    </script>
</body>
</html>
