<!DOCTYPE html>
<html lang="id" class="dark scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nihiluxxy AI Pro - Super Learning Engine SMA, TKA & UTBK SNBT 2026</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f5f3ff', 100: '#ede9fe', 200: '#ddd6fe', 300: '#c4b5fd',
                            400: '#a78bfa', 500: '#8b5cf6', 600: '#7c3aed', 700: '#6d28d9',
                            800: '#5b21b6', 900: '#4c1d95', 950: '#2e1065',
                        }
                    },
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                        mono: ['JetBrains Mono', 'monospace'],
                    },
                    animation: {
                        'pulse-glow': 'pulseGlow 2.5s infinite alternate',
                        'float': 'float 4s ease-in-out infinite',
                    },
                    keyframes: {
                        pulseGlow: {
                            '0%': { boxShadow: '0 0 15px rgba(139, 92, 246, 0.25), 0 0 30px rgba(99, 102, 241, 0.15)' },
                            '100%': { boxShadow: '0 0 35px rgba(168, 85, 247, 0.55), 0 0 60px rgba(236, 72, 153, 0.3)' }
                        },
                        float: {
                            '0%, 100%': { transform: 'translateY(0px)' },
                            '50%': { transform: 'translateY(-8px)' }
                        }
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        body { 
            font-family: 'Plus Jakarta Sans', sans-serif; 
            background-color: #060913;
            background-image: 
                radial-gradient(at 0% 0%, rgba(124, 58, 237, 0.15) 0px, transparent 50%),
                radial-gradient(at 100% 0%, rgba(99, 102, 241, 0.15) 0px, transparent 50%),
                radial-gradient(at 50% 100%, rgba(236, 72, 153, 0.1) 0px, transparent 50%);
            background-attachment: fixed;
        }
        .gradient-brand { background: linear-gradient(135deg, #090e1a 0%, #161b33 45%, #2a224a 100%); }
        .gradient-accent { background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 50%, #ec4899 100%); }
        .glass-header { background: rgba(6, 9, 19, 0.85); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); }
        .glass-card { background: rgba(21, 29, 48, 0.45); backdrop-filter: blur(14px); -webkit-backdrop-filter: blur(14px); border: 1px solid rgba(255, 255, 255, 0.08); }
        .glass-modal { background: rgba(10, 14, 26, 0.95); backdrop-filter: blur(24px); -webkit-backdrop-filter: blur(24px); border: 1px solid rgba(139, 92, 246, 0.35); }
        
        .custom-scrollbar::-webkit-scrollbar { width: 6px; height: 6px; }
        .custom-scrollbar::-webkit-scrollbar-track { background: rgba(11, 16, 29, 0.7); }
        .custom-scrollbar::-webkit-scrollbar-thumb { background: rgba(139, 92, 246, 0.4); border-radius: 9999px; }
        .custom-scrollbar::-webkit-scrollbar-thumb:hover { background: rgba(139, 92, 246, 0.75); }
    </style>
</head>
<body class="bg-[#060913] text-slate-100 min-h-screen flex flex-col selection:bg-purple-500 selection:text-white custom-scrollbar relative">

    <!-- Top Announcement & AI Status Bar -->
    <div class="bg-gradient-to-r from-purple-950 via-slate-950 to-indigo-950 text-xs py-2 px-4 font-medium border-b border-purple-500/20 text-purple-200 flex justify-between items-center z-50">
        <div class="flex items-center gap-2">
            <span class="inline-flex items-center px-2.5 py-0.5 rounded-full text-[10px] font-black bg-purple-500/20 text-purple-300 border border-purple-500/40 shadow-sm">
                ⚡ Nihiluxxy AI Pro v5.0 Ultra
            </span>
            <span class="hidden sm:inline text-slate-300">Database Materi SMA Terlengkap & Bank Soal Simulasi UTBK SNBT 2026</span>
        </div>
        <div class="flex items-center gap-4 text-[11px] font-semibold text-purple-300">
            <span class="hidden md:flex items-center gap-1.5 font-mono text-emerald-400">
                <span class="w-2 h-2 rounded-full bg-emerald-400 animate-pulse"></span> Multi-Subject AI Active
            </span>
            <span class="text-slate-700 hidden md:inline">•</span>
            <span id="live-clock" class="font-mono text-purple-200 font-bold">--:--:-- WIB</span>
        </div>
    </div>

    <!-- Header Navigation Bar -->
    <header class="sticky top-0 z-40 glass-header border-b border-slate-800/80 transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between gap-4">
            
            <!-- Brand Logo -->
            <div class="flex items-center gap-3 cursor-pointer group" onclick="switchView('home')">
                <div class="w-11 h-11 rounded-2xl gradient-accent flex items-center justify-center text-white font-black text-xl shadow-lg shadow-purple-500/30 group-hover:scale-105 transition duration-300 animate-pulse-glow">
                    <i data-lucide="sparkles" class="w-6 h-6"></i>
                </div>
                <div class="flex flex-col">
                    <div class="flex items-center gap-1.5">
                        <span class="text-2xl font-black tracking-tight text-white group-hover:text-purple-300 transition">Nihiluxxy</span>
                        <span class="text-[9px] font-black px-1.5 py-0.5 rounded-md bg-gradient-to-r from-purple-500 to-pink-500 text-white uppercase tracking-wider">AI PRO</span>
                    </div>
                    <span class="text-[9px] uppercase tracking-widest text-purple-400 font-extrabold -mt-1">Super Learning Engine</span>
                </div>
            </div>

            <!-- Global Search Desktop -->
            <div class="hidden lg:flex items-center flex-1 max-w-md mx-6">
                <div class="relative w-full">
                    <i data-lucide="search" class="w-4 h-4 absolute left-3.5 top-1/2 -translate-y-1/2 text-slate-400"></i>
                    <input type="text" id="global-search" oninput="handleGlobalSearch(this.value)" placeholder="Cari materi & soal (misal: Integral, Turunan, Kirchhoff, Titrasi, Silogisme)..." class="w-full bg-slate-900/90 border border-slate-700/80 rounded-2xl pl-10 pr-12 py-2 text-xs text-slate-200 focus:outline-none focus:border-purple-500 focus:ring-1 focus:ring-purple-500 transition shadow-inner">
                    <kbd class="hidden sm:inline-block absolute right-3 top-1/2 -translate-y-1/2 text-[9px] bg-slate-800 border border-slate-700 px-1.5 py-0.5 rounded text-slate-400 font-mono font-bold">⌘K</kbd>
                    <div id="search-results-popover" class="hidden absolute left-0 right-0 top-12 bg-slate-900/95 border border-purple-500/30 rounded-2xl shadow-2xl p-2 z-50 max-h-80 overflow-y-auto custom-scrollbar backdrop-blur-xl"></div>
                </div>
            </div>

            <!-- Navigation Desktop -->
            <nav class="hidden md:flex items-center gap-1 bg-slate-900/90 p-1.5 rounded-2xl border border-slate-800 text-xs font-semibold">
                <button onclick="switchView('home')" id="nav-home" class="px-4 py-2.5 rounded-xl text-white bg-purple-600 transition flex items-center gap-1.5 font-bold shadow-md shadow-purple-600/30">
                    <i data-lucide="home" class="w-4 h-4"></i> Beranda
                </button>
                <button onclick="switchView('materi')" id="nav-materi" class="px-4 py-2.5 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="book-open" class="w-4 h-4"></i> Modul SMA
                </button>
                <button onclick="switchView('utbk')" id="nav-utbk" class="px-4 py-2.5 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="award" class="w-4 h-4 text-amber-400"></i> Simulasi UTBK
                </button>
                <button onclick="switchView('flashcards')" id="nav-flashcards" class="px-4 py-2.5 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="brain" class="w-4 h-4 text-emerald-400"></i> Flashcards
                </button>
                <button onclick="switchView('riwayat')" id="nav-riwayat" class="px-4 py-2.5 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="history" class="w-4 h-4 text-purple-400"></i> Riwayat
                </button>
            </nav>

            <!-- AI Quick Trigger Header Button -->
            <div class="flex items-center gap-3">
                <button onclick="toggleAiModal()" class="px-4 py-2.5 rounded-2xl bg-gradient-to-r from-purple-600 via-indigo-600 to-pink-600 hover:from-purple-500 hover:to-pink-500 text-white font-extrabold text-xs flex items-center gap-2 shadow-lg shadow-purple-500/25 border border-purple-400/40 transition transform hover:scale-105 active:scale-95">
                    <i data-lucide="bot" class="w-4 h-4 text-purple-100 animate-bounce"></i>
                    <span class="hidden sm:inline">AI Super Tutor</span>
                </button>
            </div>
        </div>
    </header>

    <!-- Main Content Dynamic Render Container -->
    <main id="app-content" class="flex-grow max-w-7xl w-full mx-auto px-4 sm:px-6 lg:px-8 py-8">
        <!-- Rendered dynamically by JS Engine -->
    </main>

    <!-- Floating AI Tutor Trigger Widget -->
    <div class="fixed bottom-20 md:bottom-8 right-6 z-40">
        <button onclick="toggleAiModal()" class="group relative flex items-center justify-center w-14 h-14 rounded-full gradient-accent text-white shadow-2xl shadow-purple-500/50 hover:scale-110 active:scale-95 transition-all duration-300 border-2 border-white/20">
            <i data-lucide="sparkles" class="w-7 h-7"></i>
            <span class="absolute -top-1 -right-1 w-4 h-4 rounded-full bg-emerald-400 border-2 border-slate-950 animate-ping"></span>
            <span class="absolute -top-1 -right-1 w-4 h-4 rounded-full bg-emerald-400 border-2 border-slate-950"></span>
            <div class="absolute right-16 top-1/2 -translate-y-1/2 hidden group-hover:flex items-center px-3.5 py-1.5 bg-slate-900 border border-purple-500/50 rounded-xl text-xs font-bold text-white whitespace-nowrap shadow-2xl backdrop-blur-md">
                <span>Tanyakan AI Super Tutor ⚡</span>
            </div>
        </button>
    </div>

    <!-- AI Tutor Interactive Chat Drawer Modal -->
    <div id="ai-tutor-modal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-3 sm:p-6 bg-slate-950/80 backdrop-blur-md transition-opacity">
        <div class="glass-modal w-full max-w-3xl rounded-3xl overflow-hidden shadow-2xl flex flex-col h-[88vh] border border-purple-500/40">
            
            <!-- AI Modal Header -->
            <div class="p-4 sm:p-5 bg-gradient-to-r from-purple-950 via-slate-900 to-indigo-950 border-b border-purple-500/30 flex items-center justify-between">
                <div class="flex items-center gap-3">
                    <div class="w-11 h-11 rounded-2xl gradient-accent flex items-center justify-center text-white font-bold shadow-lg shadow-purple-500/30">
                        <i data-lucide="bot" class="w-6 h-6"></i>
                    </div>
                    <div>
                        <div class="flex items-center gap-2">
                            <h3 class="font-black text-white text-base">Nihiluxxy AI Super Tutor</h3>
                            <span class="text-[9px] px-2 py-0.5 rounded-full bg-emerald-500/20 text-emerald-300 border border-emerald-500/40 font-mono font-bold">Ultra Intelligence v5.0</span>
                        </div>
                        <p class="text-[11px] text-purple-300">Pakar Matematika, Kalkulus, Sains, Soshum & UTBK SNBT 2026</p>
                    </div>
                </div>
                <button onclick="toggleAiModal()" class="w-9 h-9 rounded-xl bg-slate-800/80 hover:bg-slate-700 text-slate-400 hover:text-white flex items-center justify-center transition">
                    <i data-lucide="x" class="w-5 h-5"></i>
                </button>
            </div>

            <!-- AI Quick Action Chips Bar -->
            <div class="p-3 bg-slate-900/90 border-b border-slate-800 flex gap-2 overflow-x-auto custom-scrollbar text-xs">
                <button onclick="injectAiPrompt('Tolong jelaskan konsep Integral Tentu dan Luas Daerah dengan cara mudah!')" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-purple-900/50 border border-slate-700 text-purple-200 whitespace-nowrap transition flex items-center gap-1.5">
                    <i data-lucide="calculator" class="w-3.5 h-3.5 text-pink-400"></i> Integral & Luas
                </button>
                <button onclick="injectAiPrompt('Bagaimana cara cepat menyelesaikan Hukum Kirchhoff 2 Loop pada Fisika Listrik Dinamis?')" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-purple-900/50 border border-slate-700 text-purple-200 whitespace-nowrap transition flex items-center gap-1.5">
                    <i data-lucide="zap" class="w-3.5 h-3.5 text-amber-400"></i> Kirchhoff 2 Loop
                </button>
                <button onclick="injectAiPrompt('Buatkan 1 contoh soal HOTS Kimia tentang Penyetaraan Reaksi Redoks metode Suasana Asam beserta pembahasan!')" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-purple-900/50 border border-slate-700 text-purple-200 whitespace-nowrap transition flex items-center gap-1.5">
                    <i data-lucide="flask-conical" class="w-3.5 h-3.5 text-cyan-400"></i> Reaksi Redoks HOTS
                </button>
                <button onclick="injectAiPrompt('Jelaskan trik membedakan Modus Ponens, Modus Tollens, dan Silogisme untuk UTBK SNBT!')" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-purple-900/50 border border-slate-700 text-purple-200 whitespace-nowrap transition flex items-center gap-1.5">
                    <i data-lucide="brain" class="w-3.5 h-3.5 text-emerald-400"></i> Silogisme Logika
                </button>
            </div>

            <!-- AI Chat Body Container -->
            <div id="ai-chat-body" class="flex-1 p-4 sm:p-6 overflow-y-auto custom-scrollbar space-y-4 bg-slate-950/60">
                <div class="flex gap-3 items-start">
                    <div class="w-9 h-9 rounded-xl gradient-accent flex-shrink-0 flex items-center justify-center text-white text-xs font-bold shadow-md">AI</div>
                    <div class="bg-slate-900/90 border border-purple-500/30 p-4 sm:p-5 rounded-2xl text-xs sm:text-sm text-slate-200 max-w-xl leading-relaxed shadow-xl">
                        <p class="font-bold text-purple-300 text-sm mb-1">Selamat datang di Nihiluxxy AI Super Tutor v5.0! 🚀</p>
                        <p>Ketik soal, materi, atau rumus dari mata pelajaran apapun (Matematika Wajib/Lanjut, Fisika, Kimia, Biologi, Ekonomi, Sosiologi, Geografi, Penalaran Umum). AI akan membedah konsep dan langkah penyelesaiannya secara presisi!</p>
                    </div>
                </div>
            </div>

            <!-- AI Input Box Area -->
            <div class="p-3 sm:p-4 bg-slate-900 border-t border-slate-800 flex items-center gap-2">
                <textarea id="ai-user-input" rows="1" onkeydown="handleAiKeyDown(event)" placeholder="Ketik pertanyaan atau salin soal di sini (misal: 'Hitung turunan dari f(x) = x^3 - 3x + 2')..." class="flex-1 bg-slate-950 border border-slate-700/80 rounded-2xl px-4 py-3 text-xs sm:text-sm text-slate-100 focus:outline-none focus:border-purple-500 custom-scrollbar resize-none"></textarea>
                <button onclick="sendAiQuery()" class="w-12 h-12 rounded-2xl gradient-accent text-white flex items-center justify-center hover:opacity-95 transition shadow-lg shadow-purple-500/25 flex-shrink-0">
                    <i data-lucide="send" class="w-5 h-5"></i>
                </button>
            </div>
        </div>
    </div>

    <!-- Mobile Navigation Bottom Bar -->
    <div class="md:hidden fixed bottom-0 left-0 right-0 glass-header border-t border-slate-800/80 flex justify-around py-2.5 text-[10px] font-semibold text-slate-400 z-30 backdrop-blur-lg">
        <button onclick="switchView('home')" id="mob-home" class="flex flex-col items-center gap-1 text-purple-400 font-bold">
            <i data-lucide="home" class="w-5 h-5"></i> Beranda
        </button>
        <button onclick="switchView('materi')" id="mob-materi" class="flex flex-col items-center gap-1">
            <i data-lucide="book-open" class="w-5 h-5"></i> Modul SMA
        </button>
        <button onclick="switchView('utbk')" id="mob-utbk" class="flex flex-col items-center gap-1">
            <i data-lucide="award" class="w-5 h-5"></i> UTBK/TKA
        </button>
        <button onclick="switchView('flashcards')" id="mob-flashcards" class="flex flex-col items-center gap-1">
            <i data-lucide="brain" class="w-5 h-5"></i> Flashcards
        </button>
        <button onclick="switchView('riwayat')" id="mob-riwayat" class="flex flex-col items-center gap-1">
            <i data-lucide="history" class="w-5 h-5"></i> Riwayat
        </button>
    </div>

    <!-- Application Footer -->
    <footer class="mt-auto border-t border-slate-800/80 bg-slate-950/80 py-8 text-xs text-slate-400 relative z-10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center gap-4">
            <div class="flex items-center gap-2">
                <div class="w-6 h-6 rounded-lg gradient-accent flex items-center justify-center text-white text-xs font-bold">N</div>
                <span class="font-extrabold text-slate-200">Nihiluxxy AI Platform Edition 2026</span>
                <span class="text-slate-600">|</span>
                <span>Hak Cipta &copy; 2026. Kurikulum Merdeka & K13 Terverifikasi.</span>
            </div>
            <div class="flex gap-6 text-slate-400">
                <a href="#" onclick="toggleAiModal()" class="hover:text-purple-400 transition flex items-center gap-1">
                    <i data-lucide="bot" class="w-3.5 h-3.5 text-purple-400"></i> AI Assistant
                </a>
                <a href="#" class="hover:text-purple-400 transition">Panduan HOTS</a>
                <a href="#" class="hover:text-purple-400 transition">Kebijakan Privasi</a>
            </div>
        </div>
    </footer>

    <!-- JS Application Engine -->
    <script>
        // Realtime Clock
        setInterval(() => {
            const now = new Date();
            const timeStr = now.toLocaleTimeString('id-ID') + ' WIB';
            const clockEl = document.getElementById('live-clock');
            if (clockEl) clockEl.innerText = timeStr;
        }, 1000);

        // Keyboard Shortcut ⌘K / Ctrl+K
        document.addEventListener('keydown', (e) => {
            if ((e.metaKey || e.ctrlKey) && e.key === 'k') {
                e.preventDefault();
                document.getElementById('global-search')?.focus();
            }
        });

        // Core State
        const state = {
            activeView: 'home',
            selectedKurikulum: 'Merdeka',
            selectedSubject: 'mat',
            attempts: JSON.parse(localStorage.getItem('nihiluxxy_attempts') || '[]'),
            currentSimAnswers: {},
            activeSimKey: null,
            simTimerInterval: null,
            simTimeLeft: 0,
            currentFlashcardIdx: 0
        };

        // Highly Expanded Database Engine
        const db = {
            mapel: [
                { id: 'mat', nama: 'Matematika Wajib & Lanjut', icon: 'calculator', color: 'from-blue-600 to-cyan-500', k13: 'Kelas 10-12 IPA/IPS', merdeka: 'Fase E & F (Wajib & Tingkat Lanjut)' },
                { id: 'fis', nama: 'Fisika', icon: 'zap', color: 'from-indigo-600 to-blue-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Peminatan Sains)' },
                { id: 'kim', nama: 'Kimia', icon: 'flask-conical', color: 'from-purple-600 to-pink-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Peminatan Sains)' },
                { id: 'bio', nama: 'Biologi', icon: 'dna', color: 'from-emerald-600 to-teal-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Peminatan Sains)' },
                { id: 'eko', nama: 'Ekonomi & Akuntansi', icon: 'trending-up', color: 'from-amber-600 to-yellow-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Peminatan Sosial)' },
                { id: 'sos', nama: 'Sosiologi', icon: 'users', color: 'from-rose-600 to-red-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Peminatan Sosial)' },
                { id: 'geo', nama: 'Geografi', icon: 'globe', color: 'from-teal-600 to-emerald-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Peminatan Sosial)' },
                { id: 'lit', nama: 'Literasi Bahasa & Penalaran', icon: 'book-marked', color: 'from-orange-600 to-amber-500', k13: 'Wajib Semua Jurusan', merdeka: 'Fase E & F (General Literacy & PU)' }
            ],
            flashcards: [
                { mapel: 'Matematika', pertanyaan: 'Apakah turunan pertama dari f(x) = axⁿ menurut aturan turunan dasar?', jawaban: 'f\'(x) = a · n · xⁿ⁻¹.' },
                { mapel: 'Matematika', pertanyaan: 'Berapakah rumus integral tentu ∫ xⁿ dx untuk n ≠ -1?', jawaban: '∫ xⁿ dx = [1 / (n + 1)] · xⁿ⁺¹ + C.' },
                { mapel: 'Matematika', pertanyaan: 'Apakah syarat dua vektor u dan v tegak lurus (ortogonal)?', jawaban: 'Perkalian titiknya nol: u · v = 0.' },
                { mapel: 'Fisika', pertanyaan: 'Apakah Hukum Kirchhoff II tentang tegangan dalam sebuah loop tertutup?', jawaban: 'Jumlah perubahan potensial (ΣE + Σ(I·R)) dalam loop tertutup adalah nol.' },
                { mapel: 'Fisika', pertanyaan: 'Bagaimana nilai v_y pada titik puncak gerak parabola?', jawaban: 'v_y = 0 m/s.' },
                { mapel: 'Kimia', pertanyaan: 'Apakah perubahan yang terjadi saat Sistem Kesetimbangan ditambah konsentrasi pereaksinya?', jawaban: 'Kesetimbangan akan bergeser ke arah Kanan (ke arah Produk/Hasil Reaksi).' },
                { mapel: 'Kimia', pertanyaan: 'Apakah syarat wujud zat yang dihitung dalam rumus K_c?', jawaban: 'Hanya wujud Gas (g) dan Larutan/Aqueous (aq).' },
                { mapel: 'Biologi', pertanyaan: 'Apakah peran utama Klorofil dalam tahap Reaksi Terang Fotosintesis?', jawaban: 'Menyerap energi foton matahari dan mengalami eksitasi elektron.' },
                { mapel: 'Biologi', pertanyaan: 'Di manakah tempat terjadinya Siklus Krebs dalam sel?', jawaban: 'Di dalam Matriks Mitokondria.' },
                { mapel: 'Ekonomi', pertanyaan: 'Apakah rumus Elastisitas Harga Permintaan (E_d)?', jawaban: 'E_d = (% Perubahan Jumlah Permintaan) / (% Perubahan Harga).' },
                { mapel: 'Sosiologi', pertanyaan: 'Apakah perbedaan mendasar antara Akulturasi dan Asimilasi?', jawaban: 'Akulturasi: Pembauran budaya tanpa menghilangkan ciri asli. Asimilasi: Pembauran hingga membentuk budaya baru.' },
                { mapel: 'Geografi', pertanyaan: 'Apakah fungsi utama Citra Penginderaan Jauh inframerah termal?', jawaban: 'Mendeteksi suhu permukaan bumi, pemetaan vegetasi, dan persebaran kalor.' },
                { mapel: 'Penalaran Umum', pertanyaan: 'Apakah kesimpulan sah dari Modus Tollens: P → Q, ~Q?', jawaban: 'Kesimpulannya adalah ~P (Bukan P).' }
            ],
            materiDetails: {
                'mat': [
                    {
                        title: '1. Eksponen, Bentuk Akar & Logaritma (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Konsep Dasar:</strong> Eksponen adalah perkalian berulang. Logaritma adalah operasi invers dari eksponensial (aⁿ = b ⇔ ᵃlog b = n).',
                        visual: 'ᵃlog(b·c) = ᵃlog b + ᵃlog c  |  ᵃlog(b/c) = ᵃlog b - ᵃlog c  |  ᵃlog bⁿ = n · ᵃlog b',
                        tips: '<strong>Metode Cerdas:</strong> Jika menemui persamaan eksponen a^(f(x)) = a^(g(x)), langsung samakan pangkatnya f(x) = g(x).',
                        contohSoal: 'Jika ᵃlog b + ᵃlog b² = 12, hitung ᵃlog(a·b).<br><strong>Penyelesaian:</strong> 3 · ᵃlog b = 12 ⇒ ᵃlog b = 4. Maka ᵃlog(a·b) = ᵃlog a + ᵃlog b = 1 + 4 = <strong>5</strong>.'
                    },
                    {
                        title: '2. Persamaan Kuadrat & Rumus Vieta (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Konsep Dasar:</strong> ax² + bx + c = 0. Diskriminan D = b² - 4ac menentukan jenis akar (D > 0 dua akar real beda, D = 0 akar kembar, D < 0 imajiner).',
                        visual: 'Vieta: x₁ + x₂ = -b/a  |  x₁ · x₂ = c/a  |  Titik Puncak Parabola: (-b / 2a , -D / 4a)',
                        tips: 'Untuk mencari x₁² + x₂², gunakan identitas Vieta: (x₁ + x₂)² - 2(x₁·x₂).',
                        contohSoal: 'Jika x² - (k + 2)x + 16 = 0 memiliki dua akar kembar positif, tentukan k.<br><strong>Penyelesaian:</strong> D = (k+2)² - 64 = 0 ⇒ k+2 = ±8 ⇒ k = 6 atau -10. Syarat positif: x₁+x₂ = k+2 > 0 ⇒ <strong>k = 6</strong>.'
                    },
                    {
                        title: '3. Limit Fungsi Aljabar & Aturan L\'Hopital (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Konsep Dasar:</strong> Jika substitusi menghasilkan bentuk 0/0 atau ∞/∞, gunakan Aturan L\'Hopital (turunkan pembilang dan penyebut).',
                        visual: 'lim (x→c) [f(x) / g(x)] = lim (x→c) [f\'(x) / g\'(x)]',
                        tips: 'Gunakan L\'Hopital untuk menghemat waktu saat menghadapi limit pecahan aljabar di UTBK.',
                        contohSoal: 'Hitung lim (x→3) (x² - 9) / (x - 3).<br><strong>Jawab:</strong> Turunan pembilang (2x) & penyebut (1). lim (x→3) (2x / 1) = 2(3) = <strong>6</strong>.'
                    },
                    {
                        title: '4. Turunan Fungsi Aljabar & Garis Singgung (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Konsep Dasar:</strong> Turunan f\'(x) menyatakan gradien garis singgung kurva (m = f\'(x_1)). Titik stasioner terjadi saat f\'(x) = 0.',
                        visual: 'f(x) = u · v ⇒ f\'(x) = u\'v + uv\'  |  Gradien Garis Singgung m = f\'(x_1)',
                        tips: 'Untuk mencari nilai maksimum/minimum, cari akar f\'(x) = 0 lalu uji pada fungsi asal.',
                        contohSoal: 'Tentukan gradien garis singgung f(x) = x³ - 2x + 5 di titik x = 2.<br><strong>Jawab:</strong> f\'(x) = 3x² - 2 ⇒ m = f\'(2) = 3(2)² - 2 = 12 - 2 = <strong>10</strong>.'
                    },
                    {
                        title: '5. Integral Tentu & Luas Daerah Kurva (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Konsep Dasar:</strong> Integral adalah antiturunan. Integral tentu ∫[a,b] f(x) dx menghitung luas daerah di bawah kurva f(x) dari x=a hingga x=b.',
                        visual: 'Luas Antara 2 Kurva: L = ∫[a,b] (y_atas - y_bawah) dx  |  Dua Kurva: L = (D√D) / (6a²)',
                        tips: '<strong>Trik Cepat UTBK:</strong> Luas daerah dibatasi parabola dan garis dapat dihitung instan dengan L = (D√D) / (6a²).',
                        contohSoal: 'Hitung luas daerah dibatasi y = x² dan sumbu-X dari x = 0 hingga x = 3.<br><strong>Jawab:</strong> ∫[0,3] x² dx = [x³/3] limit 0 sampai 3 = (27/3) - 0 = <strong>9 satuan luas</strong>.'
                    }
                ],
                'fis': [
                    {
                        title: '1. Kinematika & Gerak Parabola (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Perpaduan GLB horizontal (v_x = v₀ cos θ) dan GLBB vertikal (v_y = v₀ sin θ - gt).',
                        visual: 'H_max = (v₀² sin² θ) / 2g  |  X_max = (v₀² sin 2θ) / g',
                        tips: 'Di titik tertinggi, v_y = 0 m/s, namun v_x tetap konstan v₀ cos θ.',
                        contohSoal: 'Batu dilempar v₀ = 20 m/s sudut 30° (g = 10 m/s²). Ketinggian maksimum?<br><strong>Jawab:</strong> H_max = (400 × (0.5)²) / 20 = <strong>5 meter</strong>.'
                    },
                    {
                        title: '2. Hukum Newton & Dinamika Gerak (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Hukum I (ΣF = 0), Hukum II (ΣF = m·a), Hukum III (F_aksi = -F_reaksi).',
                        visual: 'Gaya Gesek: f_g = μ · N  |  Komponen Bidang Miring: F_sejajar = m·g sin θ',
                        tips: 'Uraikan seluruh gaya sejajar dan tegak lurus bidang gerak.',
                        contohSoal: 'Balok 4 kg berada pada bidang miring licin 30° (g = 10 m/s²). Berapakah percepatannya?<br><strong>Jawab:</strong> a = g sin 30° = 10 × 0,5 = <strong>5 m/s²</strong>.'
                    },
                    {
                        title: '3. Gelombang Bunyi & Efek Doppler (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Perubahan frekuensi bunyi akibat gerak relatif antara sumber dan pendengar.',
                        visual: 'f_p = [(v ± v_p) / (v ± v_s)] · f_s',
                        tips: '<strong>Tanda Doppler:</strong> Pendengar mendekat (+), Sumber mendekat (-).',
                        contohSoal: 'Ambulans (f_s = 640 Hz) bergerak v_s = 20 m/s mendekati pendengar diam (v_p = 0, v = 340 m/s). Berapa f_p?<br><strong>Jawab:</strong> f_p = [340 / (340 - 20)] × 640 = <strong>680 Hz</strong>.'
                    },
                    {
                        title: '4. Listrik Dinamis & Hukum Kirchhoff (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Hukum Kirchhoff I (Arus Masuk = Arus Keluar). Hukum Kirchhoff II (ΣE + Σ(I·R) = 0 pada loop tertutup).',
                        visual: 'Seri: R_total = R₁ + R₂  |  Paralel: 1/R_total = 1/R₁ + 1/R₂',
                        tips: 'Jika hasil arus I bernilai negatif, artinya arah arus sebenarnya berlawanan dengan arah pemisalan loop.',
                        contohSoal: 'R₁ = 3 Ω dan R₂ = 6 Ω dirangkai paralel disambung baterai 12 V. Berapa arus total?<br><strong>Jawab:</strong> R_p = (3×6)/(3+6) = 2 Ω. Arus I = V / R_p = 12 / 2 = <strong>6 Ampere</strong>.'
                    }
                ],
                'kim': [
                    {
                        title: '1. Stoikiometri & Konsep Mol (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Mol adalah satuan jumlah zat. 1 mol = 6,02 × 10²³ partikel. Hubungan massa, volume STP, dan molaritas.',
                        visual: 'n = m / Mr  |  V_STP = n × 22,4 L  |  Molaritas M = n / V(L)',
                        tips: 'Bagi mol zat dengan koefisien reaksinya. Nilai terkecil adalah Pereaksi Pembatas.',
                        contohSoal: 'Hitung volume 0,25 mol gas O₂ pada keadaan STP.<br><strong>Jawab:</strong> V = 0,25 × 22,4 = <strong>5,6 Liter</strong>.'
                    },
                    {
                        title: '2. Termokimia & Hukum Hess (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Reaksi Eksoterm (ΔH < 0) vs Endoterm (ΔH > 0). Hukum Hess menyatakan ΔH tidak bergantung pada tahapan reaksi.',
                        visual: 'ΔH_reaksi = Σ ΔH°f(produk) - Σ ΔH°f(pereaksi)',
                        tips: 'Jika reaksi dibalik, tanda ΔH dibalik. Jika reaksi dikali n, nilai ΔH dikali n.',
                        contohSoal: 'Kalor pembentukan ΔH°f CO₂ = -393,5 kJ/mol. Pembakaran 12 gram C (Ar = 12) melepas kalor berapa?<br><strong>Jawab:</strong> n = 12/12 = 1 mol. Kalor = <strong>393,5 kJ</strong>.'
                    },
                    {
                        title: '3. Kesetimbangan Kimia & Asas Le Chatelier (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Reaksi bolak-balik mencapai kesetimbangan saat laju reaksi maju = laju reaksi balik. Pergeseran dipengaruhi konsentrasi, suhu, tekanan, dan volume.',
                        visual: 'K_c = [Produk]ⁿ / [Pereaksi]ᵐ  |  Hanya wujud Gas (g) dan Larutan (aq)',
                        tips: 'Jika suhu dinaikkan, kesetimbangan bergeser ke arah reaksi Endoterm (ΔH positif).',
                        contohSoal: 'Reaksi N₂ + 3H₂ ⇌ 2NH₃ (ΔH = -92 kJ). Agar NH₃ makin banyak, suhu harus?<br><strong>Jawab:</strong> Diturunkan (karena reaksi pembentukan NH₃ eksoterm).'
                    },
                    {
                        title: '4. Reaksi Redoks & Sel Volta (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Redoks adalah reaksi serah terima elektron. Sel Volta mengubah energi kimia menjadi listrik secara spontan (E°sel > 0).',
                        visual: 'KRAO: Katoda Reduksi (Kutub +) | Anoda Oksidasi (Kutub -)  |  E°sel = E°katoda - E°anoda',
                        tips: '<strong>Jembatan Keledai:</strong> KRAO (Katoda Reduksi, Anoda Oksidasi). Logam yang E° lebih positif berada di Katoda.',
                        contohSoal: 'Diketahui E° Zn²⁺/Zn = -0,76 V dan E° Cu²⁺/Cu = +0,34 V. Hitung E°sel.<br><strong>Jawab:</strong> E°sel = +0,34 - (-0,76) = <strong>+1,10 Volt</strong>.'
                    }
                ],
                'bio': [
                    {
                        title: '1. Biologi Sel & Transpor Membran (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Membran sel bersifat semipermeabel. Transpor Pasif (Difusi, Osmosis) tanpa ATP; Transpor Aktif butuh ATP.',
                        visual: 'Osmosis: Pelarut (air) bergerak dari hipotonis (encer) ke hipertonis (pekat)',
                        tips: 'Sel darah merah di larutan hipertonis akan mengalami Krenasi (pengerutan sel).',
                        contohSoal: 'Mengapa sel tumbuhan di larutan hipotonis tidak pecah?<br><strong>Jawab:</strong> Karena sel tumbuhan memiliki Dinding Sel yang kuat (mengalami Turgid).'
                    },
                    {
                        title: '2. Metabolisme: Katabolisme & Anabolisme (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Katabolisme memecah senyawa kompleks (Respirasi Aerob 36-38 ATP). Anabolisme menyusun senyawa (Fotosintesis).',
                        visual: 'Fotosintesis: Reaksi Terang (Tilakoid → ATP, NADPH, O₂) + Reaksi Gelap (Stroma → Glukosa)',
                        tips: 'Penerima elektron terakhir pada respirasi aerob adalah Oksigen (O₂), membentuk H₂O.',
                        contohSoal: 'Di manakah tempat berlangsungnya Siklus Calvin (Reaksi Gelap Fotosintesis)?<br><strong>Jawab:</strong> Di dalam <strong>Stroma</strong> kloroplas.'
                    },
                    {
                        title: '3. Genetika & Persilangan Hukum Mendel (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'DNA membawa kode genetik. Monohibrid dominan penuh F2 = 3 : 1; Dihibrid = 9 : 3 : 3 : 1.',
                        visual: 'Pasangan Basa DNA: Adenin - Timin (2 ikatan H)  |  Guanin - Sitosin (3 ikatan H)',
                        tips: 'Makin banyak ikatan G-C, pita DNA makin stabil karena 3 ikatan hidrogen.',
                        contohSoal: 'Dihibrid AaBb disilangkan sesamanya. Berapa peluang keturunan homozigot resesif (aabb)?<br><strong>Jawab:</strong> (1/4) × (1/4) = <strong>1/16</strong>.'
                    }
                ],
                'eko': [
                    {
                        title: '1. Kelangkaan & Biaya Peluang / Opportunity Cost (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Biaya Peluang adalah nilai kesempatan terbaik yang dikorbankan karena memilih alternatif lain.',
                        visual: 'Biaya Peluang = Nilai Alternatif Terbaik yang Tidak Dipilih',
                        tips: 'Biaya peluang tidak dijumlahkan, melainkan diambil dari nilai SATU opsi tertinggi.',
                        contohSoal: 'Budi memilih kuliah. Opsi kerja dilepas: Staf (4jt) atau Sales (4.5jt). Biaya peluang?<br><strong>Jawab:</strong> <strong>Rp 4.500.000</strong>.'
                    },
                    {
                        title: '2. Keseimbangan Pasar & Elastisitas (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Keseimbangan pasar terjadi saat Q_d = Q_s. Elastisitas mengukur kepekaan perubahan jumlah akibat perubahan harga.',
                        visual: 'Q_d = Q_s  |  Elastis (E > 1), Inelastis (E < 1), Uniter (E = 1)',
                        tips: 'Barang kebutuhan pokok (beras, obat) umumnya bersifat Inelastis (E < 1).',
                        contohSoal: 'Q_d = 20 - 2P dan Q_s = -4 + 2P. Hitung harga keseimbangan P_e.<br><strong>Jawab:</strong> 20 - 2P = -4 + 2P ⇒ 4P = 24 ⇒ P_e = <strong>6</strong>.'
                    }
                ],
                'sos': [
                    {
                        title: '1. Sosiologi Sebagai Ilmu & Ciri-Cirinya (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '4 Ciri Sosiologi: Empiris, Teoritis, Kumulatif, dan Non-Etis (objektif, tidak menilai baik/buruk moral).',
                        visual: 'Non-Etis = Menganalisis fakta tanpa menghakimi secara etika',
                        tips: 'Jika soal membahas peneliti mengkaji motif kejahatan tanpa menyalahkan pelaku, cirinya Non-Etis.',
                        contohSoal: 'Peneliti mengkaji prostitusi secara ilmiah tanpa menghakimi para pelaku. Ciri sosiologinya?<br><strong>Jawab:</strong> Ciri <strong>Non-Etis</strong>.'
                    }
                ],
                'geo': [
                    {
                        title: '1. Konsep & Prinsip Geografi (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '4 Prinsip Geografi: Distribusi, Interelasi (sebab-akibat), Deskripsi, dan Korologi.',
                        visual: 'Prinsip Interelasi = Keterkaitan hubungan sebab-akibat fenomena geosfer',
                        tips: 'Bencana tanah longsor akibat penggundulan hutan di lereng dianalisis dengan Prinsip Interelasi.',
                        contohSoal: 'Banjir Jakarta akibat rusaknya kawasan resapan Bogor. Prinsip geografi?<br><strong>Jawab:</strong> <strong>Prinsip Interelasi</strong>.'
                    }
                ],
                'lit': [
                    {
                        title: '1. Penalaran Logis, Silogisme & Modus Tollens (UTBK)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Penalaran deduktif mengambil kesimpulan khusus dari premis umum.',
                        visual: 'Modus Ponens: P→Q, P ⇒ Q  |  Modus Tollens: P→Q, ~Q ⇒ ~P  |  Silogisme: P→Q, Q→R ⇒ P→R',
                        tips: 'Hati-hati jepakan logika: P → Q TIDAK BISA disimpulkan ~P → ~Q atau Q → P!',
                        contohSoal: 'Premis 1: Jika belajar rajin, lulus UTBK. Premis 2: Budi tidak lulus UTBK. Kesimpulan?<br><strong>Jawab:</strong> Budi tidak belajar rajin (Modus Tollens).'
                    }
                ]
            },
            simulasiBank: {
                'utbk-pk': {
                    title: 'UTBK SNBT - Pengetahuan Kuantitatif (PK)',
                    durasiMinutes: 10,
                    soal: [
                        {
                            id: 'pk_q1',
                            pertanyaan: 'Diketahui persamaan kuadrat x² - (k + 2)x + 16 = 0 memiliki dua akar real positif yang sama (kembar). Nilai k yang memenuhi adalah...',
                            pilihan: ['A. 6 atau -10', 'B. 6 saja', 'C. 8 atau -8', 'D. 10 saja', 'E. -6 saja'],
                            kunci: 'B. 6 saja',
                            solusiLengkap: '1. Syarat kembar: D = b² - 4ac = 0 ⇒ (-(k+2))² - 64 = 0 ⇒ k+2 = ±8 ⇒ k = 6 atau -10.<br>2. Syarat akar positif: x₁+x₂ = k+2 > 0 ⇒ 6+2 = 8 > 0 (Memenuhi k=6).'
                        },
                        {
                            id: 'pk_q2',
                            pertanyaan: 'Jika 3ⁿ⁺¹ + 3ⁿ = 36, maka nilai dari 2ⁿ adalah...',
                            pilihan: ['A. 2', 'B. 4', 'C. 8', 'D. 16', 'E. 32'],
                            kunci: 'B. 4',
                            solusiLengkap: '3ⁿ(3 + 1) = 36 ⇒ 3ⁿ(4) = 36 ⇒ 3ⁿ = 9 ⇒ n = 2. Maka 2ⁿ = 2² = 4.'
                        },
                        {
                            id: 'pk_q3',
                            pertanyaan: 'Jika ᵃlog 2 = x dan ᵃlog 3 = y, maka nilai dari ᵃlog 18 adalah...',
                            pilihan: ['A. x + y', 'B. x + 2y', 'C. 2x + y', 'D. x² + y', 'E. x · y²'],
                            kunci: 'B. x + 2y',
                            solusiLengkap: 'ᵃlog 18 = ᵃlog(2 × 3²) = ᵃlog 2 + 2 · ᵃlog 3 = x + 2y.'
                        },
                        {
                            id: 'pk_q4',
                            pertanyaan: 'Nilai dari lim (x→2) (x² - 4) / (x - 2) adalah...',
                            pilihan: ['A. 0', 'B. 2', 'C. 4', 'D. 8', 'E. Tidak terdefinisi'],
                            kunci: 'C. 4',
                            solusiLengkap: 'Bentuk 0/0. Aturan L\'Hopital: turunkan pembilang (2x) dan penyebut (1). lim (x→2) (2x / 1) = 2(2) = 4.'
                        },
                        {
                            id: 'pk_q5',
                            pertanyaan: 'Luas daerah yang dibatasi oleh parabola y = x² dan garis y = 4 adalah...',
                            pilihan: ['A. 16/3 satuan', 'B. 32/3 satuan', 'C. 64/3 satuan', 'D. 8 satuan', 'E. 12 satuan'],
                            kunci: 'B. 32/3 satuan',
                            solusiLengkap: 'Titik potong x² = 4 ⇒ x = -2 sampai x = 2. Luas = ∫[-2,2] (4 - x²) dx = [4x - x³/3] limit -2 sampai 2 = (8 - 8/3) - (-8 + 8/3) = 16 - 16/3 = 32/3.'
                        }
                    ]
                },
                'utbk-pu': {
                    title: 'UTBK SNBT - Penalaran Umum & Logika (PU)',
                    durasiMinutes: 10,
                    soal: [
                        {
                            id: 'pu_q1',
                            pertanyaan: 'Semua peserta tryout membawa kartu ujian. Sebagian peserta tryout menggunakan kemeja putih. Kesimpulan yang tepat adalah...',
                            pilihan: [
                                'A. Semua peserta tryout berkemeja putih membawa kartu ujian',
                                'B. Sebagian peserta tryout yang membawa kartu ujian berkemeja putih',
                                'C. Semua peserta tryout tidak berkemeja putih',
                                'D. Peserta yang membawa kartu ujian pasti tidak berkemeja putih',
                                'E. Tidak ada kesimpulan yang dapat ditarik'
                            ],
                            kunci: 'B. Sebagian peserta tryout yang membawa kartu ujian berkemeja putih',
                            solusiLengkap: 'Karena SEMUA peserta membawa kartu ujian, maka SEBAGIAN peserta berkemeja putih pasti membawa kartu ujian.'
                        },
                        {
                            id: 'pu_q2',
                            pertanyaan: 'Jika hari hujan, maka jalanan licin. Hari ini jalanan tidak licin. Kesimpulan yang sah adalah...',
                            pilihan: ['A. Hari ini hujan', 'B. Hari ini tidak hujan', 'C. Hari ini mendung', 'D. Jalanan kering karena hujan', 'E. Tidak dapat disimpulkan'],
                            kunci: 'B. Hari ini tidak hujan',
                            solusiLengkap: 'Modus Tollens: P → Q, ~Q ⇒ ~P. P = Hujan, Q = Licin. Karena ~Q (tidak licin), maka ~P (tidak hujan).'
                        },
                        {
                            id: 'pu_q3',
                            pertanyaan: 'Diketahui barisan angka: 3, 6, 12, 21, 33, ... Angka berikutnya adalah...',
                            pilihan: ['A. 42', 'B. 45', 'C. 48', 'D. 51', 'E. 54'],
                            kunci: 'C. 48',
                            solusiLengkap: 'Pola selisih: +3, +6, +9, +12, ... Selisih berikutnya adalah +15. Maka 33 + 15 = 48.'
                        }
                    ]
                },
                'tka-saintek': {
                    title: 'TKA Saintek - Fisika, Kimia & Biologi HOTS',
                    durasiMinutes: 10,
                    soal: [
                        {
                            id: 'saintek_q1',
                            pertanyaan: 'Benda bermassa 2 kg ditarik gaya F = 20 N sudut 60° terhadap horizontal pada lantai licin. Berapakah percepatan benda?',
                            pilihan: ['A. 5 m/s²', 'B. 10 m/s²', 'C. 5√3 m/s²', 'D. 20 m/s²', 'E. 10√3 m/s²'],
                            kunci: 'A. 5 m/s²',
                            solusiLengkap: 'F_x = F cos 60° = 20 (0,5) = 10 N. a = F_x / m = 10 / 2 = 5 m/s².'
                        },
                        {
                            id: 'saintek_q2',
                            pertanyaan: 'Larutan HCl 0,01 M memiliki volume 100 mL. Nilai pH larutan tersebut adalah...',
                            pilihan: ['A. 1', 'B. 2', 'C. 3', 'D. 12', 'E. 13'],
                            kunci: 'B. 2',
                            solusiLengkap: 'HCl asam kuat valensi 1. [H⁺] = 10⁻² M. pH = -log(10⁻²) = 2.'
                        },
                        {
                            id: 'saintek_q3',
                            pertanyaan: 'Pada katode sel elektrolisis larutan CuSO₄ dengan elektrode karbon (C), zat yang dihasilkan adalah...',
                            pilihan: ['A. Gas Oksigen', 'B. Gas Hidrogen', 'C. Endapan Logam Tembaga (Cu)', 'D. Gas Klorin', 'E. Larutan Asam Sulfat'],
                            kunci: 'C. Endapan Logam Tembaga (Cu)',
                            solusiLengkap: 'Di katode terjadi reduksi kation. Kation Cu²⁺ memiliki E° lebih positif daripada air, sehingga Cu²⁺ tereduksi menjadi logam Cu (Cu²⁺ + 2e⁻ → Cu).'
                        }
                    ]
                },
                'tka-soshum': {
                    title: 'TKA Soshum - Ekonomi, Sosiologi & Geografi',
                    durasiMinutes: 10,
                    soal: [
                        {
                            id: 'soshum_q1',
                            pertanyaan: 'Apabila pemerintah menetapkan harga maksimum (Ceiling Price) di bawah harga keseimbangan pasar, dampak langsung yang terjadi adalah...',
                            pilihan: ['A. Kelebihan penawaran (Excess Supply)', 'B. Kelebihan permintaan / Kelangkaan barang (Excess Demand)', 'C. Harga pasar melonjak', 'D. Produsen mengalami surplus besar', 'E. Kurva penawaran bergeser ke kanan'],
                            kunci: 'B. Kelebihan permintaan / Kelangkaan barang (Excess Demand)',
                            solusiLengkap: 'Harga maksimum di bawah pasar membuat Qd naik (pembeli ingin beli banyak) tetapi Qs turun (penjual enggan menjual), memicu Excess Demand.'
                        },
                        {
                            id: 'soshum_q2',
                            pertanyaan: 'Peneliti sosiologi menganalisis fenomena kemiskinan perkotaan tanpa menghakimi secara moral baik atau buruknya objek. Ciri sosiologi ini adalah...',
                            pilihan: ['A. Empiris', 'B. Kumulatif', 'C. Non-Etis', 'D. Teoritis', 'E. Spekulatif'],
                            kunci: 'C. Non-Etis',
                            solusiLengkap: 'Ciri Non-Etis berarti sosiologi menjelaskan fakta sosial secara objektif tanpa memberikan penilaian etis/moral.'
                        }
                    ]
                }
            }
        };

        // UI View Switcher Engine
        function switchView(viewName) {
            state.activeView = viewName;

            ['home', 'materi', 'utbk', 'flashcards', 'riwayat'].forEach(v => {
                const el = document.getElementById(`nav-${v}`);
                if (el) {
                    el.className = v === viewName 
                        ? "px-4 py-2.5 rounded-xl text-white bg-purple-600 font-bold shadow-md shadow-purple-600/30 transition flex items-center gap-1.5"
                        : "px-4 py-2.5 rounded-xl text-slate-300 hover:text-white font-medium transition flex items-center gap-1.5";
                }

                const mobEl = document.getElementById(`mob-${v}`);
                if (mobEl) {
                    mobEl.className = v === viewName 
                        ? "flex flex-col items-center gap-1 text-purple-400 font-bold"
                        : "flex flex-col items-center gap-1 text-slate-400 font-medium";
                }
            });

            const content = document.getElementById('app-content');
            if (viewName === 'home') content.innerHTML = renderHome();
            else if (viewName === 'materi') content.innerHTML = renderMateriScreen();
            else if (viewName === 'utbk') content.innerHTML = renderUTBKScreen();
            else if (viewName === 'flashcards') content.innerHTML = renderFlashcardScreen();
            else if (viewName === 'riwayat') {
                content.innerHTML = renderRiwayatScreen();
                if (state.attempts.length > 0) openDetailRiwayat(state.attempts.length - 1);
            }

            lucide.createIcons();
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // Global Search Logic
        function handleGlobalSearch(query) {
            const popover = document.getElementById('search-results-popover');
            if (!query || query.trim().length < 2) {
                popover.classList.add('hidden');
                return;
            }

            const q = query.toLowerCase().trim();
            let matches = [];

            db.mapel.forEach(m => {
                const list = db.materiDetails[m.id] || [];
                list.forEach(mat => {
                    if (mat.title.toLowerCase().includes(q) || mat.summary.toLowerCase().includes(q)) {
                        matches.push({ mapelId: m.id, mapelNama: m.nama, title: mat.title });
                    }
                });
            });

            if (matches.length === 0) {
                popover.innerHTML = `<div class="p-3 text-xs text-slate-400 text-center">Tidak ditemukan materi dengan kata kunci "${query}"</div>`;
            } else {
                popover.innerHTML = matches.map(res => `
                    <div onclick="selectSearchResult('${res.mapelId}')" class="p-3 hover:bg-slate-800/80 rounded-xl cursor-pointer transition border-b border-slate-800/60 last:border-0">
                        <span class="text-[10px] font-bold text-purple-400 uppercase tracking-wider block">${res.mapelNama}</span>
                        <span class="text-xs text-white font-semibold block mt-0.5">${res.title}</span>
                    </div>
                `).join('');
            }
            popover.classList.remove('hidden');
        }

        function selectSearchResult(mapelId) {
            document.getElementById('search-results-popover').classList.add('hidden');
            document.getElementById('global-search').value = '';
            state.selectedSubject = mapelId;
            switchView('materi');
            openDetailMapel(mapelId);
        }

        // Render Home View
        function renderHome() {
            return `
                <!-- Hero Banner -->
                <div class="relative rounded-3xl gradient-brand p-8 sm:p-12 overflow-hidden border border-purple-500/30 shadow-2xl mb-12">
                    <div class="absolute -right-20 -bottom-20 w-96 h-96 bg-purple-600/20 rounded-full blur-3xl pointer-events-none"></div>
                    <div class="relative z-10 max-w-3xl">
                        <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-purple-500/10 border border-purple-500/30 text-purple-300 text-xs font-semibold mb-6">
                            <i data-lucide="sparkles" class="w-4 h-4 text-purple-400"></i>
                            <span>Nihiluxxy AI Pro 2026 • Penjelasan Konsep Intuitif & Akurat</span>
                        </div>
                        <h1 class="text-3xl sm:text-5xl font-black text-white tracking-tight mb-4 leading-tight">
                            Kuasai Seluruh Konsep SMA & Taklukkan <span class="bg-clip-text text-transparent gradient-accent">UTBK SNBT 2026</span>.
                        </h1>
                        <p class="text-slate-300 text-xs sm:text-sm mb-8 leading-relaxed">
                            Modul SMA (Kelas 10–12) komprehensif, rumus visual, tips instan, serta pengerjaan soal HOTS terperinci dibantu oleh **Nihiluxxy AI Tutor v5.0**.
                        </p>
                        <div class="flex flex-wrap gap-4">
                            <button onclick="switchView('materi')" class="gradient-accent text-white font-extrabold px-6 py-3.5 rounded-2xl shadow-lg shadow-purple-500/25 hover:opacity-95 transition flex items-center gap-2 text-xs sm:text-sm">
                                <i data-lucide="book-open" class="w-4 h-4"></i> Pelajari Modul Terperinci
                            </button>
                            <button onclick="toggleAiModal()" class="bg-slate-900/90 border border-purple-500/40 text-purple-200 font-extrabold px-6 py-3.5 rounded-2xl hover:bg-slate-800 transition flex items-center gap-2 text-xs sm:text-sm">
                                <i data-lucide="bot" class="w-4 h-4 text-purple-400"></i> Tanya AI Tutor
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Stats Cards -->
                <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-12">
                    <div class="glass-card p-5 rounded-2xl text-center border-purple-500/20">
                        <span class="text-2xl font-black text-purple-400 font-mono">8+</span>
                        <span class="text-xs text-slate-400 block mt-1 font-semibold">Mata Pelajaran SMA</span>
                    </div>
                    <div class="glass-card p-5 rounded-2xl text-center border-purple-500/20">
                        <span class="text-2xl font-black text-emerald-400 font-mono">100%</span>
                        <span class="text-xs text-slate-400 block mt-1 font-semibold">K13 & Merdeka Active</span>
                    </div>
                    <div class="glass-card p-5 rounded-2xl text-center border-purple-500/20">
                        <span class="text-2xl font-black text-amber-400 font-mono">HOTS</span>
                        <span class="text-xs text-slate-400 block mt-1 font-semibold">Pembahasan Akurat</span>
                    </div>
                    <div class="glass-card p-5 rounded-2xl text-center border-purple-500/20">
                        <span class="text-2xl font-black text-cyan-400 font-mono">2026</span>
                        <span class="text-xs text-slate-400 block mt-1 font-semibold">AI Assistant Integrated</span>
                    </div>
                </div>

                <!-- Subject Grid Section -->
                <div class="mb-12">
                    <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4 mb-6">
                        <div>
                            <h2 class="text-2xl font-black text-white tracking-tight">Mata Pelajaran SMA</h2>
                            <p class="text-slate-400 text-xs sm:text-sm">Pilih kurikulum untuk melihat cakupan materi</p>
                        </div>
                        <div class="bg-slate-900/90 p-1 rounded-2xl border border-slate-800 flex gap-1 text-xs font-bold">
                            <button onclick="setKurikulum('Merdeka')" class="px-4 py-2 rounded-xl transition ${state.selectedKurikulum === 'Merdeka' ? 'bg-purple-600 text-white shadow-md' : 'text-slate-400 hover:text-white'}">Kurikulum Merdeka</button>
                            <button onclick="setKurikulum('K13')" class="px-4 py-2 rounded-xl transition ${state.selectedKurikulum === 'K13' ? 'bg-purple-600 text-white shadow-md' : 'text-slate-400 hover:text-white'}">Kurikulum 2013</button>
                        </div>
                    </div>

                    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-5">
                        ${db.mapel.map(m => `
                            <div class="glass-card border border-slate-800 hover:border-purple-500/60 p-5 rounded-2xl transition duration-300 hover:-translate-y-1 group cursor-pointer shadow-lg relative overflow-hidden" onclick="openDetailMapel('${m.id}')">
                                <div class="w-12 h-12 rounded-2xl bg-gradient-to-br ${m.color} flex items-center justify-center text-white mb-4 shadow-lg group-hover:scale-110 transition duration-300">
                                    <i data-lucide="${m.icon}"></i>
                                </div>
                                <h3 class="font-extrabold text-white text-base mb-1 group-hover:text-purple-300 transition">${m.nama}</h3>
                                <p class="text-[11px] text-purple-400 font-semibold mb-4 leading-tight">
                                    ${state.selectedKurikulum === 'Merdeka' ? m.merdeka : m.k13}
                                </p>
                                <div class="flex items-center justify-between text-xs text-slate-400 pt-3 border-t border-slate-800/80">
                                    <span class="font-bold text-[11px]">Buka Modul Belajar</span>
                                    <i data-lucide="arrow-right" class="w-4 h-4 text-purple-400 group-hover:translate-x-1 transition"></i>
                                </div>
                            </div>
                        `).join('')}
                    </div>
                </div>

                <!-- Last Attempt Card -->
                <div class="glass-card border border-slate-800 rounded-3xl p-6 sm:p-8 shadow-xl">
                    <div class="flex items-center justify-between mb-4">
                        <div class="flex items-center gap-3">
                            <div class="p-2.5 rounded-2xl bg-purple-500/10 text-purple-400 border border-purple-500/20">
                                <i data-lucide="history" class="w-5 h-5"></i>
                            </div>
                            <div>
                                <h3 class="font-extrabold text-white text-base">Riwayat Simulasi Terakhir</h3>
                                <p class="text-xs text-slate-400">Evaluasi & pelajari pembahasan akurat dari pengerjaan Anda</p>
                            </div>
                        </div>
                        <button onclick="switchView('riwayat')" class="text-xs text-purple-400 hover:text-purple-300 font-bold flex items-center gap-1">
                            <span>Lihat Semua</span>
                            <i data-lucide="chevron-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                    ${renderLastAttemptCard()}
                </div>
            `;
        }

        function renderLastAttemptCard() {
            if (state.attempts.length === 0) {
                return `
                    <div class="text-center py-8 text-slate-500 text-xs border border-dashed border-slate-800 rounded-2xl bg-slate-900/40">
                        <i data-lucide="info" class="w-6 h-6 mx-auto mb-2 text-slate-600"></i>
                        Belum ada simulasi yang diselesaikan. Selesaikan simulasi TKA/UTBK untuk mencatat riwayat akurat Anda di sini.
                    </div>
                `;
            }
            const last = state.attempts[state.attempts.length - 1];
            return `
                <div class="bg-slate-900/80 border border-slate-800 p-5 rounded-2xl flex flex-col sm:flex-row justify-between sm:items-center gap-4">
                    <div>
                        <div class="flex items-center gap-2 mb-1.5">
                            <span class="text-[10px] font-extrabold px-2 py-0.5 rounded-full bg-emerald-500/20 text-emerald-300 border border-emerald-500/30">Pengerjaan Terakhir</span>
                            <span class="text-xs text-slate-500 font-mono">${last.tanggal}</span>
                        </div>
                        <h4 class="font-black text-white text-base">${last.judulSimulasi}</h4>
                        <p class="text-xs text-slate-400 mt-1">Akurasi Skor: <span class="text-purple-300 font-bold font-mono">${last.skor}%</span> (${last.benar} dari ${last.totalSoal} Soal Benar)</p>
                    </div>
                    <button onclick="openDetailRiwayat(${state.attempts.length - 1})" class="px-5 py-3 bg-purple-600 hover:bg-purple-500 text-white font-extrabold text-xs rounded-xl transition shadow-lg shadow-purple-600/20 flex items-center justify-center gap-2">
                        <i data-lucide="file-search" class="w-4 h-4"></i> Lihat Pembahasan Akurat
                    </button>
                </div>
            `;
        }

        function setKurikulum(k) {
            state.selectedKurikulum = k;
            switchView('home');
        }

        // Render Modul Materi Screen
        function renderMateriScreen() {
            return `
                <div class="mb-8">
                    <h1 class="text-3xl font-black text-white tracking-tight">Modul Pembelajaran SMA (Kelas 10-12)</h1>
                    <p class="text-slate-400 text-xs sm:text-sm mt-1">Penjelasan mendalam, analogi intuitif, rumus visual, tips cepat, dan contoh soal HOTS.</p>
                </div>
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
                    <div class="lg:col-span-4 space-y-3">
                        <h3 class="text-xs uppercase tracking-wider font-extrabold text-purple-400 px-1">Pilih Mata Pelajaran</h3>
                        ${db.mapel.map(m => `
                            <button onclick="openDetailMapel('${m.id}')" id="mapel-btn-${m.id}" class="w-full text-left p-4 rounded-2xl bg-slate-900/60 border border-slate-800 hover:bg-slate-800 hover:border-purple-500/50 transition flex items-center gap-3.5 group">
                                <div class="w-10 h-10 rounded-xl bg-gradient-to-br ${m.color} flex items-center justify-center text-white font-bold text-xs shadow-md group-hover:scale-105 transition">
                                    <i data-lucide="${m.icon}" class="w-5 h-5"></i>
                                </div>
                                <div class="flex flex-col">
                                    <span class="font-extrabold text-sm text-slate-200 group-hover:text-purple-300 transition">${m.nama}</span>
                                    <span class="text-[10px] text-slate-500 font-medium">Sub-materi HOTS Lengkap</span>
                                </div>
                            </button>
                        `).join('')}
                    </div>
                    <div id="materi-reader" class="lg:col-span-8 glass-card border border-slate-800 rounded-3xl p-6 sm:p-8 shadow-2xl">
                        <!-- Injected by JS -->
                    </div>
                </div>
            `;
        }

        function openDetailMapel(mapelId) {
            state.selectedSubject = mapelId;
            if (state.activeView !== 'materi') switchView('materi');

            db.mapel.forEach(m => {
                const btn = document.getElementById(`mapel-btn-${m.id}`);
                if (btn) {
                    btn.className = m.id === mapelId
                        ? "w-full text-left p-4 rounded-2xl bg-slate-800 border border-purple-500/80 flex items-center gap-3.5 group shadow-lg"
                        : "w-full text-left p-4 rounded-2xl bg-slate-900/60 border border-slate-800 hover:bg-slate-800 transition flex items-center gap-3.5 group";
                }
            });

            const mapel = db.mapel.find(m => m.id === mapelId);
            const materiList = db.materiDetails[mapelId] || [];

            const reader = document.getElementById('materi-reader');
            if (reader) {
                reader.innerHTML = `
                    <div class="flex items-center justify-between pb-6 border-b border-slate-800 mb-8">
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-2xl bg-gradient-to-br ${mapel.color} flex items-center justify-center text-white font-bold shadow-lg">
                                <i data-lucide="${mapel.icon}"></i>
                            </div>
                            <div>
                                <h2 class="text-2xl font-black text-white tracking-tight">${mapel.nama}</h2>
                                <p class="text-xs text-purple-400 font-extrabold mt-0.5">Kurikulum K13 & Merdeka Active</p>
                            </div>
                        </div>
                        <button onclick="askAiAboutSubject('${mapel.nama}')" class="px-3.5 py-2 rounded-xl bg-purple-600/20 border border-purple-500/40 text-purple-300 hover:bg-purple-600 hover:text-white transition text-xs font-bold flex items-center gap-1.5">
                            <i data-lucide="bot" class="w-4 h-4"></i> Tanya AI
                        </button>
                    </div>
                    <div class="space-y-6">
                        ${materiList.map((mat, idx) => `
                            <div class="bg-slate-900/90 border border-slate-800 p-6 rounded-2xl shadow-md">
                                <div class="flex items-center justify-between mb-3">
                                    <span class="text-[10px] font-extrabold uppercase bg-purple-500/20 text-purple-300 px-3 py-1 rounded-full border border-purple-500/30">${mat.kurikulum}</span>
                                    <span class="text-xs text-slate-500 font-mono">Modul Terperinci #${idx + 1}</span>
                                </div>
                                <h3 class="text-lg font-extrabold text-white mb-3">${mat.title}</h3>
                                <div class="text-slate-300 text-xs sm:text-sm mb-4 leading-relaxed">${mat.summary}</div>
                                
                                <div class="bg-slate-950 p-4 rounded-xl font-mono text-xs text-purple-300 mb-4 border border-slate-800 text-center overflow-x-auto">
                                    ${mat.visual}
                                </div>

                                <div class="bg-amber-500/10 border-l-4 border-amber-500 p-4 rounded-r-xl text-xs text-amber-200 mb-4 leading-relaxed">
                                    ${mat.tips}
                                </div>

                                <div class="bg-slate-950/80 border border-slate-800 p-4 rounded-xl text-xs text-slate-300 leading-relaxed mb-4">
                                    <span class="text-emerald-400 font-extrabold block mb-2">📝 Contoh Soal & Pembahasan HOTS:</span>
                                    ${mat.contohSoal}
                                </div>

                                <button onclick="askAiAboutTopic('${mat.title}')" class="w-full py-2.5 bg-slate-800 hover:bg-purple-900/40 border border-slate-700 hover:border-purple-500/50 text-purple-300 text-xs font-bold rounded-xl transition flex items-center justify-center gap-2">
                                    <i data-lucide="sparkles" class="w-3.5 h-3.5"></i> Minta AI Bedah Lebih Dalam Modul Ini
                                </button>
                            </div>
                        `).join('')}
                    </div>
                `;
                lucide.createIcons();
            }
        }

        // Render UTBK Simulation Screen
        function renderUTBKScreen() {
            return `
                <div class="mb-8">
                    <h1 class="text-3xl font-black text-white tracking-tight">Simulasi TKA & UTBK SNBT 2026</h1>
                    <p class="text-slate-400 text-xs sm:text-sm mt-1">Uji pemahaman dengan timer real-time interaktif, penilaian otomatis, & pembahasan terperinci.</p>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div class="glass-card border border-slate-800 p-6 rounded-3xl flex flex-col justify-between shadow-xl">
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-amber-500/20 border border-amber-500/30 text-amber-400 flex items-center justify-center mb-4 font-black">
                                <i data-lucide="calculator" class="w-6 h-6"></i>
                            </div>
                            <span class="text-[10px] uppercase font-extrabold text-amber-400 bg-amber-500/10 px-2.5 py-1 rounded-md border border-amber-500/20">SNBT Standard</span>
                            <h3 class="text-xl font-extrabold text-white mt-3 mb-1">UTBK - Pengetahuan Kuantitatif (PK)</h3>
                            <p class="text-slate-400 text-xs mb-6 leading-relaxed">Uji pemahaman aljabar, kalkulus, logaritma, & geometri HOTS.</p>
                        </div>
                        <button onclick="startSimulasi('utbk-pk')" class="w-full py-3.5 bg-amber-500 hover:bg-amber-400 text-slate-950 font-black text-xs rounded-xl transition shadow-lg shadow-amber-500/20 flex items-center justify-center gap-2">
                            <i data-lucide="play" class="w-4 h-4 fill-current"></i> Mulai Tes (10 Menit)
                        </button>
                    </div>

                    <div class="glass-card border border-slate-800 p-6 rounded-3xl flex flex-col justify-between shadow-xl">
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-cyan-500/20 border border-cyan-500/30 text-cyan-400 flex items-center justify-center mb-4 font-black">
                                <i data-lucide="brain" class="w-6 h-6"></i>
                            </div>
                            <span class="text-[10px] uppercase font-extrabold text-cyan-400 bg-cyan-500/10 px-2.5 py-1 rounded-md border border-cyan-500/20">SNBT Standard</span>
                            <h3 class="text-xl font-extrabold text-white mt-3 mb-1">UTBK - Penalaran Umum (PU)</h3>
                            <p class="text-slate-400 text-xs mb-6 leading-relaxed">Uji logika deduktif, silogisme, pola barisan, & kesimpulan paragraf.</p>
                        </div>
                        <button onclick="startSimulasi('utbk-pu')" class="w-full py-3.5 bg-cyan-500 hover:bg-cyan-400 text-slate-950 font-black text-xs rounded-xl transition shadow-lg shadow-cyan-500/20 flex items-center justify-center gap-2">
                            <i data-lucide="play" class="w-4 h-4 fill-current"></i> Mulai Tes (10 Menit)
                        </button>
                    </div>

                    <div class="glass-card border border-slate-800 p-6 rounded-3xl flex flex-col justify-between shadow-xl">
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-indigo-500/20 border border-indigo-500/30 text-indigo-400 flex items-center justify-center mb-4 font-black">
                                <i data-lucide="zap" class="w-6 h-6"></i>
                            </div>
                            <span class="text-[10px] uppercase font-extrabold text-indigo-400 bg-indigo-500/10 px-2.5 py-1 rounded-md border border-indigo-500/20">TKA High Level</span>
                            <h3 class="text-xl font-extrabold text-white mt-3 mb-1">TKA Saintek - Fisika, Kimia & Bio</h3>
                            <p class="text-slate-400 text-xs mb-6 leading-relaxed">Uji penalaran sains lanjutan: mekanika, sel elektrolisis, & genetika.</p>
                        </div>
                        <button onclick="startSimulasi('tka-saintek')" class="w-full py-3.5 bg-indigo-600 hover:bg-indigo-500 text-white font-black text-xs rounded-xl transition shadow-lg shadow-indigo-600/20 flex items-center justify-center gap-2">
                            <i data-lucide="play" class="w-4 h-4 fill-current"></i> Mulai Tes (10 Menit)
                        </button>
                    </div>

                    <div class="glass-card border border-slate-800 p-6 rounded-3xl flex flex-col justify-between shadow-xl">
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-rose-500/20 border border-rose-500/30 text-rose-400 flex items-center justify-center mb-4 font-black">
                                <i data-lucide="users" class="w-6 h-6"></i>
                            </div>
                            <span class="text-[10px] uppercase font-extrabold text-rose-400 bg-rose-500/10 px-2.5 py-1 rounded-md border border-rose-500/20">TKA High Level</span>
                            <h3 class="text-xl font-extrabold text-white mt-3 mb-1">TKA Soshum - Eko, Sos & Geo</h3>
                            <p class="text-slate-400 text-xs mb-6 leading-relaxed">Uji pemahaman ekonomi ceiling price, sosiologi empiris, & prinsip geografi.</p>
                        </div>
                        <button onclick="startSimulasi('tka-soshum')" class="w-full py-3.5 bg-rose-600 hover:bg-rose-500 text-white font-black text-xs rounded-xl transition shadow-lg shadow-rose-600/20 flex items-center justify-center gap-2">
                            <i data-lucide="play" class="w-4 h-4 fill-current"></i> Mulai Tes (10 Menit)
                        </button>
                    </div>
                </div>
            `;
        }

        // Active Simulation Engine with Timer
        function startSimulasi(simKey) {
            state.activeSimKey = simKey;
            state.currentSimAnswers = {};
            const currentSim = db.simulasiBank[simKey];
            
            state.simTimeLeft = (currentSim.durasiMinutes || 10) * 60;

            const app = document.getElementById('app-content');
            app.innerHTML = `
                <div class="max-w-3xl mx-auto glass-card border border-purple-500/30 p-6 sm:p-8 rounded-3xl shadow-2xl relative">
                    
                    <!-- Timer Header -->
                    <div class="sticky top-24 z-30 bg-slate-900/95 border border-purple-500/40 p-4 rounded-2xl mb-6 backdrop-blur-xl flex items-center justify-between shadow-xl">
                        <div>
                            <span class="text-[10px] font-extrabold text-purple-400 tracking-wider uppercase block">Simulasi Berjalan</span>
                            <h2 class="text-sm sm:text-base font-black text-white">${currentSim.title}</h2>
                        </div>
                        <div class="flex items-center gap-3">
                            <div class="bg-slate-950 border border-slate-700 px-3.5 py-1.5 rounded-xl text-center">
                                <span class="text-[9px] text-slate-400 uppercase font-extrabold block">Sisa Waktu</span>
                                <span id="sim-timer-display" class="text-xs sm:text-sm font-black text-amber-400 font-mono">10:00</span>
                            </div>
                        </div>
                    </div>

                    <div id="quiz-container" class="space-y-8">
                        ${currentSim.soal.map((q, idx) => `
                            <div class="bg-slate-900/90 p-6 rounded-2xl border border-slate-800">
                                <div class="flex items-center justify-between mb-3">
                                    <span class="text-xs font-bold text-purple-400 font-mono">Soal #${idx + 1}</span>
                                    <span class="text-[10px] text-slate-500 font-semibold">Tipe: Pilihan Ganda HOTS</span>
                                </div>
                                <p class="text-sm sm:text-base text-slate-100 font-medium mb-5 leading-relaxed">${q.pertanyaan}</p>
                                <div class="space-y-3">
                                    ${q.pilihan.map(opt => `
                                        <label class="flex items-center p-3.5 rounded-xl border border-slate-800 hover:bg-slate-800/80 hover:border-purple-500/50 transition cursor-pointer group">
                                            <input type="radio" name="question_${q.id}" value="${opt}" onchange="recordAnswer('${q.id}', '${opt}')" class="w-4 h-4 text-purple-600 focus:ring-purple-500 bg-slate-900 border-slate-700">
                                            <span class="ml-3.5 text-xs sm:text-sm text-slate-300 font-medium group-hover:text-white transition">${opt}</span>
                                        </label>
                                    `).join('')}
                                </div>
                            </div>
                        `).join('')}
                    </div>

                    <div class="mt-8 pt-6 border-t border-slate-800 flex justify-between items-center">
                        <button onclick="stopTimerAndExit()" class="px-5 py-2.5 border border-slate-800 text-slate-400 hover:text-white hover:bg-slate-800 text-xs font-extrabold rounded-xl transition">Batal</button>
                        <button onclick="submitSimulasi('${simKey}')" class="px-6 py-3.5 gradient-accent text-white font-black text-xs rounded-xl shadow-lg shadow-purple-500/25 hover:opacity-95 transition flex items-center gap-2">
                            <i data-lucide="check-circle" class="w-4 h-4"></i> Selesaikan Tes
                        </button>
                    </div>
                </div>
            `;
            lucide.createIcons();
            window.scrollTo({ top: 0, behavior: 'smooth' });

            clearInterval(state.simTimerInterval);
            state.simTimerInterval = setInterval(() => {
                state.simTimeLeft--;
                const mins = Math.floor(state.simTimeLeft / 60);
                const secs = state.simTimeLeft % 60;
                const display = `${mins.toString().padStart(2, '0')}:${secs.toString().padStart(2, '0')}`;
                
                const timerEl = document.getElementById('sim-timer-display');
                if (timerEl) {
                    timerEl.innerText = display;
                    if (state.simTimeLeft <= 60) timerEl.className = "text-xs sm:text-sm font-black text-rose-500 animate-pulse font-mono";
                }

                if (state.simTimeLeft <= 0) {
                    clearInterval(state.simTimerInterval);
                    alert('Waktu pengerjaan telah habis! Jawaban Anda akan tersimpan secara otomatis.');
                    submitSimulasi(simKey);
                }
            }, 1000);
        }

        function recordAnswer(qId, val) {
            state.currentSimAnswers[qId] = val;
        }

        function stopTimerAndExit() {
            clearInterval(state.simTimerInterval);
            switchView('utbk');
        }

        function submitSimulasi(simKey) {
            clearInterval(state.simTimerInterval);
            const sim = db.simulasiBank[simKey];
            let benarCount = 0;
            const total = sim.soal.length;

            const reviewDetails = sim.soal.map(q => {
                const userAns = state.currentSimAnswers[q.id] || 'Tidak Dijawab';
                const isCorrect = userAns === q.kunci;
                if (isCorrect) benarCount++;
                return {
                    pertanyaan: q.pertanyaan,
                    jawabanUser: userAns,
                    kunci: q.kunci,
                    isCorrect: isCorrect,
                    solusi: q.solusiLengkap
                };
            });

            const score = Math.round((benarCount / total) * 100);
            const now = new Date();
            const dateStr = now.toLocaleDateString('id-ID', { day: 'numeric', month: 'short', year: 'numeric', hour: '2-digit', minute: '2-digit' }) + ' WIB';

            const attemptRecord = {
                id: 'att_' + Date.now(),
                judulSimulasi: sim.title,
                tanggal: dateStr,
                skor: score,
                benar: benarCount,
                totalSoal: total,
                detail: reviewDetails
            };

            state.attempts.push(attemptRecord);
            localStorage.setItem('nihiluxxy_attempts', JSON.stringify(state.attempts));

            switchView('riwayat');
            openDetailRiwayat(state.attempts.length - 1);
        }

        // Render Interactive Flashcard View
        function renderFlashcardScreen() {
            const card = db.flashcards[state.currentFlashcardIdx];
            return `
                <div class="mb-8 text-center max-w-2xl mx-auto">
                    <span class="text-xs font-extrabold uppercase tracking-widest text-emerald-400 bg-emerald-500/10 px-3 py-1 rounded-full border border-emerald-500/20 mb-2 inline-block">Flashcards Pintar</span>
                    <h1 class="text-3xl font-black text-white tracking-tight">Latihan Cepat Hafalan & Konsep</h1>
                    <p class="text-slate-400 text-xs sm:text-sm mt-1">Uji ingatan intuitif Anda sebelum menghadapi ujian asli.</p>
                </div>

                <div class="max-w-xl mx-auto">
                    <div id="flashcard-box" onclick="flipFlashcard()" class="glass-card border border-purple-500/40 rounded-3xl p-8 sm:p-12 min-h-[260px] flex flex-col justify-between items-center text-center cursor-pointer shadow-2xl transition duration-500 transform hover:scale-[1.02]">
                        <span class="text-[10px] font-black uppercase text-purple-400 font-mono tracking-widest">${card.mapel} • Klik Kartu Untuk Membalik</span>
                        
                        <div id="flashcard-content" class="my-auto py-4">
                            <p class="text-base sm:text-lg font-bold text-white leading-relaxed">${card.pertanyaan}</p>
                        </div>

                        <span class="text-[11px] text-slate-500 font-bold">Kartu ${state.currentFlashcardIdx + 1} dari ${db.flashcards.length}</span>
                    </div>

                    <div class="flex justify-between items-center mt-6">
                        <button onclick="prevFlashcard()" class="px-5 py-2.5 bg-slate-900 border border-slate-800 text-slate-300 hover:text-white rounded-xl text-xs font-bold transition flex items-center gap-1.5">
                            <i data-lucide="arrow-left" class="w-4 h-4"></i> Sebelumnya
                        </button>
                        <button onclick="nextFlashcard()" class="px-5 py-2.5 bg-purple-600 hover:bg-purple-500 text-white rounded-xl text-xs font-bold transition flex items-center gap-1.5 shadow-lg shadow-purple-600/25">
                            Selanjutnya <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>
            `;
        }

        let isCardFlipped = false;
        function flipFlashcard() {
            const card = db.flashcards[state.currentFlashcardIdx];
            const content = document.getElementById('flashcard-content');
            if (!content) return;

            isCardFlipped = !isCardFlipped;
            if (isCardFlipped) {
                content.innerHTML = `<p class="text-sm sm:text-base font-semibold text-emerald-300 leading-relaxed bg-emerald-950/40 p-4 rounded-2xl border border-emerald-500/30">💡 ${card.jawaban}</p>`;
            } else {
                content.innerHTML = `<p class="text-base sm:text-lg font-bold text-white leading-relaxed">${card.pertanyaan}</p>`;
            }
        }

        function nextFlashcard() {
            isCardFlipped = false;
            state.currentFlashcardIdx = (state.currentFlashcardIdx + 1) % db.flashcards.length;
            switchView('flashcards');
        }

        function prevFlashcard() {
            isCardFlipped = false;
            state.currentFlashcardIdx = (state.currentFlashcardIdx - 1 + db.flashcards.length) % db.flashcards.length;
            switchView('flashcards');
        }

        // Render History View
        function renderRiwayatScreen() {
            if (state.attempts.length === 0) {
                return `
                    <div class="mb-8">
                        <h1 class="text-3xl font-black text-white tracking-tight">Riwayat Pengerjaan</h1>
                        <p class="text-slate-400 text-xs sm:text-sm mt-1">Daftar evaluasi simulasi dan pembahasan akurat Anda.</p>
                    </div>
                    <div class="glass-card border border-slate-800 rounded-3xl p-12 text-center text-slate-500 shadow-xl">
                        <div class="w-16 h-16 rounded-full bg-slate-900 border border-slate-800 flex items-center justify-center mx-auto mb-4 text-slate-600">
                            <i data-lucide="history" class="w-8 h-8"></i>
                        </div>
                        <p class="text-base font-extrabold text-slate-300">Belum Ada Riwayat Tersimpan</p>
                        <p class="text-xs text-slate-500 mt-1 mb-6">Selesaikan simulasi TKA/UTBK untuk mencatat riwayat jawaban akurat Anda di sini.</p>
                        <button onclick="switchView('utbk')" class="px-6 py-3 bg-purple-600 hover:bg-purple-500 text-white font-extrabold text-xs rounded-xl transition shadow-lg shadow-purple-600/25">
                            Mulai Simulasi Sekarang
                        </button>
                    </div>
                `;
            }

            return `
                <div class="mb-8 flex flex-col sm:flex-row sm:items-center justify-between gap-4">
                    <div>
                        <h1 class="text-3xl font-black text-white tracking-tight">Riwayat & Pembahasan Akurat</h1>
                        <p class="text-slate-400 text-xs sm:text-sm mt-1">Pilih pengerjaan di bawah untuk memeriksa kunci jawaban & cara pengerjaan terperinci.</p>
                    </div>
                    <button onclick="clearHistory()" class="px-4 py-2 border border-rose-500/30 text-rose-400 hover:bg-rose-500/10 text-xs font-bold rounded-xl transition self-start sm:self-auto flex items-center gap-1.5">
                        <i data-lucide="trash-2" class="w-4 h-4"></i> Hapus Semua Riwayat
                    </button>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
                    <div class="lg:col-span-4 space-y-3">
                        <h3 class="text-xs uppercase tracking-wider font-extrabold text-purple-400 px-1">Daftar Pengerjaan</h3>
                        ${state.attempts.map((att, idx) => `
                            <button onclick="openDetailRiwayat(${idx})" id="att-btn-${idx}" class="w-full text-left p-4 rounded-2xl bg-slate-900/60 border border-slate-800 hover:bg-slate-800 transition flex items-center justify-between group">
                                <div>
                                    <span class="text-[10px] text-slate-500 font-mono block">${att.tanggal}</span>
                                    <h4 class="font-extrabold text-xs sm:text-sm text-white group-hover:text-purple-300 transition mt-0.5">${att.judulSimulasi}</h4>
                                </div>
                                <span class="text-sm font-black text-purple-300 font-mono bg-purple-500/10 border border-purple-500/20 px-2.5 py-1 rounded-lg">${att.skor}%</span>
                            </button>
                        `).join('')}
                    </div>

                    <div id="riwayat-detail-container" class="lg:col-span-8 glass-card border border-slate-800 rounded-3xl p-6 sm:p-8 shadow-2xl">
                        <!-- History details injected here -->
                    </div>
                </div>
            `;
        }

        function openDetailRiwayat(index) {
            state.attempts.forEach((_, i) => {
                const btn = document.getElementById(`att-btn-${i}`);
                if (btn) {
                    btn.className = i === index
                        ? "w-full text-left p-4 rounded-2xl bg-slate-800 border border-purple-500/80 flex items-center justify-between shadow-lg"
                        : "w-full text-left p-4 rounded-2xl bg-slate-900/60 border border-slate-800 hover:bg-slate-800 transition flex items-center justify-between group";
                }
            });

            const att = state.attempts[index];
            const container = document.getElementById('riwayat-detail-container');
            if (!container || !att) return;

            container.innerHTML = `
                <div class="flex items-center justify-between pb-6 border-b border-slate-800 mb-6">
                    <div>
                        <span class="text-xs text-purple-400 font-mono font-semibold block">${att.tanggal}</span>
                        <h2 class="text-xl font-black text-white mt-0.5">${att.judulSimulasi}</h2>
                    </div>
                    <div class="text-right">
                        <span class="text-3xl font-black text-purple-300 font-mono">${att.skor}%</span>
                        <p class="text-[10px] text-slate-400 font-bold mt-0.5">${att.benar} dari ${att.totalSoal} Soal Benar</p>
                    </div>
                </div>

                <div class="space-y-6">
                    ${att.detail.map((d, i) => `
                        <div class="bg-slate-900/90 border ${d.isCorrect ? 'border-emerald-500/40' : 'border-rose-500/40'} p-5 rounded-2xl shadow-md">
                            <div class="flex items-center justify-between mb-3">
                                <span class="text-xs font-bold text-slate-400 font-mono">Soal #${i + 1}</span>
                                <span class="text-[10px] font-extrabold px-2.5 py-1 rounded-full ${d.isCorrect ? 'bg-emerald-500/20 text-emerald-300 border border-emerald-500/30' : 'bg-rose-500/20 text-rose-300 border border-rose-500/30'}">
                                    ${d.isCorrect ? '✓ Jawaban Benar' : '✗ Kurang Tepat'}
                                </span>
                            </div>
                            <p class="text-xs sm:text-sm text-slate-200 font-medium mb-4 leading-relaxed">${d.pertanyaan}</p>
                            
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 mb-4 text-xs font-semibold">
                                <div class="bg-slate-950 p-3 rounded-xl border border-slate-800">
                                    <span class="text-slate-500 block text-[10px] font-mono">Jawaban Anda:</span>
                                    <span class="${d.isCorrect ? 'text-emerald-300' : 'text-rose-300'} font-bold">${d.jawabanUser}</span>
                                </div>
                                <div class="bg-slate-950 p-3 rounded-xl border border-slate-800">
                                    <span class="text-slate-500 block text-[10px] font-mono">Kunci Akurat:</span>
                                    <span class="text-emerald-300 font-bold">${d.kunci}</span>
                                </div>
                            </div>

                            <div class="bg-purple-950/30 border border-purple-800/40 p-4 rounded-xl text-xs text-slate-300 leading-relaxed mb-3">
                                <span class="text-purple-300 font-extrabold block mb-1">📘 Pembahasan Akurat & Langkah Penyelesaian:</span>
                                ${d.solusi}
                            </div>

                            <button onclick="askAiAboutQuestion('${d.pertanyaan.replace(/'/g, "\\'")}')" class="w-full py-2 bg-slate-950 hover:bg-purple-950/50 border border-purple-500/30 text-purple-300 text-xs font-bold rounded-xl transition flex items-center justify-center gap-1.5">
                                <i data-lucide="bot" class="w-3.5 h-3.5"></i> Jelaskan Langkah Ini Lebih Detail via AI
                            </button>
                        </div>
                    `).join('')}
                </div>
            `;
            lucide.createIcons();
        }

        function clearHistory() {
            if (confirm('Apakah Anda yakin ingin menghapus seluruh riwayat pengerjaan simulasi?')) {
                state.attempts = [];
                localStorage.removeItem('nihiluxxy_attempts');
                switchView('riwayat');
            }
        }

        // ==========================================
        // ENHANCED NIHILUXXY AI TUTOR ENGINE v5.0
        // ==========================================
        function toggleAiModal() {
            const modal = document.getElementById('ai-tutor-modal');
            if (modal) {
                modal.classList.toggle('hidden');
                if (!modal.classList.contains('hidden')) {
                    document.getElementById('ai-user-input')?.focus();
                }
            }
        }

        function handleAiKeyDown(e) {
            if (e.key === 'Enter' && !e.shiftKey) {
                e.preventDefault();
                sendAiQuery();
            }
        }

        function injectAiPrompt(text) {
            const input = document.getElementById('ai-user-input');
            if (input) {
                input.value = text;
                sendAiQuery();
            }
        }

        function askAiAboutTopic(topicTitle) {
            toggleAiModal();
            injectAiPrompt(`Tolong berikan penjelasan super mendalam, analisis konsep, dan rumus praktis untuk topik: ${topicTitle}`);
        }

        function askAiAboutSubject(subjectName) {
            toggleAiModal();
            injectAiPrompt(`Beri saya ringkasan peta konsep terpenting yang sering keluar di UTBK SNBT untuk mata pelajaran: ${subjectName}`);
        }

        function askAiAboutQuestion(qText) {
            toggleAiModal();
            injectAiPrompt(`Tolong bedah dan jelaskan langkah demi langkah penyelesaian dari soal berikut: "${qText}"`);
        }

        function sendAiQuery() {
            const input = document.getElementById('ai-user-input');
            const chatBody = document.getElementById('ai-chat-body');
            if (!input || !chatBody) return;

            const text = input.value.trim();
            if (!text) return;

            // Render User Bubble
            const userBubble = document.createElement('div');
            userBubble.className = "flex gap-3 items-start justify-end";
            userBubble.innerHTML = `
                <div class="bg-purple-600 text-white p-3.5 rounded-2xl text-xs sm:text-sm max-w-xl leading-relaxed shadow-lg font-medium">
                    ${text}
                </div>
                <div class="w-8 h-8 rounded-xl bg-slate-800 flex-shrink-0 flex items-center justify-center text-purple-300 text-xs font-bold font-mono">You</div>
            `;
            chatBody.appendChild(userBubble);

            input.value = '';
            chatBody.scrollTop = chatBody.scrollHeight;

            // Render AI Loading State
            const aiBubble = document.createElement('div');
            aiBubble.className = "flex gap-3 items-start";
            const loadingId = 'ai-loading-' + Date.now();
            aiBubble.innerHTML = `
                <div class="w-8 h-8 rounded-xl gradient-accent flex-shrink-0 flex items-center justify-center text-white text-xs font-bold">AI</div>
                <div id="${loadingId}" class="bg-slate-900/90 border border-purple-500/30 p-4 rounded-2xl text-xs sm:text-sm text-slate-300 max-w-xl leading-relaxed shadow-lg flex items-center gap-2">
                    <i data-lucide="loader-2" class="w-4 h-4 text-purple-400 animate-spin"></i>
                    <span>Nihiluxxy AI v5.0 sedang memproses & menganalisis pertanyaan...</span>
                </div>
            `;
            chatBody.appendChild(aiBubble);
            lucide.createIcons();
            chatBody.scrollTop = chatBody.scrollHeight;

            // Multi-Subject Smart Response Engine
            setTimeout(() => {
                const target = document.getElementById(loadingId);
                if (target) {
                    const responseHTML = generateSmartAiResponse(text);
                    target.innerHTML = responseHTML;
                    chatBody.scrollTop = chatBody.scrollHeight;
                }
            }, 1000);
        }

        function generateSmartAiResponse(query) {
            const q = query.toLowerCase();

            // INTEGRAL
            if (q.includes('integral') || q.includes('luas daerah')) {
                return `
                    <div class="space-y-3">
                        <span class="text-pink-400 font-extrabold block text-xs">📐 Nihiluxxy AI Step Solver - Integral & Luas:</span>
                        <p><strong>Aturan Dasar Integral:</strong> ∫ xⁿ dx = [1 / (n + 1)] · xⁿ⁺¹ + C</p>
                        <p><strong>Rumus Cepat Luas Antara Parabola & Garis:</strong></p>
                        <div class="bg-slate-950 p-3 rounded-xl border border-slate-800 text-xs font-mono text-purple-300 text-center">
                            Luas L = (D √D) / (6 a²)
                        </div>
                        <p class="text-xs text-slate-300">Gunakan rumus D√D / 6a² jika soal meminta luas yang dibatasi parabola ax² + bx + c = 0 tanpa perlu menghitung integral panjang!</p>
                    </div>
                `;
            }
            // TURUNAN
            else if (q.includes('turunan') || q.includes('gradien') || q.includes('singgung')) {
                return `
                    <div class="space-y-3">
                        <span class="text-cyan-400 font-extrabold block text-xs">📈 Nihiluxxy AI - Turunan & Gradien:</span>
                        <p><strong>Aturan Turunan Dasar:</strong> f(x) = axⁿ ⇒ f'(x) = a·n·xⁿ⁻¹</p>
                        <p><strong>Mencari Garis Singgung di (x₁, y₁):</strong></p>
                        <ol class="list-decimal list-inside space-y-1 text-xs text-slate-300 font-mono">
                            <li>Hitung gradien m = f'(x₁).</li>
                            <li>Gunakan rumus garis: y - y₁ = m(x - x₁).</li>
                        </ol>
                    </div>
                `;
            }
            // KIRCHHOFF & LISTRIK
            else if (q.includes('kirchhoff') || q.includes('listrik') || q.includes('loop')) {
                return `
                    <div class="space-y-3">
                        <span class="text-amber-400 font-extrabold block text-xs">⚡ Trik Fisika AI - Kirchhoff 2 Loop:</span>
                        <p><strong>Aturan Tegangan Loop:</strong> ΣE + Σ(I · R) = 0</p>
                        <ul class="list-disc list-inside space-y-1 text-xs text-slate-300">
                            <li>Jika loop menembus kutub panjang baterai duluan = <strong>(+) E</strong>.</li>
                            <li>Jika loop menembus kutub pendek baterai duluan = <strong>(-) E</strong>.</li>
                            <li>Jika arah arus searah loop = <strong>(+) I·R</strong>.</li>
                        </ul>
                    </div>
                `;
            }
            // REDOKS & KIMIA
            else if (q.includes('redoks') || q.includes('sel volta') || q.includes('katoda')) {
                return `
                    <div class="space-y-3">
                        <span class="text-purple-300 font-extrabold block text-xs">🧪 Jembatan Keledai Reaksi Redoks:</span>
                        <div class="bg-slate-950 p-3 rounded-xl border border-slate-800 text-xs font-mono text-emerald-300 text-center">
                            KRAO: Katoda Reduksi (Kutub +) | Anoda Oksidasi (Kutub -)
                        </div>
                        <p class="text-xs text-slate-300"><strong>E°sel = E°katoda - E°anoda.</strong> Logam yang nilai E° reduksinya lebih besar (lebih positif) selalu berada di Katoda!</p>
                    </div>
                `;
            }
            // LOGIKA & SILOGISME
            else if (q.includes('silogisme') || q.includes('modus') || q.includes('penalaran')) {
                return `
                    <div class="space-y-3">
                        <span class="text-emerald-400 font-extrabold block text-xs">🧠 Trik Logika UTBK SNBT:</span>
                        <ul class="list-disc list-inside space-y-1 text-xs text-slate-300">
                            <li><strong>Modus Ponens:</strong> P → Q, P ⇒ Kesimpulan: <strong>Q</strong></li>
                            <li><strong>Modus Tollens:</strong> P → Q, ~Q ⇒ Kesimpulan: <strong>~P</strong></li>
                            <li><strong>Silogisme:</strong> P → Q, Q → R ⇒ Kesimpulan: <strong>P → R</strong></li>
                        </ul>
                    </div>
                `;
            }
            // FALLBACK GENERAL
            else {
                return `
                    <div class="space-y-2">
                        <span class="text-purple-300 font-extrabold block text-xs">🤖 Analisis AI Nihiluxxy v5.0:</span>
                        <p>Terima kasih atas pertanyaanmu mengenai: <em>"${query}"</em>.</p>
                        <p>Untuk membedah tipe soal ini dengan tepat, petakan variabel ke rumus utamanya dan eliminasi pilihan jawaban yang tidak logis. Ketik soal spesifik atau topik yang ingin kamu bedah!</p>
                    </div>
                `;
            }
        }

        // Initialize App
        document.addEventListener('DOMContentLoaded', () => {
            switchView('home');
        });
    </script>
</body>
</html>
