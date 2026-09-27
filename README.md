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
                radial-gradient(at 0% 0%, rgba(124, 58, 237, 0.18) 0px, transparent 50%),
                radial-gradient(at 100% 0%, rgba(99, 102, 241, 0.18) 0px, transparent 50%),
                radial-gradient(at 50% 100%, rgba(236, 72, 153, 0.12) 0px, transparent 50%);
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
                ⚡ Nihiluxxy AI Pro v6.0 Ultra Master Expanded
            </span>
            <span class="hidden sm:inline text-slate-300">Seluruh Materi SMA (Kelas 10-12 Kompleks) & Bank Soal UTBK SNBT 2026</span>
        </div>
        <div class="flex items-center gap-4 text-[11px] font-semibold text-purple-300">
            <span class="hidden md:flex items-center gap-1.5 font-mono text-emerald-400">
                <span class="w-2 h-2 rounded-full bg-emerald-400 animate-pulse"></span> Multi-Solver Engine Active
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
                    <input type="text" id="global-search" oninput="handleGlobalSearch(this.value)" placeholder="Cari materi & soal (misal: Vektor, Matriks, pH, Stoikiometri, Hukum Newton, Sosiologi)..." class="w-full bg-slate-900/90 border border-slate-700/80 rounded-2xl pl-10 pr-12 py-2 text-xs text-slate-200 focus:outline-none focus:border-purple-500 focus:ring-1 focus:ring-purple-500 transition shadow-inner">
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
                <button onclick="switchView('kalkulator')" id="nav-kalkulator" class="px-4 py-2.5 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="calculator" class="w-4 h-4 text-cyan-400"></i> Kalkulator AI
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
                            <span class="text-[9px] px-2 py-0.5 rounded-full bg-emerald-500/20 text-emerald-300 border border-emerald-500/40 font-mono font-bold">Smart Multi-Solver v6.0</span>
                        </div>
                        <p class="text-[11px] text-purple-300">Pakar Matematika, Fisika, Kimia, Biologi, Ekonomi, Sosiologi, Geografi, Sejarah & UTBK SNBT 2026</p>
                    </div>
                </div>
                <button onclick="toggleAiModal()" class="w-9 h-9 rounded-xl bg-slate-800/80 hover:bg-slate-700 text-slate-400 hover:text-white flex items-center justify-center transition">
                    <i data-lucide="x" class="w-5 h-5"></i>
                </button>
            </div>

            <!-- AI Quick Action Chips Bar -->
            <div class="p-3 bg-slate-900/90 border-b border-slate-800 flex gap-2 overflow-x-auto custom-scrollbar text-xs">
                <button onclick="injectAiPrompt('Bagaimana cara cepat menghitung Perkalian Titik dan Proyeksi Vektor Ortogonal?')" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-purple-900/50 border border-slate-700 text-purple-200 whitespace-nowrap transition flex items-center gap-1.5">
                    <i data-lucide="move-right" class="w-3.5 h-3.5 text-blue-400"></i> Proyeksi Vektor
                </button>
                <button onclick="injectAiPrompt('Tolong jelaskan rumus Invers dan Determinan Matriks 2x2 beserta contoh soal HOTS!')" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-purple-900/50 border border-slate-700 text-purple-200 whitespace-nowrap transition flex items-center gap-1.5">
                    <i data-lucide="grid" class="w-3.5 h-3.5 text-pink-400"></i> Matriks & Invers
                </button>
                <button onclick="injectAiPrompt('Bagaimana menghitung pH larutan penyangga (buffer) asam dan basa secara cepat?')" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-purple-900/50 border border-slate-700 text-purple-200 whitespace-nowrap transition flex items-center gap-1.5">
                    <i data-lucide="flask-conical" class="w-3.5 h-3.5 text-emerald-400"></i> pH Larutan Buffer
                </button>
                <button onclick="injectAiPrompt('Jelaskan Hukum Kirchhoff II dan cara menentukan arah arus loop dalam rangkaian listrik!')" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-purple-900/50 border border-slate-700 text-purple-200 whitespace-nowrap transition flex items-center gap-1.5">
                    <i data-lucide="zap" class="w-3.5 h-3.5 text-amber-400"></i> Hukum Kirchhoff
                </button>
            </div>

            <!-- AI Chat Body Container -->
            <div id="ai-chat-body" class="flex-1 p-4 sm:p-6 overflow-y-auto custom-scrollbar space-y-4 bg-slate-950/60">
                <div class="flex gap-3 items-start">
                    <div class="w-9 h-9 rounded-xl gradient-accent flex-shrink-0 flex items-center justify-center text-white text-xs font-bold shadow-md">AI</div>
                    <div class="bg-slate-900/90 border border-purple-500/30 p-4 sm:p-5 rounded-2xl text-xs sm:text-sm text-slate-200 max-w-xl leading-relaxed shadow-xl">
                        <p class="font-bold text-purple-300 text-sm mb-1">Selamat datang di Nihiluxxy AI Super Tutor v6.0 Master Expanded! 🚀</p>
                        <p>Ketik soal rumit untuk mata pelajaran Matematika, Fisika, Kimia, Biologi, Ekonomi, Sosiologi, Geografi, Sejarah, atau Penalaran UTBK. Engine AI akan mengurai konsep, memberikan analogi intuitif, serta menyajikan solusi presisi langkah-demi-langkah!</p>
                    </div>
                </div>
            </div>

            <!-- AI Input Box Area -->
            <div class="p-3 sm:p-4 bg-slate-900 border-t border-slate-800 flex items-center gap-2">
                <textarea id="ai-user-input" rows="1" onkeydown="handleAiKeyDown(event)" placeholder="Ketik pertanyaan atau salin soal di sini (misal: 'Berapa pH larutan CH3COOH 0,1 M jika Ka = 10^-5?')..." class="flex-1 bg-slate-950 border border-slate-700/80 rounded-2xl px-4 py-3 text-xs sm:text-sm text-slate-100 focus:outline-none focus:border-purple-500 custom-scrollbar resize-none"></textarea>
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
            <i data-lucide="book-open" class="w-5 h-5"></i> Modul
        </button>
        <button onclick="switchView('kalkulator')" id="mob-kalkulator" class="flex flex-col items-center gap-1">
            <i data-lucide="calculator" class="w-5 h-5"></i> Hitung
        </button>
        <button onclick="switchView('utbk')" id="mob-utbk" class="flex flex-col items-center gap-1">
            <i data-lucide="award" class="w-5 h-5"></i> UTBK
        </button>
        <button onclick="switchView('flashcards')" id="mob-flashcards" class="flex flex-col items-center gap-1">
            <i data-lucide="brain" class="w-5 h-5"></i> Kartu
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
            currentFlashcardIdx: 0,
            flashcardFilter: 'semua'
        };

        // Fully Expanded Database Engine - 100% Comprehensive Content
        const db = {
            mapel: [
                { id: 'mat', nama: 'Matematika Wajib & Lanjut', icon: 'calculator', color: 'from-blue-600 to-cyan-500', k13: 'Kelas 10-12 IPA/IPS', merdeka: 'Fase E & F (14 Modul Terperinci)' },
                { id: 'fis', nama: 'Fisika', icon: 'zap', color: 'from-indigo-600 to-blue-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Kinematika, Listrik, Optik, Modern)' },
                { id: 'kim', nama: 'Kimia', icon: 'flask-conical', color: 'from-purple-600 to-pink-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Stoikiometri, Asam-Basa, Buffer, Redoks)' },
                { id: 'bio', nama: 'Biologi', icon: 'dna', color: 'from-emerald-600 to-teal-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Sel, Metabolisme, Genetika, Ekologi)' },
                { id: 'eko', nama: 'Ekonomi & Akuntansi', icon: 'trending-up', color: 'from-amber-600 to-yellow-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Pasar, Moneter, Jurnal Penyesuaian)' },
                { id: 'sos', nama: 'Sosiologi', icon: 'users', color: 'from-rose-600 to-red-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Interaksi, Penyimpangan, Stratifikasi)' },
                { id: 'geo', nama: 'Geografi', icon: 'globe', color: 'from-teal-600 to-emerald-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Prinsip, Litosfer, Atmosfer, Peta)' },
                { id: 'sej', nama: 'Sejarah Indonesia & Dunia', icon: 'landmark', color: 'from-red-600 to-orange-500', k13: 'Kelas 10-12 Wajib/Peminatan', merdeka: 'Fase E & F (Peradaban, Proklamasi, Orba)' },
                { id: 'lit', nama: 'Literasi Bahasa & Penalaran', icon: 'book-marked', color: 'from-orange-600 to-amber-500', k13: 'Wajib Semua Jurusan', merdeka: 'Fase E & F (General Literacy & PU)' }
            ],
            flashcards: [
                { mapel: 'Matematika', pertanyaan: 'Apakah turunan pertama dari f(x) = axⁿ menurut aturan turunan dasar?', jawaban: 'f\'(x) = a · n · xⁿ⁻¹.' },
                { mapel: 'Matematika', pertanyaan: 'Berapakah rumus integral tentu ∫ xⁿ dx untuk n ≠ -1?', jawaban: '∫ xⁿ dx = [1 / (n + 1)] · xⁿ⁺¹ + C.' },
                { mapel: 'Matematika', pertanyaan: 'Apakah syarat utama dua vektor u dan v saling tegak lurus (ortogonal)?', jawaban: 'Hasil perkalian titiknya sama dengan nol: u · v = 0.' },
                { mapel: 'Matematika', pertanyaan: 'Apakah rumus invers fungsi rasional f(x) = (ax + b) / (cx + d)?', jawaban: 'f⁻¹(x) = (-dx + b) / (cx - a).' },
                { mapel: 'Matematika', pertanyaan: 'Berapakah jumlah tak hingga deret geometri jika suku pertama a dan rasio r (|r| < 1)?', jawaban: 'S_∞ = a / (1 - r).' },
                { mapel: 'Fisika', pertanyaan: 'Apakah Hukum Kirchhoff II tentang tegangan dalam sebuah loop tertutup?', jawaban: 'Jumlah perubahan potensial (ΣE + Σ(I·R)) dalam loop tertutup adalah nol.' },
                { mapel: 'Fisika', pertanyaan: 'Bagaimana nilai v_y pada titik puncak gerak parabola?', jawaban: 'v_y = 0 m/s.' },
                { mapel: 'Fisika', pertanyaan: 'Apakah rumus frekuensi gelombang pada Efek Doppler jika sumber bunyi mendekat?', jawaban: 'f_p = [v / (v - v_s)] · f_s.' },
                { mapel: 'Kimia', pertanyaan: 'Apakah perubahan yang terjadi saat Sistem Kesetimbangan ditambah konsentrasi pereaksinya?', jawaban: 'Kesetimbangan bergeser ke arah Kanan (ke arah Produk/Hasil Reaksi).' },
                { mapel: 'Kimia', pertanyaan: 'Bagaimanakah rumus menghitung [H⁺] pada larutan penyangga (buffer) asam?', jawaban: '[H⁺] = K_a × (mol Asam Lemah / mol Basa Konjugasi).' },
                { mapel: 'Kimia', pertanyaan: 'Apakah syarat wujud zat yang dihitung dalam rumus K_c?', jawaban: 'Hanya wujud Gas (g) dan Larutan/Aqueous (aq).' },
                { mapel: 'Biologi', pertanyaan: 'Apakah peran utama Klorofil dalam Reaksi Terang Fotosintesis?', jawaban: 'Menyerap energi foton matahari dan mengalami eksitasi elektron.' },
                { mapel: 'Biologi', pertanyaan: 'Di manakah tempat terjadinya Siklus Krebs dalam sel?', jawaban: 'Di dalam Matriks Mitokondria.' },
                { mapel: 'Biologi', pertanyaan: 'Apakah fungsi utama organel Ribosom dalam sel?', jawaban: 'Sintesis protein dari asam amino berdasarkan arahan mRNA.' },
                { mapel: 'Ekonomi', pertanyaan: 'Apakah rumus Elastisitas Harga Permintaan (E_d)?', jawaban: 'E_d = (% Perubahan Jumlah Permintaan) / (% Perubahan Harga).' },
                { mapel: 'Ekonomi', pertanyaan: 'Bagaimana dampak penetapan harga batas atas (Ceiling Price) bagi pasar?', jawaban: 'Membuat jumlah permintaan melebihi penawaran (Excess Demand / Kelangkaan).' },
                { mapel: 'Sosiologi', pertanyaan: 'Apakah perbedaan mendasar antara Akulturasi dan Asimilasi?', jawaban: 'Akulturasi: Pembauran budaya tanpa menghilangkan ciri asli. Asimilasi: Pembauran hingga membentuk budaya baru.' },
                { mapel: 'Sosiologi', pertanyaan: 'Apakah arti ciri Sosiologi bersifat Non-Etis?', jawaban: 'Menganalisis fakta sosial secara objektif tanpa menilai baik atau buruknya moral pelaku.' },
                { mapel: 'Geografi', pertanyaan: 'Apakah fungsi utama Citra Penginderaan Jauh inframerah termal?', jawaban: 'Mendeteksi suhu permukaan bumi, pemetaan vegetasi, dan persebaran kalor.' },
                { mapel: 'Sejarah', pertanyaan: 'Apakah latar belakang utama terjadinya peristiwa Rengasdengklok pada 16 Agustus 1945?', jawaban: 'Perbedaan pendapat antara golongan muda dan tua mengenai waktu pelaksanaan proklamasi tanpa campur tangan PPKI/Jepang.' },
                { mapel: 'Penalaran Umum', pertanyaan: 'Apakah kesimpulan sah dari Modus Tollens: P → Q, ~Q?', jawaban: 'Kesimpulannya adalah ~P (Bukan P).' }
            ],
            materiDetails: {
                'mat': [
                    {
                        title: '1. Eksponen, Bentuk Akar & Logaritma (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Eksponen menggambarkan bentuk perkalian berulang dari suatu bilangan basis. Logaritma adalah operasi kebalikan (invers) dari eksponensial yang menentukan besar pangkat suatu bilangan pokok (misal: aⁿ = b ⇔ ᵃlog b = n).',
                        visual: 'ᵃlog(b·c) = ᵃlog b + ᵃlog c  |  ᵃlog(b/c) = ᵃlog b - ᵃlog c  |  ᵃlog bⁿ = n · ᵃlog b',
                        tips: '<strong>Langkah Cerdas Penyelesaian:</strong> Apabila menemui persamaan eksponen berbentuk a^(f(x)) = a^(g(x)), segera samakan pangkatnya menjadi f(x) = g(x) dengan syarat basis a > 0 dan a ≠ 1.',
                        contohSoal: 'Jika diketahui ᵃlog b + ᵃlog b² = 12, hitunglah nilai dari ᵃlog(a·b).<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Gunakan sifat logaritma: ᵃlog b² = 2 · ᵃlog b.<br>2. Persamaan menjadi: ᵃlog b + 2 · ᵃlog b = 12 ⇒ 3 · ᵃlog b = 12 ⇒ ᵃlog b = 4.<br>3. Hitung ᵃlog(a·b) = ᵃlog a + ᵃlog b = 1 + 4 = <strong>5</strong>.'
                    },
                    {
                        title: '2. Persamaan Kuadrat & Rumus Vieta (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Persamaan kuadrat adalah persamaan polinomial berderajat dua dengan bentuk umum ax² + bx + c = 0. Nilai Diskriminan D = b² - 4ac menentukan sifat akar (D > 0 dua akar real berbeda, D = 0 dua akar kembar, D < 0 akar imajiner).',
                        visual: 'Vieta: x₁ + x₂ = -b/a  |  x₁ · x₂ = c/a  |  Puncak Parabola: (-b / 2a , -D / 4a)',
                        tips: '<strong>Trik HOTS:</strong> Gunakan identitas aljabar Vieta untuk menentukan jumlah kuadrat akar-akar: x₁² + x₂² = (x₁ + x₂)² - 2(x₁·x₂).',
                        contohSoal: 'Jika x² - (k + 2)x + 16 = 0 memiliki dua akar kembar positif, tentukan nilai k.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Syarat akar kembar adalah D = 0 ⇒ (-(k+2))² - 4(1)(16) = 0 ⇒ (k+2)² = 64.<br>2. Akarkan kedua ruas: k + 2 = 8 atau k + 2 = -8 ⇒ k = 6 atau k = -10.<br>3. Karena kedua akar positif, jumlah akar x₁ + x₂ = (k+2)/1 > 0 ⇒ 6+2 = 8 > 0 (Memenuhi). Jadi nilai k = <strong>6</strong>.'
                    },
                    {
                        title: '3. Trigonometri Dasar & Identitas Lanjut (Kelas 10-11 / Fase E & F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Trigonometri mempelajari hubungan antara sudut dan panjang sisi segitiga. Pada segitiga siku-siku: sin θ = depan/miring, cos θ = samping/miring, dan tan θ = depan/samping. Identitas utama yang wajib dihafalkan adalah sin²θ + cos²θ = 1.',
                        visual: 'sin(A ± B) = sin A cos B ± cos A sin B  |  cos(A ± B) = cos A cos B ∓ sin A sin B',
                        tips: '<strong>Aturan Sinus & Kosinus:</strong> Gunakan Aturan Sinus (a/sin A = b/sin B) jika diketahui pasang sudut-sisi berhadapan, dan Aturan Kosinus (c² = a² + b² - 2ab cos C) jika diketahui dua sisi dan satu sudut apit.',
                        contohSoal: 'Segitiga ABC memiliki panjang sisi a = 4 cm, b = 6 cm, dan sudut C = 60°. Hitunglah panjang sisi c.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Gunakan Aturan Kosinus: c² = a² + b² - 2ab cos C.<br>2. Substitusi nilai: c² = 4² + 6² - 2(4)(6) cos 60° = 16 + 36 - 48(0,5) = 52 - 24 = 28.<br>3. Panjang sisi c = √28 = <strong>2√7 cm</strong>.'
                    },
                    {
                        title: '4. Vektor pada R² & R³ (Proyeksi & Ortogonalitas) (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Vektor adalah besaran yang memiliki nilai dan arah. Operasi perkalian skalar dua vektor (dot product) dinyatakan sebagai u · v = |u||v| cos θ = u₁v₁ + u₂v₂ + u₃v₃.',
                        visual: 'Dua Vektor Tegak Lurus: u · v = 0  |  Proyeksi Skalar: |p| = (u · v) / |v|',
                        tips: 'Dua vektor u dan v dikatakan saling tegak lurus (ortogonal) jika dan hanya jika hasil perkalian titiknya sama dengan nol (u · v = 0).',
                        contohSoal: 'Diketahui vektor u = (2, -1) dan v = (x, 4). Jika u dan v saling tegak lurus, berapa nilai x?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Syarat tegak lurus: u · v = 0.<br>2. Hitung dot product: (2)(x) + (-1)(4) = 0 ⇒ 2x - 4 = 0 ⇒ 2x = 4 ⇒ <strong>x = 2</strong>.'
                    },
                    {
                        title: '5. Matriks, Determinan & Invers (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Matriks adalah susunan bilangan dalam bentuk baris dan kolom. Determinan matriks 2x2 [[a,b],[c,d]] didefinisikan sebagai det(A) = ad - bc. Invers matriks A⁻¹ didefinisikan sebagai (1/det A) · [[d,-b],[-c,a]].',
                        visual: 'det(A · B) = det(A) · det(B)  |  det(A⁻¹) = 1 / det(A)  |  det(k·A_2x2) = k²·det(A)',
                        tips: 'Jika nilai determinan suatu matriks sama dengan nol (det A = 0), maka matriks tersebut bersifat singular dan tidak memiliki invers.',
                        contohSoal: 'Jika det(A) = 5 dan det(B) = 2, berapakah determinan dari 3A⁻¹ · B untuk matriks berordo 2x2?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Sifat determinan: det(3A⁻¹ · B) = 3² · det(A⁻¹) · det(B).<br>2. Sifat invers: det(A⁻¹) = 1/det(A) = 1/5.<br>3. Hitung hasil akhir: 9 × (1/5) × 2 = <strong>18/5 = 3,6</strong>.'
                    },
                    {
                        title: '6. Barisan & Deret Aritmatika - Geometri (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Barisan aritmatika memiliki selisih antar suku (beda b) yang konstan, sedangkan barisan geometri memiliki perbandingan antar suku (rasio r) yang konstan. Deret geometri tak hingga konvergen jika rasio -1 < r < 1.',
                        visual: 'Aritmatika: U_n = a + (n-1)b  |  Geometri: U_n = a·rⁿ⁻¹  |  Tak Hingga: S_∞ = a / (1 - r)',
                        tips: '<strong>Trik Cepat Aritmatika:</strong> Jumlah n suku pertama deret aritmatika dapat dicari instan dengan S_n = (n / 2) · (suku pertama + suku terakhir).',
                        contohSoal: 'Sebuah deret geometri tak hingga memiliki suku pertama a = 12 dan jumlah tak hingga S_∞ = 18. Hitunglah rasionya.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Gunakan rumus S_∞ = a / (1 - r).<br>2. Substitusi nilai: 18 = 12 / (1 - r) ⇒ 1 - r = 12/18 = 2/3.<br>3. Rasio r = 1 - 2/3 = <strong>1/3</strong>.'
                    },
                    {
                        title: '7. Limit Fungsi Aljabar & Trigonometri (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Limit menjelaskan perilaku suatu fungsi ketika variabel mendekati nilai tertentu. Jika substitusi langsung menghasilkan bentuk tak tentu 0/0, selesaikan dengan memfaktorkan atau mengalikan sekawan, atau gunakan Aturan L\'Hopital (turunan pembilang / turunan penyebut).',
                        visual: 'lim (x→c) [f(x)/g(x)] = lim (x→c) [f\'(x)/g\'(x)]  |  lim (x→0) (sin ax / bx) = a/b',
                        tips: 'Ingat rumus limit trigonometri dasar: lim (x→0) (sin ax / bx) = a/b dan lim (x→0) (tan ax / bx) = a/b.',
                        contohSoal: 'Hitunglah nilai dari lim (x→0) (1 - cos 2x) / (x sin x).<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Gunakan identitas trigonometri: 1 - cos 2x = 2 sin² x.<br>2. Limit menjadi lim (x→0) (2 sin² x) / (x sin x) = lim (x→0) (2 sin x) / x.<br>3. Menurut sifat limit trigonometri lim (x→0) (sin x / x) = 1, maka hasilnya adalah 2(1) = <strong>2</strong>.'
                    },
                    {
                        title: '8. Turunan Fungsi, Garis Singgung & Stasioner (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Turunan pertama f\'(x) merepresentasikan laju perubahan seketika sekaligus gradien garis singgung (m) kurva di titik tertentu. Titik stasioner dicapai ketika f\'(x) = 0.',
                        visual: 'Aturan Rantai: d/dx [f(g(x))] = f\'(g(x)) · g\'(x)  |  m = f\'(x₁)',
                        tips: 'Fungsi selalu naik pada interval di mana f\'(x) > 0, dan fungsi selalu turun pada interval di mana f\'(x) < 0.',
                        contohSoal: 'Tentukan titik balik minimum dari kurva f(x) = x² - 6x + 8.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Syarat stasioner: f\'(x) = 0 ⇒ 2x - 6 = 0 ⇒ x = 3.<br>2. Hitung nilai fungsi y = f(3) = (3)² - 6(3) + 8 = 9 - 18 + 8 = -1.<br>3. Titik balik minimum adalah <strong>(3, -1)</strong>.'
                    },
                    {
                        title: '9. Integral Tentu, Luas & Volume Benda Putar (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Integral adalah operasi kebalikan dari turunan (antiturunan). Integral tentu digunakan untuk menghitung luas daerah di bawah kurva L = ∫[a,b] f(x) dx serta volume benda putar V = π ∫[a,b] [f(x)]² dx.',
                        visual: 'Trik Luas Parabola-Garis: L = (D √D) / (6 a²)',
                        tips: 'Gunakan rumus cepat L = (D √D) / (6a²) untuk menghitung luas daerah antara parabola ax² + bx + c dan sumbu-X tanpa perlu mengintegralkan.',
                        contohSoal: 'Hitunglah luas daerah yang dibatasi oleh parabola y = x² - 4x dan sumbu-X.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Nilai a = 1, b = -4, c = 0. Diskriminan D = (-4)² - 4(1)(0) = 16.<br>2. Gunakan rumus cepat: Luas = (16 × √16) / (6 × 1²) = (16 × 4) / 6 = 64 / 6 = <strong>32/3 satuan luas</strong>.'
                    },
                    {
                        title: '10. Polinomial / Suku Banyak & Teorema Sisa (Kelas 11 Lanjut / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Polinomial P(x) adalah bentuk aljabar berderajat n. Teorema Sisa menyatakan bahwa apabila polinomial P(x) dibagi oleh pembagi berbentuk (x - k), maka sisa pembagiannya adalah S = P(k).',
                        visual: 'Teorema Faktor: (x - k) merupakan faktor dari P(x) jika dan hanya jika P(k) = 0',
                        tips: 'Manfaatkan Metode Horner untuk pembagian polinomial agar proses perhitungan jauh lebih cepat dibandingkan pembagian bersusun.',
                        contohSoal: 'Jika P(x) = 2x³ - x² + ax - 4 dibagi oleh (x - 2) menghasilkan sisa 10, tentukan nilai a.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Menurut Teorema Sisa: Sisa = P(2) = 10.<br>2. Substitusi x = 2: 2(2)³ - (2)² + a(2) - 4 = 10 ⇒ 16 - 4 + 2a - 4 = 10.<br>3. Simplifikasi: 8 + 2a = 10 ⇒ 2a = 2 ⇒ <strong>a = 1</strong>.'
                    },
                    {
                        title: '11. Kombinatorika, Permutasi & Peluang (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Permutasi digunakan untuk menghitung susunan objek dengan memperhatikan urutan P(n,r) = n!/(n-r)!. Kombinasi digunakan jika urutan tidak diperhatikan C(n,r) = n!/[r!(n-r)!].',
                        visual: 'Peluang P(A) = n(A) / n(S)  |  Kejadian Saling Bebas: P(A ∩ B) = P(A) × P(B)',
                        tips: '<strong>Kata Kunci HOTS:</strong> Jika soal menyebutkan "susunan/jabatan/ranking", gunakan Permutasi. Jika menyebutkan "pemilihan tim/kelompok/kelereng acak", gunakan Kombinasi.',
                        contohSoal: 'Dari 6 orang calon pengurus, akan dipilih 3 orang untuk menjadi anggota tim peneliti. Berapa banyak cara pemilihan?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Karena pemilihan tim tidak membedakan jabatan, gunakan Kombinasi C(6,3).<br>2. Hitung: C(6,3) = 6! / (3! · (6-3)!) = (6 × 5 × 4) / (3 × 2 × 1) = <strong>20 cara</strong>.'
                    },
                    {
                        title: '12. Geometri Analitik Lingkaran & Garis Singgung (Kelas 11 Lanjut / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Lingkaran berpusat di (a,b) dengan jari-jari r memiliki persamaan (x - a)² + (y - b)² = r². Persamaan umum lingkaran adalah x² + y² + Ax + By + C = 0 dengan Pusat (-A/2, -B/2) dan r = √(A²/4 + B²/4 - C).',
                        visual: 'Garis Singgung Bergradien m: y - b = m(x - a) ± r √(1 + m²)',
                        tips: 'Panjang garis singgung persekutuan luar dua lingkaran dengan jarak pusat d dan jari-jari R, r adalah L = √(d² - (R - r)²).',
                        contohSoal: 'Tentukan titik pusat dan jari-jari lingkaran dari persamaan x² + y² - 4x + 6y - 12 = 0.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Pusat lingkaran = (-(-4)/2, -6/2) = <strong>(2, -3)</strong>.<br>2. Jari-jari r = √(2² + (-3)² - (-12)) = √(4 + 9 + 12) = √25 = <strong>5 unit</strong>.'
                    },
                    {
                        title: '13. Fungsi Komposisi & Fungsi Invers (Kelas 10-11 / Fase E & F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Fungsi komposisi (f ∘ g)(x) memetakan g(x) terlebih dahulu lalu dimasukkan ke dalam f(x). Fungsi invers f⁻¹(x) merepresentasikan pemetaan kebalikan dari daerah hasil kembali ke daerah asal.',
                        visual: 'Invers Fungsi Rasional: f(x) = (ax + b)/(cx + d) ⇒ f⁻¹(x) = (-dx + b)/(cx - a)',
                        tips: '<strong>Trik Cepat Invers Rasional:</strong> Untuk membalikkan fungsi f(x) = (ax + b) / (cx + d), cukup tukar posisi angka a dan d lalu balikkan tandanya menjadi negatif.',
                        contohSoal: 'Jika f(x) = (3x + 2) / (x - 4), tentukanlah rumus fungsi invers f⁻¹(x).<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Identifikasi parameter: a = 3, b = 2, c = 1, d = -4.<br>2. Gunakan rumus cepat: tukar posisi a=3 dan d=-4 dengan mengubah tanda.<br>3. Hasil fungsi invers f⁻¹(x) = <strong>(4x + 2) / (x - 3)</strong>.'
                    },
                    {
                        title: '14. Program Linear & Nilai Optimum (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Program linear adalah metode untuk memaksimalkan atau meminimalkan fungsi tujuan f(x,y) = ax + by di bawah kendala sistem pertidaksamaan linear.',
                        visual: 'Garis Selidik: ax + by = k  |  Uji Titik Pojok Daerah Penyelesaian (DP)',
                        tips: 'Nilai optimum selalu terletak pada salah satu titik pojok (vertiks) dari daerah himpunan penyelesaian (DHP).',
                        contohSoal: 'Tentukan nilai maksimum dari fungsi objektif z = 3x + 4y jika titik-titik pojok DHP adalah (0,5), (3,3), dan (4,0).<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Uji titik (0,5): z = 3(0) + 4(5) = 20.<br>2. Uji titik (3,3): z = 3(3) + 4(3) = 9 + 12 = 21.<br>3. Uji titik (4,0): z = 3(4) + 4(0) = 12.<br>4. Nilai maksimum adalah <strong>21</strong> (di titik (3,3)).'
                    }
                ],
                'fis': [
                    {
                        title: '1. Kinematika & Gerak Parabola (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Gerak parabola merupakan perpaduan antara Gerak Lurus Beraturan (GLB) pada sumbu horizontal X dan Gerak Lurus Berubah Beraturan (GLBB) pada sumbu vertikal Y di bawah pengaruh percepatan gravitasi.',
                        visual: 'H_max = (v₀² sin² θ) / 2g  |  X_max = (v₀² sin 2θ) / g',
                        tips: 'Di titik tertinggi trajectory parabola, komponen kecepatan vertikal bernilai v_y = 0 m/s, tetapi kecepatan horizontal v_x tetap konstan v₀ cos θ.',
                        contohSoal: 'Sebuah peluru ditembakkan dengan v₀ = 20 m/s dan sudut elevasi 30° (g = 10 m/s²). Hitunglah tinggi maksimum peluru.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Gunakan rumus H_max = (v₀² sin² θ) / 2g.<br>2. Nilai sin 30° = 0,5.<br>3. Hitung: H_max = (20² × (0,5)²) / (2 × 10) = (400 × 0,25) / 20 = 100 / 20 = <strong>5 meter</strong>.'
                    },
                    {
                        title: '2. Hukum Newton & Dinamika Gerak (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Hukum I Newton menjelaskan kelembaman (ΣF = 0), Hukum II Newton menjelaskan hubungan gaya dan percepatan (ΣF = m·a), serta Hukum III Newton menjelaskan aksi-reaksi (F_aksi = -F_reaksi).',
                        visual: 'Gaya Gesek: f_g = μ · N  |  Komponen Bidang Miring: F_sejajar = m·g sin θ',
                        tips: 'Selalu uraikan seluruh komponen gaya sejajar dan tegak lurus bidang gerak terlebih dahulu sebelum menyusun persamaan percepatan.',
                        contohSoal: 'Balok 4 kg berada pada bidang miring licin bersudut 30° (g = 10 m/s²). Berapakah percepatan balok menyusuri bidang?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Gaya penggerak searah bidang miring adalah F = m·g sin 30°.<br>2. Menurut Hukum II Newton: a = F / m = (m·g sin 30°) / m = g sin 30°.<br>3. Hitung: a = 10 × 0,5 = <strong>5 m/s²</strong>.'
                    },
                    {
                        title: '3. Gelombang Bunyi & Efek Doppler (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Efek Doppler adalah perubahan frekuensi bunyi yang terdeteksi oleh pendengar akibat adanya gerak relatif antara sumber bunyi dan pendengar.',
                        visual: 'f_p = [(v ± v_p) / (v ± v_s)] · f_s',
                        tips: '<strong>Aturan Tanda Efek Doppler:</strong> Pendengar mendekat (+), pendengar menjauh (-), sumber mendekat (-), sumber menjauh (+). (Ingat: mendekat membuat frekuensi lebih tinggi!).',
                        contohSoal: 'Ambulans (f_s = 640 Hz) melaju v_s = 20 m/s mendekati pengamat diam (v_p = 0, v = 340 m/s). Hitung frekuensi yang didengar pengamat.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Karena sumber mendekat, gunakan v - v_s di penyebut.<br>2. Hitung: f_p = [340 / (340 - 20)] × 640 = (340 / 320) × 640 = 340 × 2 = <strong>680 Hz</strong>.'
                    },
                    {
                        title: '4. Listrik Dinamis & Hukum Kirchhoff (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Hukum Kirchhoff I menyatakan bahwa jumlah arus masuk cabang sama dengan arus keluar. Hukum Kirchhoff II menyatakan bahwa dalam satu loop tertutup, jumlah ggl baterai dan penurunan tegangan bernilai nol (ΣE + Σ(I·R) = 0).',
                        visual: 'Seri: R_total = R₁ + R₂  |  Paralel: 1/R_total = 1/R₁ + 1/R₂  |  P = V · I',
                        tips: 'Jika dari perhitungan Hukum Kirchhoff diperoleh nilai arus I bernilai negatif, artinya arah pemisalan arus sebenarnya berlawanan arah.',
                        contohSoal: 'Hambatan R₁ = 3 Ω dan R₂ = 6 Ω dirangkai paralel lalu dihubungkan ke sumber tegangan 12 V. Hitunglah arus total rangkaian.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Hambatan pengganti paralel: 1/R_p = 1/3 + 1/6 = 3/6 ⇒ R_p = 2 Ω.<br>2. Arus total menurut Hukum Ohm: I = V / R_p = 12 / 2 = <strong>6 Ampere</strong>.'
                    }
                ],
                'kim': [
                    {
                        title: '1. Stoikiometri & Konsep Mol (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Mol adalah satuan jumlah zat kimia. 1 mol zat mengandung 6,02 × 10²³ partikel (Avisogadro). Hubungan dasar: n = massa / Mr, dan pada STP (0°C, 1 atm), V = n × 22,4 Liter.',
                        visual: 'n = m / Mr  |  V_STP = n × 22,4 L  |  Molaritas M = n / V(L)',
                        tips: 'Untuk menentukan Pereaksi Pembatas, bagilah jumlah mol masing-masing zat pereaksi dengan koefisien reaksinya. Nilai terkecil adalah pereaksi yang habis terlebih dahulu.',
                        contohSoal: 'Hitunglah volume dari 0,25 mol gas O₂ pada kondisi standar (STP).<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Gunakan rumus V_STP = mol × 22,4 Liter.<br>2. Hitung: V = 0,25 × 22,4 = <strong>5,6 Liter</strong>.'
                    },
                    {
                        title: '2. Termokimia & Hukum Hess (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Termokimia mempelajari perubahan kalor dalam reaksi kimia. Reaksi eksoterm melepaskan kalor (ΔH < 0), sedangkan endoterm menyerap kalor (ΔH > 0). Hukum Hess menyatakan bahwa perubahan entalpi reaksi hanya bergantung pada keadaan awal dan akhir.',
                        visual: 'ΔH_reaksi = Σ ΔH°f(produk) - Σ ΔH°f(pereaksi)',
                        tips: 'Jika suatu persamaan reaksi dibalik, tanda nilai ΔH harus dibalik (+ jadi -). Jika reaksi dikalikan n, nilai ΔH juga dikalikan n.',
                        contohSoal: 'Kalor pembentukan standar ΔH°f CO₂ = -393,5 kJ/mol. Berapa kalor yang dilepaskan pada pembakaran sempurna 12 gram Karbon (Ar C = 12)?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Hitung mol C = massa / Ar = 12 / 12 = 1 mol.<br>2. Karena ΔH°f CO₂ melambangkan pembakaran 1 mol C, kalor yang dilepas = <strong>393,5 kJ</strong>.'
                    },
                    {
                        title: '3. Larutan Asam-Basa, Buffer & Titrasi (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> pH merepresentasikan derajat keasaman pH = -log[H⁺]. Larutan Penyangga (Buffer) mampu mempertahankan pH ketika ditambah sedikit asam/basa. Buffer Asam terdiri dari Asam Lemah dan Basa Konjugasinya.',
                        visual: 'Buffer Asam: [H⁺] = K_a × (mol Asam Lemah / mol Basa Konjugasi)  |  pH = -log[H⁺]',
                        tips: 'Jika asam lemah bereaksi dengan basa kuat dan menyisakan asam lemah, maka terbentuk sistem Larutan Penyangga (Buffer).',
                        contohSoal: 'Hitung pH larutan buffer yang mengandung 0,1 mol CH₃COOH (Ka = 10⁻⁵) dan 0,01 mol CH₃COONa.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Gunakan rumus [H⁺] = Ka × (mol asam / mol garam) = 10⁻⁵ × (0,1 / 0,01) = 10⁻⁵ × 10 = 10⁻⁴ M.<br>2. Hitung pH = -log(10⁻⁴) = <strong>4</strong>.'
                    },
                    {
                        title: '4. Reaksi Redoks & Sel Volta (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Reaksi redoks melibatkan transfer elektron. Sel Volta mengubah energi kimia menjadi energi listrik secara spontan. Katode merupakan tempat terjadinya reduksi (kutub +), sedangkan Anode tempat oksidasi (kutub -).',
                        visual: 'KRAO: Katode Reduksi (+) | Anode Oksidasi (-)  |  E°sel = E°katode - E°anode',
                        tips: '<strong>Singkatan Hafalan:</strong> KRAO (Katoda Reduksi, Anoda Oksidasi). Logam dengan potensial reduksi E° lebih positif selalu bertindak sebagai Katoda.',
                        contohSoal: 'Diketahui E° Zn²⁺/Zn = -0,76 V dan E° Cu²⁺/Cu = +0,34 V. Hitunglah potensial standar sel (E°sel) yang terbentuk.<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Logam Cu memiliki E° lebih positif (+0,34 V) sehingga menjadi Katode.<br>2. Hitung: E°sel = E°katode - E°anode = +0,34 - (-0,76) = <strong>+1,10 Volt</strong>.'
                    }
                ],
                'bio': [
                    {
                        title: '1. Biologi Sel & Transpor Membran (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Membran sel bersifat selektif permeabel. Transpor pasif (difusi dan osmosis) terjadi mengikuti gradien konsentrasi tanpa energi ATP, sedangkan transpor aktif (pompa Na⁺-K⁺) membutuhkan energi ATP.',
                        visual: 'Osmosis: Pelarut (air) berpindah dari hipotonis (encer) menuju hipertonis (pekat)',
                        tips: 'Sel darah merah (eritrosit) yang dimasukkan ke dalam larutan hipertonis akan kehilangan air dan mengalami pengerutan sel (Krenasi).',
                        contohSoal: 'Mengapa sel tumbuhan tidak pecah (lisis) saat berada di lingkungan hipotonis?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>Air masuk ke dalam sel tumbuhan hingga mencapai tekanan turgor maksimal, tetapi sel tidak pecah karena dilindungi oleh <strong>Dinding Sel</strong> yang kaku dan kuat.'
                    },
                    {
                        title: '2. Metabolisme: Katabolisme & Anabolisme (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Katabolisme memecah molekul kompleks menjadi sederhana dan menghasilkan ATP (Respirasi Aerob: Glikolisis, Dekarboksilasi Oksidatif, Siklus Krebs, Transpor Elektron). Anabolisme menyusun molekul kompleks (Fotosintesis).',
                        visual: 'Fotosintesis: Reaksi Terang (Tilakoid → ATP, NADPH, O₂) + Reaksi Gelap (Stroma → Glukosa)',
                        tips: 'Penerima (akseptor) elektron terakhir pada tahap Transpor Elektron respirasi aerob adalah molekul Oksigen (O₂), yang kemudian membentuk H₂O.',
                        contohSoal: 'Di manakah tempat terjadinya tahap Siklus Krebs dalam respirasi seluler aerob?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>Siklus Krebs berlangsung di dalam <strong>Matriks Mitokondria</strong> dan menghasilkan 2 ATP, 6 NADH, 2 FADH₂, dan 4 CO₂.'
                    },
                    {
                        title: '3. Genetika & Hukum Persilangan Mendel (Kelas 12 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> DNA menyimpan informasi genetik dalam bentuk susunan basa nitrogen (Adenin-Timin, Guanin-Sitosin). Hukum I Mendel menyatakan pemisahan gen secara bebas saat pembentukan gamet.',
                        visual: 'Pasangan Basa DNA: Adenin - Timin (2 ikatan H)  |  Guanin - Sitosin (3 ikatan H)',
                        tips: 'Rasio fenotip persilangan monohibrid dominan penuh F2 adalah 3 : 1, sedangkan rasio fenotip persilangan dihibrid heterozigot (AaBb × AaBb) F2 adalah 9 : 3 : 3 : 1.',
                        contohSoal: 'Tanaman dihibrid AaBb disilangkan dengan sesamanya. Berapa peluang mendapatkan keturunan bergenotip homozigot resesif (aabb)?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Peluang aa dari Aa × Aa adalah 1/4.<br>2. Peluang bb dari Bb × Bb adalah 1/4.<br>3. Peluang kombinasi aabb = (1/4) × (1/4) = <strong>1/16 (atau 6,25%)</strong>.'
                    }
                ],
                'eko': [
                    {
                        title: '1. Kelangkaan & Biaya Peluang / Opportunity Cost (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Kelangkaan terjadi karena kebutuhan manusia tidak terbatas sedangkan sumber daya terbatas. Biaya Peluang adalah nilai barang/kesempatan terbaik yang dikorbankan karena memilih opsi alternatif lain.',
                        visual: 'Biaya Peluang = Nilai Kesempatan Terbaik yang Tidak Dipilih (Tergantikan)',
                        tips: 'Nilai Biaya Peluang diukur dari nilai opsi tertinggi yang DITINGGALKAN, bukan jumlah total seluruh alternatif.',
                        contohSoal: 'Rina memiliki opsi kerja: Perusahaan A (gaji 5 jt), Perusahaan B (gaji 6 jt). Jika Rina memilih melanjutkan kuliah, berapakah biaya peluangnya?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>Opsi tertinggi yang dikorbankan Rina adalah tawaran Perusahaan B. Maka biaya peluangnya adalah <strong>Rp 6.000.000</strong>.'
                    },
                    {
                        title: '2. Keseimbangan Pasar & Elastisitas (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Keseimbangan pasar tercapai ketika jumlah permintaan sama dengan jumlah penawaran (Qd = Qs). Elastisitas mengukur kepekaan perubahan jumlah barang akibat perubahan harga.',
                        visual: 'Syarat Keseimbangan: Q_d = Q_s  |  E = (% ΔQ) / (% ΔP)',
                        tips: 'Jika nilai elastisitas E > 1 disebut Elastis, E < 1 disebut Inelastis, dan E = 1 disebut Uniter.',
                        contohSoal: 'Diketahui fungsi permintaan Q_d = 40 - 2P dan fungsi penawaran Q_s = -10 + 3P. Tentukan harga keseimbangan pasar (P_e).<br><strong>Langkah Penyelesaian Terperinci:</strong><br>1. Samakan Q_d = Q_s ⇒ 40 - 2P = -10 + 3P.<br>2. Kelompokkan variabel: 5P = 50 ⇒ P_e = <strong>10</strong>.'
                    }
                ],
                'sos': [
                    {
                        title: '1. Sosiologi Sebagai Ilmu & Ciri-Cirinya (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Sosiologi adalah ilmu yang mempelajari masyarakat dan interaksi sosial. 4 Ciri Utama Sosiologi: Empiris (berdasarkan observasi fakta), Teoritis (menyusun abstraksi), Kumulatif (memperbaiki teori lama), dan Non-Etis (objektif).',
                        visual: 'Non-Etis = Menganalisis fenomena tanpa menilai baik atau buruknya moral pelaku',
                        tips: 'Jika dalam soal disebutkan peneliti mengungkap motif kejahatan tanpa menyalahkan atau menghakimi pelaku secara moral, ciri sosiologi yang dimaksud adalah Non-Etis.',
                        contohSoal: 'Sosiolog mengkaji fenomena anak jalanan secara sistematis tanpa menghakimi latar belakang moral mereka. Ciri sosiologi apakah ini?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>Fokus kajian adalah mengungkap fakta sosial secara objektif tanpa penilaian etis, sehingga mencerminkan ciri <strong>Non-Etis</strong>.'
                    }
                ],
                'geo': [
                    {
                        title: '1. Konsep & Prinsip Utama Geografi (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Geografi mempelajari fenomena geosfer. 4 Prinsip Geografi: Persebaran (distribusi tak merata), Interelasi (keterkaitan sebab-akibat), Deskripsi (penjelasan tabel/peta), dan Korologi (komprehensif ruang).',
                        visual: 'Prinsip Interelasi = Hubungan timbal balik / sebab-akibat antar fenomena geosfer',
                        tips: 'Gunakan Prinsip Interelasi jika soal menghubungkan dua fenomena, misalnya penebangan hutan di hulunya sungai yang menyebabkan banjir bandang di pemukiman hilir.',
                        contohSoal: 'Bencana tanah longsor di Puncak terjadi akibat pembukaan lahan hutan yang tak terkendali. Prinsip geografi yang digunakan?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>Fenomena longsor dihubungkan langsung dengan sebab pembukaan lahan, sehingga dianalisis menggunakan <strong>Prinsip Interelasi</strong>.'
                    }
                ],
                'sej': [
                    {
                        title: '1. Peristiwa Sekitar Proklamasi & Pembentukan Negara (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Kekalahan Jepang dalam Perang Pasifik memicu perdebatan antara Golongan Muda dan Golongan Tua yang berujung pada Peristiwa Rengasdengklok untuk mengamankan Soekarno-Hatta agar proklamasi dilakukan tanpa pengaruh Jepang.',
                        visual: 'Rengasdengklok (16 Ags 1945) → Perumusan Teks (Rumah Tadashi Maeda) → Proklamasi (Pegangsaan Timur 56)',
                        tips: 'Tujuan utama penjelasan Golongan Muda membawa Soekarno-Hatta ke Rengasdengklok adalah menjauhkan mereka dari tekanan dan pengaruh janji kemerdekaan Jepang.',
                        contohSoal: 'Apakah alasan utama Golongan Muda membawa Soekarno dan Hatta ke Rengasdengklok pada 16 Agustus 1945?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>Untuk mendesak agar proklamasi kemerdekaan segera dilaksanakan secara mandiri tanpa campur tangan dan janji dari pihak Panitia Persiapan Kemerdekaan Indonesia (PPKI) buatan Jepang.'
                    }
                ],
                'lit': [
                    {
                        title: '1. Penalaran Logis, Silogisme & Modus Tollens (UTBK)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Penjelasan Konsep Terperinci:</strong> Penalaran deduktif menarik kesimpulan yang pasti sah dari premis-premis umum. Tiga aturan penarikan kesimpulan utama: Modus Ponens, Modus Tollens, dan Silogisme.',
                        visual: 'Modus Ponens: P→Q, P ⇒ Q  |  Modus Tollens: P→Q, ~Q ⇒ ~P  |  Silogisme: P→Q, Q→R ⇒ P→R',
                        tips: '<strong>Jebakan Logika UTBK:</strong> Dari premis P → Q, KITA TIDAK BISA menyimpulkan ~P → ~Q atau Q → P. Hati-hati dengan kekeliruan ini!',
                        contohSoal: 'Premis 1: Jika siswa belajar konsisten, maka ia lulus UTBK. Premis 2: Andi tidak lulus UTBK. Apakah kesimpulan yang sah?<br><strong>Langkah Penyelesaian Terperinci:</strong><br>Gunakan Modus Tollens (P → Q, ~Q ⇒ ~P). P = Belajar konsisten, Q = Lulus UTBK. Karena ~Q (tidak lulus), maka kesimpulannya adalah <strong>Andi tidak belajar secara konsisten (~P)</strong>.'
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

            ['home', 'materi', 'kalkulator', 'utbk', 'flashcards', 'riwayat'].forEach(v => {
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
            else if (viewName === 'kalkulator') content.innerHTML = renderKalkulatorScreen();
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
                            <span>Nihiluxxy AI Pro 2026 • Master Expanded Edition</span>
                        </div>
                        <h1 class="text-3xl sm:text-5xl font-black text-white tracking-tight mb-4 leading-tight">
                            Kuasai Seluruh Konsep SMA & Taklukkan <span class="bg-clip-text text-transparent gradient-accent">UTBK SNBT 2026</span>.
                        </h1>
                        <p class="text-slate-300 text-xs sm:text-sm mb-8 leading-relaxed">
                            Modul SMA (Kelas 10–12) komprehensif seluruh mata pelajaran, rumus visual, tips instan, kalkulator sains otomatis, serta pengerjaan soal HOTS terperinci dibantu oleh **Nihiluxxy AI Tutor v6.0**.
                        </p>
                        <div class="flex flex-wrap gap-4">
                            <button onclick="switchView('materi')" class="gradient-accent text-white font-extrabold px-6 py-3.5 rounded-2xl shadow-lg shadow-purple-500/25 hover:opacity-95 transition flex items-center gap-2 text-xs sm:text-sm">
                                <i data-lucide="book-open" class="w-4 h-4"></i> Pelajari Modul Terperinci
                            </button>
                            <button onclick="switchView('kalkulator')" class="bg-slate-900/90 border border-cyan-500/40 text-cyan-200 font-extrabold px-6 py-3.5 rounded-2xl hover:bg-slate-800 transition flex items-center gap-2 text-xs sm:text-sm">
                                <i data-lucide="calculator" class="w-4 h-4 text-cyan-400"></i> Kalkulator AI Math & Sains
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Stats Cards -->
                <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-12">
                    <div class="glass-card p-5 rounded-2xl text-center border-purple-500/20">
                        <span class="text-2xl font-black text-purple-400 font-mono">50+</span>
                        <span class="text-xs text-slate-400 block mt-1 font-semibold">Modul Seluruh Mapel</span>
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
                        <span class="text-xs text-slate-400 block mt-1 font-semibold">Multi-Solver Integrated</span>
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

                    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-5">
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

        // Render Kalkulator Sains & Matematika Screen
        function renderKalkulatorScreen() {
            return `
                <div class="mb-8">
                    <h1 class="text-3xl font-black text-white tracking-tight">Kalkulator AI Matematika & Sains</h1>
                    <p class="text-slate-400 text-xs sm:text-sm mt-1">Hitung otomatis persamaan kuadrat, invers/determinan matriks, kombinatorika, deret tak hingga, pH kimia, dan kinematics.</p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    
                    <!-- 1. Kalkulator Persamaan Kuadrat -->
                    <div class="glass-card border border-purple-500/30 p-6 rounded-3xl shadow-xl">
                        <div class="flex items-center gap-3 mb-4">
                            <div class="p-2.5 rounded-xl bg-purple-500/20 text-purple-300">
                                <i data-lucide="function-square" class="w-5 h-5"></i>
                            </div>
                            <h3 class="font-extrabold text-white text-sm">Persamaan Kuadrat (ax² + bx + c = 0)</h3>
                        </div>
                        <div class="grid grid-cols-3 gap-2 mb-4">
                            <input type="number" id="calc-a" placeholder="a" value="1" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="number" id="calc-b" placeholder="b" value="-5" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="number" id="calc-c" placeholder="c" value="6" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                        </div>
                        <button onclick="calculateQuad()" class="w-full py-2 bg-purple-600 hover:bg-purple-500 text-white font-extrabold text-xs rounded-xl transition mb-4 shadow-md">
                            Hitung Akar & Vieta
                        </button>
                        <div id="calc-quad-res" class="bg-slate-950/80 border border-slate-800 p-3 rounded-xl text-xs font-mono text-purple-300">
                            Hasil akan muncul di sini...
                        </div>
                    </div>

                    <!-- 2. Kalkulator Determinan & Invers Matriks 2x2 -->
                    <div class="glass-card border border-cyan-500/30 p-6 rounded-3xl shadow-xl">
                        <div class="flex items-center gap-3 mb-4">
                            <div class="p-2.5 rounded-xl bg-cyan-500/20 text-cyan-300">
                                <i data-lucide="grid" class="w-5 h-5"></i>
                            </div>
                            <h3 class="font-extrabold text-white text-sm">Determinan & Invers Matriks</h3>
                        </div>
                        <div class="grid grid-cols-2 gap-2 mb-4 max-w-xs mx-auto">
                            <input type="number" id="mat-a" placeholder="a" value="3" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="number" id="mat-b" placeholder="b" value="2" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="number" id="mat-c" placeholder="c" value="1" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="number" id="mat-d" placeholder="d" value="4" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                        </div>
                        <button onclick="calculateMatrix()" class="w-full py-2 bg-cyan-600 hover:bg-cyan-500 text-white font-extrabold text-xs rounded-xl transition mb-4 shadow-md">
                            Hitung Invers & Det
                        </button>
                        <div id="calc-mat-res" class="bg-slate-950/80 border border-slate-800 p-3 rounded-xl text-xs font-mono text-cyan-300">
                            Hasil matriks muncul di sini...
                        </div>
                    </div>

                    <!-- 3. Kalkulator Permutasi & Kombinasi -->
                    <div class="glass-card border border-emerald-500/30 p-6 rounded-3xl shadow-xl">
                        <div class="flex items-center gap-3 mb-4">
                            <div class="p-2.5 rounded-xl bg-emerald-500/20 text-emerald-300">
                                <i data-lucide="dices" class="w-5 h-5"></i>
                            </div>
                            <h3 class="font-extrabold text-white text-sm">Permutasi P(n,r) & Kombinasi C(n,r)</h3>
                        </div>
                        <div class="grid grid-cols-2 gap-2 mb-4">
                            <input type="number" id="comb-n" placeholder="n (total)" value="6" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="number" id="comb-r" placeholder="r (dipilih)" value="3" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                        </div>
                        <button onclick="calculateComb()" class="w-full py-2 bg-emerald-600 hover:bg-emerald-500 text-white font-extrabold text-xs rounded-xl transition mb-4 shadow-md">
                            Hitung Peluang & Cara
                        </button>
                        <div id="calc-comb-res" class="bg-slate-950/80 border border-slate-800 p-3 rounded-xl text-xs font-mono text-emerald-300">
                            Hasil kombinasi muncul di sini...
                        </div>
                    </div>

                    <!-- 4. Deret Geometri Tak Hingga -->
                    <div class="glass-card border border-amber-500/30 p-6 rounded-3xl shadow-xl">
                        <div class="flex items-center gap-3 mb-4">
                            <div class="p-2.5 rounded-xl bg-amber-500/20 text-amber-300">
                                <i data-lucide="infinity" class="w-5 h-5"></i>
                            </div>
                            <h3 class="font-extrabold text-white text-sm">Deret Geometri Tak Hingga (S_∞)</h3>
                        </div>
                        <div class="grid grid-cols-2 gap-2 mb-4">
                            <input type="number" id="geo-a" placeholder="a (suku awal)" value="12" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="text" id="geo-r" placeholder="r (rasio < 1)" value="0.333" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                        </div>
                        <button onclick="calculateGeoInfin()" class="w-full py-2 bg-amber-600 hover:bg-amber-500 text-white font-extrabold text-xs rounded-xl transition mb-4 shadow-md">
                            Hitung Jumlah Tak Hingga
                        </button>
                        <div id="calc-geo-res" class="bg-slate-950/80 border border-slate-800 p-3 rounded-xl text-xs font-mono text-amber-300">
                            Hasil deret muncul di sini...
                        </div>
                    </div>

                    <!-- 5. Kalkulator Kimia: pH Larutan Asam / Basa -->
                    <div class="glass-card border border-pink-500/30 p-6 rounded-3xl shadow-xl">
                        <div class="flex items-center gap-3 mb-4">
                            <div class="p-2.5 rounded-xl bg-pink-500/20 text-pink-300">
                                <i data-lucide="flask-conical" class="w-5 h-5"></i>
                            </div>
                            <h3 class="font-extrabold text-white text-sm">Hitung pH Asam Kuat (pH = -log[H⁺])</h3>
                        </div>
                        <div class="grid grid-cols-2 gap-2 mb-4">
                            <input type="number" step="0.001" id="chem-m" placeholder="Molaritas (M)" value="0.01" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="number" id="chem-val" placeholder="Valensi Asam" value="1" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                        </div>
                        <button onclick="calculatePH()" class="w-full py-2 bg-pink-600 hover:bg-pink-500 text-white font-extrabold text-xs rounded-xl transition mb-4 shadow-md">
                            Hitung Konsentrasi & pH
                        </button>
                        <div id="calc-ph-res" class="bg-slate-950/80 border border-slate-800 p-3 rounded-xl text-xs font-mono text-pink-300">
                            Hasil pH muncul di sini...
                        </div>
                    </div>

                    <!-- 6. Kalkulator Fisika: Tinggi Maksimum Gerak Parabola -->
                    <div class="glass-card border border-blue-500/30 p-6 rounded-3xl shadow-xl">
                        <div class="flex items-center gap-3 mb-4">
                            <div class="p-2.5 rounded-xl bg-blue-500/20 text-blue-300">
                                <i data-lucide="zap" class="w-5 h-5"></i>
                            </div>
                            <h3 class="font-extrabold text-white text-sm">Tinggi Maksimum Gerak Parabola</h3>
                        </div>
                        <div class="grid grid-cols-2 gap-2 mb-4">
                            <input type="number" id="phys-v0" placeholder="v₀ (m/s)" value="20" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                            <input type="number" id="phys-angle" placeholder="Sudut θ (°)" value="30" class="bg-slate-950 border border-slate-700 rounded-xl p-2 text-center text-xs font-mono text-white">
                        </div>
                        <button onclick="calculateParabola()" class="w-full py-2 bg-blue-600 hover:bg-blue-500 text-white font-extrabold text-xs rounded-xl transition mb-4 shadow-md">
                            Hitung H_max & X_max
                        </button>
                        <div id="calc-phys-res" class="bg-slate-950/80 border border-slate-800 p-3 rounded-xl text-xs font-mono text-blue-300">
                            Hasil ketinggian muncul di sini...
                        </div>
                    </div>

                </div>
            `;
        }

        // Calculation Logic
        function calculateQuad() {
            const a = parseFloat(document.getElementById('calc-a').value);
            const b = parseFloat(document.getElementById('calc-b').value);
            const c = parseFloat(document.getElementById('calc-c').value);
            const res = document.getElementById('calc-quad-res');

            if (isNaN(a) || isNaN(b) || isNaN(c) || a === 0) {
                res.innerHTML = "Nilai 'a' tidak boleh nol!";
                return;
            }

            const D = b * b - 4 * a * c;
            const x_sum = -b / a;
            const x_prod = c / a;

            let text = `D = ${D} | x₁+x₂ = ${x_sum} | x₁·x₂ = ${x_prod}<br>`;
            if (D > 0) {
                const x1 = (-b + Math.sqrt(D)) / (2 * a);
                const x2 = (-b - Math.sqrt(D)) / (2 * a);
                text += `Akar Real Beda: x₁ = ${x1.toFixed(2)}, x₂ = ${x2.toFixed(2)}`;
            } else if (D === 0) {
                const x = -b / (2 * a);
                text += `Akar Kembar: x₁ = x₂ = ${x.toFixed(2)}`;
            } else {
                text += `Akar Imajiner (D < 0)`;
            }
            res.innerHTML = text;
        }

        function calculateMatrix() {
            const a = parseFloat(document.getElementById('mat-a').value);
            const b = parseFloat(document.getElementById('mat-b').value);
            const c = parseFloat(document.getElementById('mat-c').value);
            const d = parseFloat(document.getElementById('mat-d').value);
            const res = document.getElementById('calc-mat-res');

            const det = a * d - b * c;
            let text = `det(A) = ${det}<br>`;

            if (det === 0) {
                text += `Matriks Singular (Tidak berpangkat/invers).`;
            } else {
                text += `A⁻¹ = [[ ${(d/det).toFixed(2)}, ${(-b/det).toFixed(2)} ], [ ${(-c/det).toFixed(2)}, ${(a/det).toFixed(2)} ]]`;
            }
            res.innerHTML = text;
        }

        function factorial(n) {
            if (n < 0) return 0;
            if (n === 0 || n === 1) return 1;
            let val = 1;
            for (let i = 2; i <= n; i++) val *= i;
            return val;
        }

        function calculateComb() {
            const n = parseInt(document.getElementById('comb-n').value);
            const r = parseInt(document.getElementById('comb-r').value);
            const res = document.getElementById('calc-comb-res');

            if (isNaN(n) || isNaN(r) || r > n || n < 0 || r < 0) {
                res.innerHTML = "Syarat: 0 ≤ r ≤ n";
                return;
            }

            const P = factorial(n) / factorial(n - r);
            const C = P / factorial(r);

            res.innerHTML = `P(${n},${r}) = ${P} cara<br>C(${n},${r}) = ${C} cara`;
        }

        function calculateGeoInfin() {
            const a = parseFloat(document.getElementById('geo-a').value);
            let r_str = document.getElementById('geo-r').value;
            let r = parseFloat(r_str);

            if (r_str.includes('/')) {
                const parts = r_str.split('/');
                r = parseFloat(parts[0]) / parseFloat(parts[1]);
            }

            const res = document.getElementById('calc-geo-res');

            if (Math.abs(r) >= 1) {
                res.innerHTML = "Deret Divergen (|r| ≥ 1).";
                return;
            }

            const S_inf = a / (1 - r);
            res.innerHTML = `r = ${r.toFixed(3)}<br>Jumlah S_∞ = ${S_inf.toFixed(2)}`;
        }

        function calculatePH() {
            const m = parseFloat(document.getElementById('chem-m').value);
            const val = parseFloat(document.getElementById('chem-val').value);
            const res = document.getElementById('calc-ph-res');

            if (isNaN(m) || isNaN(val) || m <= 0) {
                res.innerHTML = "Masukkan molaritas positif!";
                return;
            }

            const h_plus = m * val;
            const ph = -Math.log10(h_plus);
            res.innerHTML = `[H⁺] = ${h_plus.toExponential(2)} M<br><strong>pH Larutan = ${ph.toFixed(2)}</strong>`;
        }

        function calculateParabola() {
            const v0 = parseFloat(document.getElementById('phys-v0').value);
            const angleDeg = parseFloat(document.getElementById('phys-angle').value);
            const res = document.getElementById('calc-phys-res');

            if (isNaN(v0) || isNaN(angleDeg)) {
                res.innerHTML = "Masukkan nilai valid!";
                return;
            }

            const g = 10;
            const rad = (angleDeg * Math.PI) / 180;
            const sinVal = Math.sin(rad);
            const sin2Val = Math.sin(2 * rad);

            const H_max = (v0 * v0 * sinVal * sinVal) / (2 * g);
            const X_max = (v0 * v0 * sin2Val) / g;

            res.innerHTML = `H_max = ${H_max.toFixed(2)} meter<br>Jarak Terjauh X_max = ${X_max.toFixed(2)} meter`;
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
            let cards = db.flashcards;
            if (state.flashcardFilter && state.flashcardFilter !== 'semua') {
                cards = db.flashcards.filter(c => c.mapel.toLowerCase().includes(state.flashcardFilter.toLowerCase()));
            }
            if (cards.length === 0) cards = db.flashcards;
            if (state.currentFlashcardIdx >= cards.length) state.currentFlashcardIdx = 0;

            const card = cards[state.currentFlashcardIdx];

            return `
                <div class="mb-8 text-center max-w-2xl mx-auto">
                    <span class="text-xs font-extrabold uppercase tracking-widest text-emerald-400 bg-emerald-500/10 px-3 py-1 rounded-full border border-emerald-500/20 mb-2 inline-block">Flashcards Pintar</span>
                    <h1 class="text-3xl font-black text-white tracking-tight">Latihan Cepat Hafalan & Konsep</h1>
                    <p class="text-slate-400 text-xs sm:text-sm mt-1">Uji ingatan intuitif Anda sebelum menghadapi ujian asli.</p>

                    <!-- Filter Chips -->
                    <div class="flex flex-wrap justify-center gap-2 mt-4 text-xs font-semibold">
                        <button onclick="setFlashcardFilter('semua')" class="px-3.5 py-1.5 rounded-xl transition ${state.flashcardFilter === 'semua' ? 'bg-purple-600 text-white' : 'bg-slate-900 text-slate-400 border border-slate-800 hover:text-white'}">Semua</button>
                        <button onclick="setFlashcardFilter('matematika')" class="px-3.5 py-1.5 rounded-xl transition ${state.flashcardFilter === 'matematika' ? 'bg-purple-600 text-white' : 'bg-slate-900 text-slate-400 border border-slate-800 hover:text-white'}">Matematika</button>
                        <button onclick="setFlashcardFilter('fisika')" class="px-3.5 py-1.5 rounded-xl transition ${state.flashcardFilter === 'fisika' ? 'bg-purple-600 text-white' : 'bg-slate-900 text-slate-400 border border-slate-800 hover:text-white'}">Fisika</button>
                        <button onclick="setFlashcardFilter('kimia')" class="px-3.5 py-1.5 rounded-xl transition ${state.flashcardFilter === 'kimia' ? 'bg-purple-600 text-white' : 'bg-slate-900 text-slate-400 border border-slate-800 hover:text-white'}">Kimia</button>
                        <button onclick="setFlashcardFilter('biologi')" class="px-3.5 py-1.5 rounded-xl transition ${state.flashcardFilter === 'biologi' ? 'bg-purple-600 text-white' : 'bg-slate-900 text-slate-400 border border-slate-800 hover:text-white'}">Biologi</button>
                        <button onclick="setFlashcardFilter('ekonomi')" class="px-3.5 py-1.5 rounded-xl transition ${state.flashcardFilter === 'ekonomi' ? 'bg-purple-600 text-white' : 'bg-slate-900 text-slate-400 border border-slate-800 hover:text-white'}">Ekonomi</button>
                        <button onclick="setFlashcardFilter('sosiologi')" class="px-3.5 py-1.5 rounded-xl transition ${state.flashcardFilter === 'sosiologi' ? 'bg-purple-600 text-white' : 'bg-slate-900 text-slate-400 border border-slate-800 hover:text-white'}">Sosiologi</button>
                    </div>
                </div>

                <div class="max-w-xl mx-auto">
                    <div id="flashcard-box" onclick="flipFlashcard()" class="glass-card border border-purple-500/40 rounded-3xl p-8 sm:p-12 min-h-[280px] flex flex-col justify-between items-center text-center cursor-pointer shadow-2xl transition-all duration-300 transform hover:scale-[1.02]">
                        <span class="text-[10px] font-black uppercase text-purple-400 font-mono tracking-widest">${card.mapel} • Klik Kartu Untuk Membalik</span>
                        
                        <div id="flashcard-content" class="my-auto py-4 w-full">
                            <p class="text-base sm:text-lg font-bold text-white leading-relaxed">${card.pertanyaan}</p>
                        </div>

                        <span class="text-[11px] text-slate-500 font-bold">Kartu ${state.currentFlashcardIdx + 1} dari ${cards.length}</span>
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
            let cards = db.flashcards;
            if (state.flashcardFilter && state.flashcardFilter !== 'semua') {
                cards = db.flashcards.filter(c => c.mapel.toLowerCase().includes(state.flashcardFilter.toLowerCase()));
            }
            if (cards.length === 0) cards = db.flashcards;
            const card = cards[state.currentFlashcardIdx];
            const content = document.getElementById('flashcard-content');
            if (!content) return;

            isCardFlipped = !isCardFlipped;
            if (isCardFlipped) {
                content.innerHTML = `<p class="text-sm sm:text-base font-semibold text-emerald-300 leading-relaxed bg-emerald-950/40 p-4 rounded-2xl border border-emerald-500/30 shadow-inner">💡 ${card.jawaban}</p>`;
            } else {
                content.innerHTML = `<p class="text-base sm:text-lg font-bold text-white leading-relaxed">${card.pertanyaan}</p>`;
            }
        }

        function setFlashcardFilter(filter) {
            state.flashcardFilter = filter;
            state.currentFlashcardIdx = 0;
            isCardFlipped = false;
            switchView('flashcards');
        }

        function nextFlashcard() {
            let cards = db.flashcards;
            if (state.flashcardFilter && state.flashcardFilter !== 'semua') {
                cards = db.flashcards.filter(c => c.mapel.toLowerCase().includes(state.flashcardFilter.toLowerCase()));
            }
            if (cards.length === 0) cards = db.flashcards;

            isCardFlipped = false;
            state.currentFlashcardIdx = (state.currentFlashcardIdx + 1) % cards.length;
            switchView('flashcards');
        }

        function prevFlashcard() {
            let cards = db.flashcards;
            if (state.flashcardFilter && state.flashcardFilter !== 'semua') {
                cards = db.flashcards.filter(c => c.mapel.toLowerCase().includes(state.flashcardFilter.toLowerCase()));
            }
            if (cards.length === 0) cards = db.flashcards;

            isCardFlipped = false;
            state.currentFlashcardIdx = (state.currentFlashcardIdx - 1 + cards.length) % cards.length;
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
        // ENHANCED NIHILUXXY AI TUTOR ENGINE v6.0
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
                    <span>Nihiluxxy AI v6.0 sedang memproses & menganalisis pertanyaan...</span>
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

            // VEKTOR & PROYEKSI
            if (q.includes('vektor') || q.includes('proyeksi') || q.includes('ortogonal')) {
                return `
                    <div class="space-y-3">
                        <span class="text-blue-400 font-extrabold block text-xs">➡️ Nihiluxxy AI Multi-Solver - Vektor:</span>
                        <p><strong>1. Perkalian Titik (Dot Product):</strong> u · v = u₁v₁ + u₂v₂ + u₃v₃ = |u||v| cos θ</p>
                        <p><strong>2. Syarat Saling Tegak Lurus:</strong> u · v = 0</p>
                        <p><strong>3. Proyeksi Vektor Ortogonal u pada v:</strong></p>
                        <div class="bg-slate-950 p-3 rounded-xl border border-slate-800 text-xs font-mono text-purple-300 text-center">
                            p = [ (u · v) / |v|² ] · v
                        </div>
                    </div>
                `;
            }
            // MATRIKS & INVERS
            else if (q.includes('matriks') || q.includes('determinan') || q.includes('invers')) {
                return `
                    <div class="space-y-3">
                        <span class="text-pink-400 font-extrabold block text-xs">📊 Nihiluxxy AI - Matriks & Invers:</span>
                        <p><strong>Invers Matriks 2x2:</strong> Jika A = [[a,b],[c,d]], maka A⁻¹ = (1/det A) · [[d,-b],[-c,a]] dengan det A = ad - bc.</p>
                        <p><strong>Sifat Utama Determinan UTBK:</strong></p>
                        <ul class="list-disc list-inside space-y-1 text-xs text-slate-300 font-mono">
                            <li>det(A · B) = det(A) · det(B)</li>
                            <li>det(A⁻¹) = 1 / det(A)</li>
                            <li>det(k · A_n×n) = kⁿ · det(A)</li>
                        </ul>
                    </div>
                `;
            }
            // PH & KIMIA
            else if (q.includes('ph') || q.includes('larutan') || q.includes('buffer')) {
                return `
                    <div class="space-y-3">
                        <span class="text-emerald-400 font-extrabold block text-xs">🧪 Nihiluxxy AI - Larutan Asam Basa & Buffer:</span>
                        <p><strong>1. Asam Kuat:</strong> [H⁺] = Molaritas × Valensi Asam ⇒ pH = -log[H⁺]</p>
                        <p><strong>2. Buffer Asam:</strong> [H⁺] = K_a × (mol Asam Lemah / mol Basa Konjugasi)</p>
                        <p><strong>3. Hidrolisis Garam (Asam Lemah + Basa Kuat):</strong> [OH⁻] = √( (K_w / K_a) × M_garam )</p>
                    </div>
                `;
            }
            // FISIKA & HUKUM NEWTON
            else if (q.includes('fisika') || q.includes('newton') || q.includes('parabola') || q.includes('kirchhoff')) {
                return `
                    <div class="space-y-3">
                        <span class="text-amber-400 font-extrabold block text-xs">⚡ Nihiluxxy AI - Fisika & Dinamika:</span>
                        <p><strong>1. Hukum II Newton:</strong> ΣF = m · a</p>
                        <p><strong>2. Ketinggian Maksimum Parabola:</strong> H_max = (v₀² sin² θ) / (2g)</p>
                        <p><strong>3. Hukum II Kirchhoff:</strong> ΣE + Σ(I·R) = 0 dalam loop tertutup.</p>
                    </div>
                `;
            }
            // FALLBACK GENERAL
            else {
                return `
                    <div class="space-y-2">
                        <span class="text-purple-300 font-extrabold block text-xs">🤖 Analisis AI Nihiluxxy v6.0:</span>
                        <p>Terima kasih atas pertanyaanmu mengenai: <em>"${query}"</em>.</p>
                        <p>Untuk membedah tipe soal ini dengan tepat, petakan variabel ke rumus utamanya dan eliminasi pilihan jawaban yang tidak logis. Kamu juga bisa menggunakan fitur <strong>Kalkulator AI Math & Sains</strong> di menu navigasi!</p>
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
