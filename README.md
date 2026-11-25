<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chelsi Rianti Putri Motulo - Profil Pribadi</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Plus Jakarta Sans & Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet">
    <!-- Font Awesome untuk Ikon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        display: ['Plus Jakarta Sans', 'sans-serif'],
                    },
                    colors: {
                        royal: {
                            50: '#eff6ff',
                            100: '#dbeafe',
                            200: '#bfdbfe',
                            500: '#2563eb',
                            600: '#1d4ed8',
                            700: '#1e40af',
                            800: '#1e3a8a',
                            900: '#172554',
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-slate-50 text-slate-800 antialiased selection:bg-royal-600 selection:text-white">

    <!-- Notifikasi Toast (Pengganti alert) -->
    <div id="toast-notification" class="fixed bottom-5 right-5 z-50 transform translate-y-24 opacity-0 transition-all duration-300 bg-royal-900 text-white px-5 py-3.5 rounded-2xl shadow-xl flex items-center gap-3 border border-royal-700">
        <i class="fa-solid fa-circle-check text-blue-400 text-lg"></i>
        <span id="toast-message" class="text-sm font-medium">Perubahan berhasil disimpan!</span>
    </div>

    <!-- Navigasi Atas (Navbar) -->
    <header class="sticky top-0 z-40 bg-white/85 backdrop-blur-md border-b border-slate-200/80 transition-all">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16 sm:h-20">
                <!-- Logo / Nama Singkat -->
                <a href="#profil" class="flex items-center gap-2.5 group">
                    <div class="w-9 h-9 rounded-xl bg-gradient-to-br from-royal-600 to-royal-800 text-white flex items-center justify-center font-display font-bold text-lg shadow-sm group-hover:scale-105 transition-transform">
                        C
                    </div>
                    <span class="font-display font-bold text-lg sm:text-xl text-slate-900 tracking-tight">
                        Chelsi<span class="text-royal-600">.</span>
                    </span>
                </a>

                <!-- Menu Desktop -->
                <nav class="hidden md:flex items-center gap-8">
                    <a href="#profil" class="text-sm font-medium text-slate-600 hover:text-royal-600 transition-colors">Profil</a>
                    <a href="#biodata" class="text-sm font-medium text-slate-600 hover:text-royal-600 transition-colors">Biodata</a>
                    <a href="#tentang" class="text-sm font-medium text-slate-600 hover:text-royal-600 transition-colors">Tentang Saya</a>
                    <a href="#kontak" class="px-5 py-2.5 rounded-full bg-royal-600 hover:bg-royal-700 text-white text-sm font-medium shadow-sm shadow-royal-600/20 transition-all">
                        Hubungi Saya
                    </a>
                </nav>

                <!-- Tombol Menu Mobile -->
                <button id="mobile-menu-btn" aria-label="Buka Menu" class="md:hidden p-2.5 rounded-xl text-slate-600 hover:bg-slate-100 focus:outline-none">
                    <i class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Dropdown Menu Mobile -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-b border-slate-200 px-4 pt-2 pb-5 space-y-2 shadow-lg">
            <a href="#profil" class="block px-4 py-2.5 rounded-xl text-base font-medium text-slate-700 hover:bg-royal-50 hover:text-royal-600">Profil</a>
            <a href="#biodata" class="block px-4 py-2.5 rounded-xl text-base font-medium text-slate-700 hover:bg-royal-50 hover:text-royal-600">Biodata</a>
            <a href="#tentang" class="block px-4 py-2.5 rounded-xl text-base font-medium text-slate-700 hover:bg-royal-50 hover:text-royal-600">Tentang Saya</a>
            <a href="#kontak" class="block px-4 py-2.5 rounded-xl text-base font-medium text-royal-600 bg-royal-50 font-semibold">Kontak & Media Sosial</a>
        </div>
    </header>

    <main>
        <!-- Bagian Utama (Hero Section) -->
        <section id="profil" class="relative overflow-hidden pt-10 pb-20 sm:pt-16 sm:pb-28 bg-gradient-to-b from-royal-50/70 via-white to-slate-50">
            <!-- Dekorasi Latar Belakang Halus -->
            <div class="absolute top-0 right-0 -translate-y-12 translate-x-1/3 w-96 h-96 bg-royal-200/40 rounded-full blur-3xl pointer-events-none"></div>
            <div class="absolute bottom-0 left-0 translate-y-1/3 -translate-x-1/4 w-80 h-80 bg-blue-100/60 rounded-full blur-3xl pointer-events-none"></div>

            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-10 items-center">
                    
                    <!-- Kolom Foto Profil (Menonjol di Halaman Depan) -->
                    <div class="lg:col-span-5 flex justify-center order-1 lg:order-2">
                        <div class="relative group">
                            <!-- Aksen Bingkai Belakang -->
                            <div class="absolute -inset-3 bg-gradient-to-tr from-royal-700 via-royal-500 to-blue-300 rounded-[2rem] opacity-25 group-hover:opacity-40 blur-md transition-opacity duration-500"></div>
                            <div class="absolute -inset-1.5 bg-gradient-to-tr from-royal-600 to-blue-400 rounded-[1.85rem] transform rotate-2 group-hover:rotate-1 transition-transform duration-300"></div>
                            
                            <!-- Bingkai Foto Utama -->
                            <div class="relative bg-white p-2.5 rounded-[1.75rem] shadow-xl border border-blue-100">
                                <div class="w-64 h-80 sm:w-72 sm:h-96 rounded-2xl overflow-hidden bg-royal-600 relative">
                                    <img 
                                        src="IMG_0314 (3).jpg" 
                                        alt="Foto Profil Chelsi Rianti Putri Motulo" 
                                        class="w-full h-full object-cover object-top transform group-hover:scale-103 transition-transform duration-500"
                                        onerror="this.onerror=null; this.src='https://placehold.co/400x500/1d4ed8/ffffff?text=Chelsi+Motulo';"
                                    >
                                </div>
                                <!-- Badge Lokasi Mengambang -->
                                <div class="absolute -bottom-4 left-1/2 -translate-x-1/2 bg-white px-4 py-2 rounded-full shadow-md border border-slate-100 flex items-center gap-2 whitespace-nowrap">
                                    <span class="w-2.5 h-2.5 rounded-full bg-emerald-500 animate-pulse"></span>
                                    <span class="text-xs font-semibold text-slate-700">Tomohon, Sulawesi Utara</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Kolom Sapaan & Perkenalan -->
                    <div class="lg:col-span-7 text-center lg:text-left order-2 lg:order-1 space-y-6">
                        <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-royal-100/80 text-royal-800 text-xs sm:text-sm font-semibold tracking-wide">
                            <i class="fa-solid fa-sparkles text-royal-600"></i>
                            <span>Selamat Datang di Halaman Profil Saya</span>
                        </div>

                        <h1 class="font-display text-3xl sm:text-5xl lg:text-[3.25rem] font-extrabold text-slate-900 leading-[1.15] tracking-tight">
                            Halo, Saya <br class="hidden sm:block">
                            <span class="text-transparent bg-clip-text bg-gradient-to-r from-royal-700 to-royal-500">
                                Chelsi Rianti Putri Motulo
                            </span>
                        </h1>

                        <p class="text-base sm:text-lg text-slate-600 max-w-2xl mx-auto lg:mx-0 leading-relaxed">
                            Senang berkenalan dengan Anda! Saya adalah pribadi yang antusias dalam belajar hal-hal baru, berkembang secara positif, dan menjalin relasi yang baik. Temukan informasi lengkap mengenai profil dan perjalanan saya di sini.
                        </p>

                        <!-- Tombol Aksi Cepat -->
                        <div class="pt-2 flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4">
                            <a href="#biodata" class="w-full sm:w-auto px-7 py-3.5 rounded-2xl bg-royal-600 hover:bg-royal-700 text-white font-semibold text-sm sm:text-base shadow-lg shadow-royal-600/25 flex items-center justify-center gap-2.5 transition-all hover:-translate-y-0.5">
                                <span>Lihat Biodata Lengkap</span>
                                <i class="fa-solid fa-arrow-down text-xs"></i>
                            </a>
                            <a href="#tentang" class="w-full sm:w-auto px-7 py-3.5 rounded-2xl bg-white hover:bg-slate-50 text-slate-700 border border-slate-200 font-semibold text-sm sm:text-base shadow-sm flex items-center justify-center gap-2 transition-all">
                                <span>Tentang & Minat Saya</span>
                            </a>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- Bagian Biodata / Informasi Pribadi -->
        <section id="biodata" class="py-16 sm:py-24 bg-white border-y border-slate-200/70">
            <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center max-w-2xl mx-auto mb-12 sm:mb-16">
                    <span class="text-royal-600 font-semibold text-sm uppercase tracking-wider">Informasi Pribadi</span>
                    <h2 class="font-display text-2xl sm:text-4xl font-bold text-slate-900 mt-2">Biodata Singkat</h2>
                    <p class="text-slate-500 mt-3 text-sm sm:text-base">Data diri utama untuk mengenal saya lebih dekat secara formal maupun personal.</p>
                </div>

                <!-- Kartu Biodata Rapi -->
                <div class="bg-gradient-to-br from-slate-50 to-royal-50/40 rounded-3xl p-6 sm:p-10 border border-slate-200/80 shadow-sm">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 sm:gap-8">
                        
                        <!-- Item 1: Nama Lengkap -->
                        <div class="bg-white p-5 rounded-2xl border border-slate-100 shadow-sm flex items-start gap-4 hover:border-royal-200 transition-colors">
                            <div class="w-12 h-12 rounded-xl bg-royal-100 text-royal-600 flex items-center justify-center shrink-0 text-lg">
                                <i class="fa-solid fa-user"></i>
                            </div>
                            <div>
                                <p class="text-xs font-semibold uppercase tracking-wider text-slate-400">Nama Lengkap</p>
                                <p class="text-base sm:text-lg font-bold text-slate-900 mt-0.5">Chelsi Rianti Putri Motulo</p>
                            </div>
                        </div>

                        <!-- Item 2: Tempat, Tanggal Lahir -->
                        <div class="bg-white p-5 rounded-2xl border border-slate-100 shadow-sm flex items-start gap-4 hover:border-royal-200 transition-colors">
                            <div class="w-12 h-12 rounded-xl bg-royal-100 text-royal-600 flex items-center justify-center shrink-0 text-lg">
                                <i class="fa-solid fa-cake-candles"></i>
                            </div>
                            <div>
                                <p class="text-xs font-semibold uppercase tracking-wider text-slate-400">Tempat, Tanggal Lahir</p>
                                <p class="text-base sm:text-lg font-bold text-slate-900 mt-0.5">Tomohon, 14 Agustus 2007</p>
                            </div>
                        </div>

                        <!-- Item 3: Usia -->
                        <div class="bg-white p-5 rounded-2xl border border-slate-100 shadow-sm flex items-start gap-4 hover:border-royal-200 transition-colors">
                            <div class="w-12 h-12 rounded-xl bg-royal-100 text-royal-600 flex items-center justify-center shrink-0 text-lg">
                                <i class="fa-solid fa-hourglass-half"></i>
                            </div>
                            <div>
                                <p class="text-xs font-semibold uppercase tracking-wider text-slate-400">Usia Saat Ini</p>
                                <p class="text-base sm:text-lg font-bold text-slate-900 mt-0.5">
                                    <span id="umur-otomatis">19</span> Tahun
                                </p>
                            </div>
                        </div>

                        <!-- Item 4: Domisili / Asal -->
                        <div class="bg-white p-5 rounded-2xl border border-slate-100 shadow-sm flex items-start gap-4 hover:border-royal-200 transition-colors">
                            <div class="w-12 h-12 rounded-xl bg-royal-100 text-royal-600 flex items-center justify-center shrink-0 text-lg">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <div>
                                <p class="text-xs font-semibold uppercase tracking-wider text-slate-400">Asal / Domisili</p>
                                <p class="text-base sm:text-lg font-bold text-slate-900 mt-0.5">Kota Tomohon, Sulawesi Utara</p>
                            </div>
                        </div>

                    </div>
                </div>
            </div>
        </section>

        <!-- Bagian Tentang Saya & Minat (Dengan Fitur Mode Edit Sederhana) -->
        <section id="tentang" class="py-16 sm:py-24 bg-slate-50">
            <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
                
                <!-- Header Bagian & Tombol Mode Edit -->
                <div class="flex flex-col sm:flex-row sm:items-end justify-between gap-4 mb-10 sm:mb-12">
                    <div>
                        <span class="text-royal-600 font-semibold text-sm uppercase tracking-wider">Mengenal Lebih Jauh</span>
                        <h2 class="font-display text-2xl sm:text-4xl font-bold text-slate-900 mt-2">Tentang Saya & Minat</h2>
                    </div>
                    
                    <button id="toggle-edit-btn" onclick="toggleEditMode()" class="self-start sm:self-auto px-4 py-2.5 rounded-xl bg-white hover:bg-royal-50 text-royal-700 border border-royal-200 text-sm font-semibold shadow-sm flex items-center gap-2 transition-all">
                        <i id="edit-icon" class="fa-solid fa-pen-to-square"></i>
                        <span id="edit-btn-text">Sesuaikan Teks Profil</span>
                    </button>
                </div>

                <!-- Panduan Singkat Saat Mode Edit Aktif -->
                <div id="edit-guide" class="hidden mb-8 p-4 rounded-2xl bg-royal-600 text-white flex items-start sm:items-center gap-3 shadow-md">
                    <i class="fa-solid fa-circle-info text-xl shrink-0 mt-0.5 sm:mt-0"></i>
                    <p class="text-xs sm:text-sm leading-relaxed">
                        <strong>Mode Edit Aktif:</strong> Klik langsung pada teks di dalam kartu di bawah ini untuk mengubah riwayat pendidikan, hobi, atau keahlian Anda. Tekan tombol <strong>"Simpan Perubahan"</strong> jika sudah selesai (tersimpan otomatis di browser Anda).
                    </p>
                </div>

                <!-- Grid Kartu Tentang Saya -->
                <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                    
                    <!-- Kartu 1: Pendidikan -->
                    <div class="bg-white rounded-3xl p-6 sm:p-7 border border-slate-200/80 shadow-sm flex flex-col justify-between">
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-blue-50 text-royal-600 flex items-center justify-center text-xl mb-5">
                                <i class="fa-solid fa-graduation-cap"></i>
                            </div>
                            <h3 class="font-display text-lg font-bold text-slate-900 mb-3">Riwayat Pendidikan</h3>
                            <div id="editable-pendidikan" class="editable-field text-sm text-slate-600 space-y-2.5 leading-relaxed rounded-xl p-1 transition-all">
                                <p class="font-semibold text-slate-800">• Pendidikan Menengah / Lanjutan</p>
                                <p class="text-slate-500">Tomohon, Sulawesi Utara (Silakan klik "Sesuaikan Teks Profil" untuk mengisi nama sekolah atau perguruan tinggi Anda).</p>
                            </div>
                        </div>
                    </div>

                    <!-- Kartu 2: Hobi & Minat -->
                    <div class="bg-white rounded-3xl p-6 sm:p-7 border border-slate-200/80 shadow-sm flex flex-col justify-between">
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-blue-50 text-royal-600 flex items-center justify-center text-xl mb-5">
                                <i class="fa-solid fa-heart"></i>
                            </div>
                            <h3 class="font-display text-lg font-bold text-slate-900 mb-3">Hobi & Ketertarikan</h3>
                            <div id="editable-hobi" class="editable-field text-sm text-slate-600 space-y-2.5 leading-relaxed rounded-xl p-1 transition-all">
                                <p>• Membaca & mengeksplorasi wawasan baru</p>
                                <p>• Mendengarkan musik & kegiatan kreatif</p>
                                <p>• Berorganisasi dan berdiskusi positif</p>
                            </div>
                        </div>
                    </div>

                    <!-- Kartu 3: Keahlian & Pencapaian -->
                    <div class="bg-white rounded-3xl p-6 sm:p-7 border border-slate-200/80 shadow-sm flex flex-col justify-between">
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-blue-50 text-royal-600 flex items-center justify-center text-xl mb-5">
                                <i class="fa-solid fa-award"></i>
                            </div>
                            <h3 class="font-display text-lg font-bold text-slate-900 mb-3">Keahlian & Pencapaian</h3>
                            <div id="editable-keahlian" class="editable-field text-sm text-slate-600 space-y-2.5 leading-relaxed rounded-xl p-1 transition-all">
                                <p>• Komunikasi yang baik & kerja sama tim</p>
                                <p>• Manajemen waktu dan kedisiplinan</p>
                                <p>• Penguasaan dasar aplikasi komputer</p>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- Bagian Kontak & Media Sosial -->
        <section id="kontak" class="py-16 sm:py-24 bg-white border-t border-slate-200/70">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <span class="text-royal-600 font-semibold text-sm uppercase tracking-wider">Tetap Terhubung</span>
                <h2 class="font-display text-2xl sm:text-4xl font-bold text-slate-900 mt-2">Kontak & Media Sosial</h2>
                <p class="text-slate-500 mt-3 max-w-xl mx-auto text-sm sm:text-base">
                    Jangan ragu untuk menyapa atau menghubungi saya melalui salah satu saluran komunikasi di bawah ini.
                </p>

                <!-- Kartu Tautan Kontak -->
                <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 sm:gap-6 mt-10">
                    
                    <!-- Email -->
                    <a href="mailto:chelsi.motulo@example.com" class="group p-6 rounded-3xl bg-slate-50 hover:bg-royal-600 border border-slate-200/80 hover:border-royal-600 transition-all duration-300 flex flex-col items-center text-center shadow-sm">
                        <div class="w-14 h-14 rounded-2xl bg-white text-royal-600 group-hover:scale-110 transition-transform flex items-center justify-center text-2xl shadow-sm mb-4">
                            <i class="fa-solid fa-envelope"></i>
                        </div>
                        <h3 class="font-display font-bold text-slate-900 group-hover:text-white transition-colors">Email</h3>
                        <p class="text-xs sm:text-sm text-slate-500 group-hover:text-blue-100 mt-1 break-all">chelsi.motulo@example.com</p>
                    </a>

                    <!-- Instagram -->
                    <a href="https://instagram.com/" target="_blank" rel="noopener noreferrer" class="group p-6 rounded-3xl bg-slate-50 hover:bg-royal-600 border border-slate-200/80 hover:border-royal-600 transition-all duration-300 flex flex-col items-center text-center shadow-sm">
                        <div class="w-14 h-14 rounded-2xl bg-white text-royal-600 group-hover:scale-110 transition-transform flex items-center justify-center text-2xl shadow-sm mb-4">
                            <i class="fa-brands fa-instagram"></i>
                        </div>
                        <h3 class="font-display font-bold text-slate-900 group-hover:text-white transition-colors">Instagram</h3>
                        <p class="text-xs sm:text-sm text-slate-500 group-hover:text-blue-100 mt-1">@chelsimotulo</p>
                    </a>

                    <!-- WhatsApp -->
                    <a href="https://wa.me/6281234567890" target="_blank" rel="noopener noreferrer" class="group p-6 rounded-3xl bg-slate-50 hover:bg-royal-600 border border-slate-200/80 hover:border-royal-600 transition-all duration-300 flex flex-col items-center text-center shadow-sm">
                        <div class="w-14 h-14 rounded-2xl bg-white text-royal-600 group-hover:scale-110 transition-transform flex items-center justify-center text-2xl shadow-sm mb-4">
                            <i class="fa-brands fa-whatsapp"></i>
                        </div>
                        <h3 class="font-display font-bold text-slate-900 group-hover:text-white transition-colors">WhatsApp</h3>
                        <p class="text-xs sm:text-sm text-slate-500 group-hover:text-blue-100 mt-1">+62 812-3456-7890</p>
                    </a>

                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-royal-900 text-white py-10">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row justify-between items-center gap-4 text-center sm:text-left">
            <div>
                <p class="font-display font-bold text-lg">Chelsi Rianti Putri Motulo</p>
                <p class="text-blue-200 text-xs mt-1">Tomohon, Sulawesi Utara • Indonesia</p>
            </div>
            <p class="text-blue-200/80 text-xs sm:text-sm">
                &copy; <span id="tahun-sekarang">2026</span> Chelsi Rianti Putri Motulo. Hak Cipta Dilindungi.
            </p>
        </div>
    </footer>

    <!-- JavaScript Interaktivitas -->
    <script>
        // 1. Menu Navigasi Mobile
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Tutup menu mobile saat tautan diklik
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // 2. Perhitungan Usia Otomatis (Lahir: 14 Agustus 2007)
        function hitungUsia() {
            const tanggalLahir = new Date(2007, 7, 14); // Bulan dimulai dari 0 (7 = Agustus)
            const hariIni = new Date();
            let usia = hariIni.getFullYear() - tanggalLahir.getFullYear();
            const selisihBulan = hariIni.getMonth() - tanggalLahir.getMonth();
            
            if (selisihBulan < 0 || (selisihBulan === 0 && hariIni.getDate() < tanggalLahir.getDate())) {
                usia--;
            }
            
            const elemenUmur = document.getElementById('umur-otomatis');
            if (elemenUmur && usia > 0) {
                elemenUmur.textContent = usia;
            }
            
            const elemenTahun = document.getElementById('tahun-sekarang');
            if (elemenTahun) {
                elemenTahun.textContent = hariIni.getFullYear();
            }
        }

        // 3. Fitur Mode Edit Sederhana untuk Bagian "Tentang Saya"
        let isEditing = false;
        const editableIds = ['editable-pendidikan', 'editable-hobi', 'editable-keahlian'];

        // Muat data tersimpan dari localStorage jika ada
        function muatDataTersimpan() {
            editableIds.forEach(id => {
                const savedContent = localStorage.getItem('chelsi_profile_' + id);
                if (savedContent) {
                    document.getElementById(id).innerHTML = savedContent;
                }
            });
        }

        function toggleEditMode() {
            isEditing = !isEditing;
            const btnText = document.getElementById('edit-btn-text');
            const editIcon = document.getElementById('edit-icon');
            const editBtn = document.getElementById('toggle-edit-btn');
            const editGuide = document.getElementById('edit-guide');

            editableIds.forEach(id => {
                const el = document.getElementById(id);
                el.contentEditable = isEditing;
                if (isEditing) {
                    el.classList.add('bg-royal-50/70', 'ring-2', 'ring-royal-400', 'p-3');
                } else {
                    el.classList.remove('bg-royal-50/70', 'ring-2', 'ring-royal-400', 'p-3');
                    // Simpan ke localStorage
                    localStorage.setItem('chelsi_profile_' + id, el.innerHTML);
                }
            });

            if (isEditing) {
                btnText.textContent = 'Simpan Perubahan';
                editIcon.className = 'fa-solid fa-check';
                editBtn.classList.remove('bg-white', 'text-royal-700');
                editBtn.classList.add('bg-emerald-600', 'text-white', 'border-emerald-600');
                editGuide.classList.remove('hidden');
            } else {
                btnText.textContent = 'Sesuaikan Teks Profil';
                editIcon.className = 'fa-solid fa-pen-to-square';
                editBtn.classList.add('bg-white', 'text-royal-700');
                editBtn.classList.remove('bg-emerald-600', 'text-white', 'border-emerald-600');
                editGuide.classList.add('hidden');
                tampilkanNotifikasi('Teks profil berhasil diperbarui!');
            }
        }

        // Notifikasi Toast Ringan
        function tampilkanNotifikasi(pesan) {
            const toast = document.getElementById('toast-notification');
            const toastMsg = document.getElementById('toast-message');
            toastMsg.textContent = pesan;
            
            toast.classList.remove('translate-y-24', 'opacity-0');
            setTimeout(() => {
                toast.classList.add('translate-y-24', 'opacity-0');
            }, 3000);
        }

        // Jalankan saat halaman dimuat
        window.addEventListener('DOMContentLoaded', () => {
            hitungUsia();
            muatDataTersimpan();
        });
    </script>
</body>
</html>
