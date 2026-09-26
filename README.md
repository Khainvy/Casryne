<!DOCTYPE html>
<html lang="id" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nihiluxxy - Platform Belajar Super SMA, TKA & UTBK SNBT 2026 (Full Expanded Edition)</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f5f3ff',
                            100: '#ede9fe',
                            200: '#ddd6fe',
                            300: '#c4b5fd',
                            400: '#a78bfa',
                            500: '#8b5cf6',
                            600: '#7c3aed',
                            700: '#6d28d9',
                            800: '#5b21b6',
                            900: '#4c1d95',
                            950: '#2e1065',
                        }
                    },
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                        mono: ['JetBrains Mono', 'monospace'],
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;600;700&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        body { 
            font-family: 'Plus Jakarta Sans', sans-serif; 
            background-color: #090d16;
            scroll-behavior: smooth;
        }
        .gradient-brand { background: linear-gradient(135deg, #0b132b 0%, #1c2541 40%, #3a506b 100%); }
        .gradient-accent { background: linear-gradient(135deg, #6366f1 0%, #a855f7 50%, #ec4899 100%); }
        .gradient-gemini { background: linear-gradient(135deg, #2563eb 0%, #7c3aed 50%, #db2777 100%); }
        .gradient-card { background: linear-gradient(145deg, rgba(30, 41, 59, 0.7) 0%, rgba(15, 23, 42, 0.8) 100%); }
        .glass-header { background: rgba(9, 13, 22, 0.88); backdrop-filter: blur(16px); }
        .glass-card { background: rgba(30, 41, 59, 0.4); backdrop-filter: blur(10px); border: 1px solid rgba(255, 255, 255, 0.08); }
        
        .custom-scrollbar::-webkit-scrollbar { width: 6px; height: 6px; }
        .custom-scrollbar::-webkit-scrollbar-track { background: rgba(15, 23, 42, 0.6); }
        .custom-scrollbar::-webkit-scrollbar-thumb { background: rgba(139, 92, 246, 0.3); border-radius: 9999px; }
        .custom-scrollbar::-webkit-scrollbar-thumb:hover { background: rgba(139, 92, 246, 0.6); }

        .fade-in { animation: fadeIn 0.3s ease-in-out forwards; }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(6px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .option-selected {
            background-color: rgba(124, 58, 237, 0.2) !important;
            border-color: #8b5cf6 !important;
            box-shadow: 0 0 15px rgba(139, 92, 246, 0.2);
        }

        .typing-dot {
            animation: typingAnimation 1.4s infinite ease-in-out both;
        }
        .typing-dot:nth-child(1) { animation-delay: 0s; }
        .typing-dot:nth-child(2) { animation-delay: 0.2s; }
        .typing-dot:nth-child(3) { animation-delay: 0.4s; }
        @keyframes typingAnimation {
            0%, 80%, 100% { transform: scale(0); }
            40% { transform: scale(1); }
        }

        /* 3D Flashcard Animation Styles */
        .perspective-1000 { perspective: 1000px; }
        .transform-style-3d { transform-style: preserve-3d; transition: transform 0.6s cubic-bezier(0.4, 0, 0.2, 1); }
        .backface-hidden { backface-visibility: hidden; -webkit-backface-visibility: hidden; }
        .rotate-y-180 { transform: rotateY(180deg); }

        @media print {
            body * { visibility: hidden; }
            #riwayat-detail-container, #riwayat-detail-container * { visibility: visible; }
            #riwayat-detail-container { position: absolute; left: 0; top: 0; width: 100%; color: #000; background: #fff !important; }
            .no-print { display: none !important; }
        }
    </style>
</head>
<body class="bg-[#090d16] text-slate-100 min-h-screen flex flex-col selection:bg-purple-500 selection:text-white custom-scrollbar">

    <!-- Toast Notification Container -->
    <div id="toast-container" class="fixed top-24 right-5 z-[100] flex flex-col gap-2 pointer-events-none"></div>

    <!-- Top Navigation Banner -->
    <div class="bg-gradient-to-r from-purple-900 via-indigo-900 to-slate-900 text-xs py-1.5 px-4 text-center font-medium border-b border-purple-500/20 text-purple-200 flex justify-between items-center sticky top-0 z-[60]">
        <span class="hidden sm:inline">⚡ Edisi Terintegrasi Google Gemini AI & Bank Materi Super Lengkap SMA UTBK 2026</span>
        <span class="mx-auto sm:mx-0">🎉 Powered by Gemini 2.5 Flash • Realtime AI Tutor & Flashcard Rumus</span>
        <div class="hidden md:flex gap-4 text-[11px] font-semibold text-purple-300">
            <span class="bg-purple-800/50 px-2 py-0.5 rounded-full border border-purple-400/30">v6.5 Full Content Edition</span>
            <span>•</span>
            <span id="live-clock" class="font-mono">--:--:-- WIB</span>
        </div>
    </div>

    <!-- Header Navigation Bar -->
    <header class="sticky top-7 z-50 glass-header border-b border-slate-800/80 transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between gap-4">
            <!-- Brand Logo -->
            <div class="flex items-center gap-3 cursor-pointer group" onclick="switchView('home')">
                <div class="w-11 h-11 rounded-2xl gradient-gemini flex items-center justify-center text-white font-black text-xl shadow-lg shadow-purple-500/25 group-hover:scale-105 transition duration-300">
                    <i data-lucide="sparkles" class="w-6 h-6"></i>
                </div>
                <div class="flex flex-col">
                    <div class="flex items-center gap-1.5">
                        <span class="text-2xl font-black tracking-tight text-white group-hover:text-purple-300 transition">Nihiluxxy</span>
                        <span class="w-2 h-2 rounded-full bg-pink-500 animate-pulse"></span>
                    </div>
                    <span class="text-[9px] uppercase tracking-widest text-purple-400 font-extrabold -mt-1">Gemini AI Learning Engine</span>
                </div>
            </div>

            <!-- Search Bar Desktop -->
            <div class="hidden lg:flex items-center flex-1 max-w-md mx-6">
                <div class="relative w-full">
                    <i data-lucide="search" class="w-4 h-4 absolute left-3.5 top-1/2 -translate-y-1/2 text-slate-400"></i>
                    <input type="text" id="global-search" oninput="handleGlobalSearch(this.value)" placeholder="Cari konsep (misal: Eksponen, Newton, Stoikiometri)..." class="w-full bg-slate-900/90 border border-slate-700/80 rounded-2xl pl-10 pr-4 py-2 text-xs text-slate-200 focus:outline-none focus:border-purple-500 transition shadow-inner">
                    <div id="search-results-popover" class="hidden absolute left-0 right-0 top-12 bg-slate-900 border border-slate-700 rounded-2xl shadow-2xl p-2 z-50 max-h-80 overflow-y-auto custom-scrollbar"></div>
                </div>
            </div>

            <!-- Desktop Nav Items -->
            <nav class="hidden md:flex items-center gap-1 bg-slate-900/80 p-1.5 rounded-2xl border border-slate-800 text-xs font-semibold">
                <button onclick="switchView('home')" id="nav-home" class="px-3.5 py-2 rounded-xl text-white bg-purple-600 transition flex items-center gap-1.5">
                    <i data-lucide="home" class="w-4 h-4"></i> Beranda
                </button>
                <button onclick="switchView('materi')" id="nav-materi" class="px-3.5 py-2 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="book-open" class="w-4 h-4"></i> Modul SMA
                </button>
                <button onclick="switchView('flashcards')" id="nav-flashcards" class="px-3.5 py-2 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="layers" class="w-4 h-4 text-pink-400"></i>
                    <span>Flashcards Rumus</span>
                </button>
                <button onclick="switchView('utbk')" id="nav-utbk" class="px-3.5 py-2 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="award" class="w-4 h-4 text-amber-400"></i>
                    <span>Simulasi & Quiz</span>
                </button>
                <button onclick="switchView('riwayat')" id="nav-riwayat" class="px-3.5 py-2 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5">
                    <i data-lucide="history" class="w-4 h-4 text-purple-400"></i>
                    <span>Riwayat</span>
                </button>
            </nav>

            <!-- User Gamification & Gemini Status Badge -->
            <div class="flex items-center gap-3">
                <div class="flex items-center gap-2 bg-slate-900 border border-purple-500/30 px-3 py-1.5 rounded-2xl">
                    <span class="text-xs font-black text-amber-400 flex items-center gap-1" title="Daily Streak">
                        🔥 <span id="streak-count">1</span> Hari
                    </span>
                    <span class="text-slate-600">|</span>
                    <span class="text-xs font-black text-purple-300 font-mono flex items-center gap-1" title="User XP">
                        ⭐ <span id="xp-count">50</span> XP
                    </span>
                </div>
                <button onclick="toggleApiKeyModal()" class="p-2.5 bg-slate-900 border border-purple-500/30 rounded-2xl text-purple-300 hover:border-purple-400 transition" title="Pengaturan Gemini API Key">
                    <i data-lucide="key" class="w-4 h-4"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- Main Content Dynamic Container -->
    <main id="app-content" class="flex-grow max-w-7xl w-full mx-auto px-4 sm:px-6 lg:px-8 py-8">
        <!-- Rendered dynamically by JS Engine -->
    </main>

    <!-- Mobile Navigation Bottom Bar -->
    <div class="md:hidden fixed bottom-0 left-0 right-0 glass-header border-t border-slate-800/80 flex justify-around py-2.5 text-[10px] font-semibold text-slate-400 z-50 backdrop-blur-lg">
        <button onclick="switchView('home')" id="mob-home" class="flex flex-col items-center gap-1 text-purple-400">
            <i data-lucide="home" class="w-5 h-5"></i> Beranda
        </button>
        <button onclick="switchView('materi')" id="mob-materi" class="flex flex-col items-center gap-1">
            <i data-lucide="book-open" class="w-5 h-5"></i> Modul
        </button>
        <button onclick="switchView('flashcards')" id="mob-flashcards" class="flex flex-col items-center gap-1">
            <i data-lucide="layers" class="w-5 h-5"></i> Flashcards
        </button>
        <button onclick="switchView('utbk')" id="mob-utbk" class="flex flex-col items-center gap-1">
            <i data-lucide="award" class="w-5 h-5"></i> UTBK
        </button>
        <button onclick="switchView('riwayat')" id="mob-riwayat" class="flex flex-col items-center gap-1">
            <i data-lucide="history" class="w-5 h-5"></i> Riwayat
        </button>
    </div>

    <!-- Floating Gemini AI Assistant Button -->
    <div class="fixed bottom-20 md:bottom-6 right-6 z-50">
        <button onclick="toggleAiModal()" class="gradient-gemini hover:scale-105 transition duration-300 p-4 rounded-full text-white shadow-2xl flex items-center gap-2.5 border border-white/20 group">
            <i data-lucide="bot" class="w-6 h-6 animate-pulse"></i>
            <span class="hidden sm:inline font-extrabold text-xs pr-1">Gemini Super Tutor</span>
        </button>
    </div>

    <!-- Gemini AI Tutor Chat Modal -->
    <div id="ai-modal" class="hidden fixed bottom-24 right-6 w-[420px] max-w-[92vw] h-[520px] bg-slate-900/95 border border-purple-500/50 rounded-3xl shadow-2xl z-50 backdrop-blur-xl flex flex-col fade-in overflow-hidden">
        <div class="p-4 bg-slate-950 border-b border-slate-800 flex items-center justify-between">
            <div class="flex items-center gap-2.5">
                <div class="w-8 h-8 rounded-xl gradient-gemini flex items-center justify-center text-white font-bold text-xs shadow-md">
                    <i data-lucide="sparkles" class="w-4 h-4"></i>
                </div>
                <div>
                    <h4 class="font-extrabold text-xs text-white">Gemini 2.5 AI Tutor</h4>
                    <span id="gemini-status-indicator" class="text-[9px] text-emerald-400 font-semibold flex items-center gap-1">
                        <span class="w-1.5 h-1.5 rounded-full bg-emerald-400 animate-ping"></span> Online (Mode Otomatis/API)
                    </span>
                </div>
            </div>
            <div class="flex items-center gap-1">
                <button onclick="toggleApiKeyModal()" class="text-slate-400 hover:text-purple-300 text-xs p-1" title="Atur Gemini API Key">
                    <i data-lucide="settings" class="w-4 h-4"></i>
                </button>
                <button onclick="toggleAiModal()" class="text-slate-400 hover:text-white text-xs p-1">
                    <i data-lucide="x" class="w-5 h-5"></i>
                </button>
            </div>
        </div>
        
        <div id="ai-chat-body" class="flex-1 p-4 overflow-y-auto space-y-3 custom-scrollbar text-xs">
            <div class="bg-slate-800/80 p-3.5 rounded-2xl border border-slate-700/60 text-slate-200 leading-relaxed">
                ✨ **Halo! Saya Gemini AI Tutor**. Ditenagai oleh Google Gemini API, saya siap membantu menjelaskan rumus sulit, pembahasan soal HOTS, atau trik cepat lulus UTBK SNBT 2026.
            </div>
        </div>

        <!-- Quick Action Chips -->
        <div class="p-2 border-t border-slate-800 bg-slate-950 flex gap-1.5 overflow-x-auto text-[10px] custom-scrollbar">
            <button onclick="sendQuickPrompt('Jelaskan Rumus Vieta dan contoh soalnya!')" class="px-2.5 py-1.5 rounded-lg bg-slate-900 hover:bg-slate-800 text-purple-300 font-semibold whitespace-nowrap border border-purple-500/20">📐 Rumus Vieta</button>
            <button onclick="sendQuickPrompt('Beri saya 3 strategi belajar lulus UTBK SNBT 2026')" class="px-2.5 py-1.5 rounded-lg bg-slate-900 hover:bg-slate-800 text-purple-300 font-semibold whitespace-nowrap border border-purple-500/20">🎯 Strategi SNBT</button>
            <button onclick="sendQuickPrompt('Bagaimana cara cepat menentukan pH Larutan Buffer?')" class="px-2.5 py-1.5 rounded-lg bg-slate-900 hover:bg-slate-800 text-purple-300 font-semibold whitespace-nowrap border border-purple-500/20">🧪 Trik Buffer Kimia</button>
        </div>

        <div class="p-3 bg-slate-950 border-t border-slate-800 flex gap-2">
            <input type="text" id="ai-input" onkeypress="if(event.key === 'Enter') handleAiSend()" placeholder="Tanyakan konsep/soal pada Gemini..." class="flex-1 bg-slate-900 border border-slate-700 rounded-xl px-3 py-2 text-xs text-white focus:outline-none focus:border-purple-500">
            <button onclick="handleAiSend()" class="p-2.5 gradient-gemini hover:opacity-90 text-white rounded-xl transition shadow-md">
                <i data-lucide="send" class="w-4 h-4"></i>
            </button>
        </div>
    </div>

    <!-- API Key Settings Modal -->
    <div id="apikey-modal" class="hidden fixed inset-0 bg-black/70 z-[110] flex items-center justify-center p-4 backdrop-blur-sm">
        <div class="bg-slate-900 border border-purple-500/40 p-6 rounded-3xl max-w-md w-full shadow-2xl fade-in">
            <div class="flex justify-between items-center mb-4">
                <div class="flex items-center gap-2">
                    <div class="p-2 bg-purple-500/20 rounded-xl text-purple-400 border border-purple-500/30">
                        <i data-lucide="key" class="w-5 h-5"></i>
                    </div>
                    <h3 class="text-base font-black text-white">Pengaturan Gemini API Key</h3>
                </div>
                <button onclick="toggleApiKeyModal()" class="text-slate-400 hover:text-white"><i data-lucide="x" class="w-5 h-5"></i></button>
            </div>
            <p class="text-xs text-slate-400 mb-4 leading-relaxed">
                Masukkan API Key Google Gemini Anda untuk membuka akses langsung tanpa batas ke model **Gemini 2.5 Flash**. API Key Anda hanya disimpan di memori browser lokal (`localStorage`).
            </p>
            <input type="password" id="gemini-key-input" placeholder="AIzaSy..." class="w-full bg-slate-950 border border-slate-700 rounded-xl px-4 py-3 text-xs text-white mb-4 focus:outline-none focus:border-purple-500 font-mono">
            <div class="flex justify-between items-center gap-3">
                <a href="https://aistudio.google.com/app/apikey" target="_blank" class="text-[11px] text-purple-400 hover:underline font-bold flex items-center gap-1">
                    <span>Dapatkan API Key Gratis</span>
                    <i data-lucide="external-link" class="w-3 h-3"></i>
                </a>
                <button onclick="saveApiKey()" class="px-5 py-2.5 bg-purple-600 hover:bg-purple-500 text-white font-black text-xs rounded-xl transition">
                    Simpan Key
                </button>
            </div>
        </div>
    </div>

    <!-- Application Footer -->
    <footer class="mt-auto border-t border-slate-800/80 bg-slate-950/60 py-8 text-xs text-slate-400 mb-12 md:mb-0">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center gap-4">
            <div class="flex items-center gap-2">
                <div class="w-6 h-6 rounded-lg gradient-accent flex items-center justify-center text-white text-xs font-bold">N</div>
                <span class="font-extrabold text-slate-200">Nihiluxxy Platform Gemini Edition</span>
                <span class="text-slate-600">|</span>
                <span>Hak Cipta &copy; 2026. Terintegrasi Google Gemini AI.</span>
            </div>
            <div class="flex gap-6 text-slate-400">
                <a href="#" class="hover:text-purple-400 transition">Panduan Gemini AI</a>
                <a href="#" class="hover:text-purple-400 transition">Bank Soal HOTS</a>
                <a href="#" class="hover:text-purple-400 transition">Flashcards Rumus</a>
            </div>
        </div>
    </footer>

    <!-- JS Application Engine -->
    <script>
        // Realtime Clock Update
        setInterval(() => {
            const now = new Date();
            const timeStr = now.toLocaleTimeString('id-ID') + ' WIB';
            const clockEl = document.getElementById('live-clock');
            if (clockEl) clockEl.innerText = timeStr;
        }, 1000);

        // Core Application State
        const state = {
            activeView: 'home',
            selectedKurikulum: 'Merdeka',
            selectedSubject: 'mat',
            attempts: JSON.parse(localStorage.getItem('nihiluxxy_attempts') || '[]'),
            bookmarks: JSON.parse(localStorage.getItem('nihiluxxy_bookmarks') || '[]'),
            userXP: parseInt(localStorage.getItem('nihiluxxy_xp') || '50'),
            userStreak: parseInt(localStorage.getItem('nihiluxxy_streak') || '1'),
            geminiApiKey: localStorage.getItem('nihiluxxy_gemini_key') || '',
            currentSimAnswers: {},
            activeSimKey: null,
            timerInterval: null,
            timeLeftSeconds: 0,
            
            // Flashcard State
            flashcardsCategory: 'Semua',
            flashcardsIndex: 0,
            isFlashcardFlipped: false,
            isAutoFlipping: false,
            autoFlipTimer: null,
            autoFlipIntervalMs: 4000,
            filteredFlashcards: []
        };

        // Gamification Helpers
        function addXP(amount, reason) {
            state.userXP += amount;
            localStorage.setItem('nihiluxxy_xp', state.userXP);
            updateGamificationUI();
            showToast(`+${amount} XP: ${reason}!`, 'success');
        }

        function updateGamificationUI() {
            const xpEl = document.getElementById('xp-count');
            const streakEl = document.getElementById('streak-count');
            if (xpEl) xpEl.innerText = state.userXP;
            if (streakEl) streakEl.innerText = state.userStreak;
        }

        // Bookmark Helper
        function toggleBookmark(materiTitle) {
            const index = state.bookmarks.indexOf(materiTitle);
            if (index > -1) {
                state.bookmarks.splice(index, 1);
                showToast('Modul dihapus dari Favorit');
            } else {
                state.bookmarks.push(materiTitle);
                addXP(10, 'Menandai Modul Favorit');
            }
            localStorage.setItem('nihiluxxy_bookmarks', JSON.stringify(state.bookmarks));
            if (state.activeView === 'materi') openDetailMapel(state.selectedSubject);
        }

        // Gemini API Key Management
        function toggleApiKeyModal() {
            const modal = document.getElementById('apikey-modal');
            const input = document.getElementById('gemini-key-input');
            input.value = state.geminiApiKey;
            modal.classList.toggle('hidden');
            lucide.createIcons();
        }

        function saveApiKey() {
            const val = document.getElementById('gemini-key-input').value.trim();
            state.geminiApiKey = val;
            localStorage.setItem('nihiluxxy_gemini_key', val);
            toggleApiKeyModal();
            showToast(val ? 'Gemini API Key tersimpan!' : 'API Key dikosongkan. Menggunakan mode Simulasi Cerdas.');
            updateGeminiStatusIndicator();
        }

        function updateGeminiStatusIndicator() {
            const indicator = document.getElementById('gemini-status-indicator');
            if (indicator) {
                if (state.geminiApiKey) {
                    indicator.innerHTML = `<span class="w-1.5 h-1.5 rounded-full bg-emerald-400 animate-ping"></span> Connected to Gemini API`;
                } else {
                    indicator.innerHTML = `<span class="w-1.5 h-1.5 rounded-full bg-amber-400"></span> Mode Tutor Cerdas Bawaan`;
                }
            }
        }

        // Gemini API Integration Engine
        async function callGeminiAPI(promptText) {
            if (!state.geminiApiKey) {
                return new Promise(resolve => {
                    setTimeout(() => {
                        const p = promptText.toLowerCase();
                        if (p.includes('vieta')) {
                            resolve("💡 **Rumus Vieta (Gemini AI)**:\nUntuk persamaan kuadrat ax² + bx + c = 0:\n1. Jumlah Akar: x₁ + x₂ = -b/a\n2. Perkalian Akar: x₁ · x₂ = c/a\n\n*Tips UTBK*: Gunakan sifat ini langsung tanpa mencari akar x₁ dan x₂ satu per satu!");
                        } else if (p.includes('strategi') || p.includes('snbt')) {
                            resolve("🚀 **3 Strategi Utama Lolos UTBK 2026 (Gemini AI)**:\n1. **Kuasai Konsep Dasar (80%)**: Soal HOTS dirancang menguji kedalaman konsep, bukan hafalan.\n2. **Manajemen Waktu**: Alokasikan maksimal 1.5 menit per soal Pengetahuan Kuantitatif.\n3. **Eliminasi Cerdas**: Hilangkan 2 opsi paling tidak masuk akal dahulu.");
                        } else if (p.includes('buffer') || p.includes('kimia')) {
                            resolve("🧪 **Trik Cepat Larutan Penyangga/Buffer (Gemini AI)**:\n• Buffer Asam: [H⁺] = Ka × (mol Asam Lemah / mol Basa Konjugasi)\n• Ciri Khas UTBK: Campuran Asam Lemah + Basa Kuat yang **menyisakan Asam Lemah** selalu membentuk Buffer!");
                        } else {
                            resolve(`✨ **Penjelasan Gemini AI Tutor untuk "${promptText}"**:\n\nKonsep ini sangat krusial dalam ujian SMA dan UTBK SNBT. Langkah awal memahami materi ini adalah dengan menguasai definisi dasar, lalu menerapkan sifat-sifat utamanya pada soal bertipe HOTS. Kamu bisa menguji ketangkasanmu lewat menu **Simulasi & Gemini Quiz**!`);
                        }
                    }, 800);
                });
            }

            try {
                const endpoint = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent?key=${state.geminiApiKey}`;
                const response = await fetch(endpoint, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({
                        contents: [{
                            parts: [{ text: `Kamu adalah Gemini AI Tutor untuk siswa SMA dan calon peserta UTBK SNBT 2026 Indonesia di platform Nihiluxxy. Jawablah dengan ringkas, jelas, ilmiah, dan berikan tips cepat pengerjaan soal jika relevan.\n\nPertanyaan siswa: ${promptText}` }]
                        }]
                    })
                });

                const data = await response.json();
                if (data.candidates && data.candidates[0].content.parts[0].text) {
                    return data.candidates[0].content.parts[0].text;
                } else {
                    return "Mohon maaf, Gemini AI tidak dapat memproses permintaan saat ini. Periksa kembali API Key Anda.";
                }
            } catch (err) {
                console.error("Gemini API Error:", err);
                return "Terjadi kesalahan saat menghubungkan ke Google Gemini API. Pastikan koneksi internet stabil dan API Key valid.";
            }
        }

        // AI Chat UI Handlers
        function toggleAiModal() {
            const modal = document.getElementById('ai-modal');
            modal.classList.toggle('hidden');
            updateGeminiStatusIndicator();
            lucide.createIcons();
        }

        function askGeminiTopic(topicTitle) {
            toggleAiModal();
            sendQuickPrompt(`Jelaskan konsep inti dan trik cepat pengerjaan soal untuk topik: "${topicTitle}"`);
        }

        function sendQuickPrompt(promptText) {
            document.getElementById('ai-input').value = promptText;
            handleAiSend();
        }

        async function handleAiSend() {
            const input = document.getElementById('ai-input');
            const chatBody = document.getElementById('ai-chat-body');
            const query = input.value.trim();
            if (!query) return;

            chatBody.innerHTML += `
                <div class="bg-purple-600/30 border border-purple-500/40 p-3 rounded-2xl text-purple-100 text-right font-medium">
                    ${query}
                </div>
            `;
            input.value = '';
            chatBody.scrollTop = chatBody.scrollHeight;

            const loadingId = 'loading_' + Date.now();
            chatBody.innerHTML += `
                <div id="${loadingId}" class="bg-slate-800/90 border border-slate-700/80 p-3 rounded-2xl text-slate-400 flex items-center gap-1.5">
                    <span class="text-[10px] font-bold text-purple-400">Gemini AI sedang berpikir</span>
                    <span class="w-1.5 h-1.5 rounded-full bg-purple-400 typing-dot"></span>
                    <span class="w-1.5 h-1.5 rounded-full bg-purple-400 typing-dot"></span>
                    <span class="w-1.5 h-1.5 rounded-full bg-purple-400 typing-dot"></span>
                </div>
            `;
            chatBody.scrollTop = chatBody.scrollHeight;

            const aiReply = await callGeminiAPI(query);

            const loadingEl = document.getElementById(loadingId);
            if (loadingEl) loadingEl.remove();

            chatBody.innerHTML += `
                <div class="bg-slate-800/90 border border-slate-700/80 p-3.5 rounded-2xl text-slate-200 leading-relaxed fade-in">
                    ${aiReply.replace(/\n/g, '<br>').replace(/\*\*(.*?)\*\*/g, '<strong>$1</strong>')}
                </div>
            `;
            chatBody.scrollTop = chatBody.scrollHeight;
            addXP(5, 'Diskusi dengan Gemini AI');
        }

        // Database Engine (Lengkap & Ter-ekspansi Semua Mata Pelajaran)
        const db = {
            mapel: [
                { id: 'mat', nama: 'Matematika Wajib & Lanjut', icon: 'calculator', color: 'from-blue-600 to-cyan-500', k13: 'Kelas 10-12 IPA/IPS', merdeka: 'Fase E & F (Wajib & Tingkat Lanjut)' },
                { id: 'fis', nama: 'Fisika', icon: 'zap', color: 'from-indigo-600 to-blue-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Peminatan Sains)' },
                { id: 'kim', nama: 'Kimia', icon: 'flask-conical', color: 'from-purple-600 to-pink-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Peminatan Sains)' },
                { id: 'bio', nama: 'Biologi', icon: 'dna', color: 'from-emerald-600 to-teal-500', k13: 'Kelas 10-12 IPA', merdeka: 'Fase F (Peminatan Sains)' },
                { id: 'eko', nama: 'Ekonomi & Akuntansi', icon: 'trending-up', color: 'from-amber-600 to-yellow-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Peminatan Sosial)' },
                { id: 'sos', nama: 'Sosiologi', icon: 'users', color: 'from-rose-600 to-red-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Peminatan Sosial)' },
                { id: 'geo', nama: 'Geografi', icon: 'globe', color: 'from-teal-600 to-emerald-500', k13: 'Kelas 10-12 IPS', merdeka: 'Fase F (Peminatan Sosial)' },
                { id: 'lit', nama: 'Literasi Bahasa & Penalaran', icon: 'book-marked', color: 'from-orange-600 to-amber-500', k13: 'Wajib Semua Jurusan', merdeka: 'Fase E & F (General Literacy)' }
            ],
            
            flashcards: [
                {
                    id: 'fc1',
                    mapel: 'Matematika',
                    topik: 'Rumus Vieta (Akar Persamaan Kuadrat)',
                    tantangan: 'Bagaimanakah cara menentukan Penjumlahan (x₁ + x₂) dan Perkalian (x₁ · x₂) akar-akar ax² + bx + c = 0 tanpa mencari akar x₁ dan x₂?',
                    rumus: 'x₁ + x₂ = -b/a  |  x₁ · x₂ = c/a',
                    trik: '💡 **Trik Cepat UTBK**: Langsung gunakan perbandingan koefisien -b/a dan c/a! Tidak perlu memfaktorkan persamaan kuadrat.'
                },
                {
                    id: 'fc2',
                    mapel: 'Matematika',
                    topik: 'Deret Geometri Tak Hingga Konvergen',
                    tantangan: 'Berapakah jumlah tak hingga deret geometri (S_∞) dengan suku pertama a dan rasio r (-1 < r < 1)?',
                    rumus: 'S_∞ = a / (1 - r)',
                    trik: '💡 **Trik Cepat UTBK**: Hafalkan sebagai rumus **"A-BAH"** (a dibagi 1 minus r).'
                },
                {
                    id: 'fc3',
                    mapel: 'Matematika',
                    topik: 'Integral Parsial',
                    tantangan: 'Bagaimanakah rumus dasar metode Integral Parsial untuk mengintegralkan perkalian dua fungsi?',
                    rumus: '∫ u dv = u · v - ∫ v du',
                    trik: '💡 **Trik Cepat UTBK**: Pilih fungsi `u` yang paling mudah diturunkan menjadi nol (seperti xⁿ).'
                },
                {
                    id: 'fc4',
                    mapel: 'Fisika',
                    topik: 'Efek Doppler (Gelombang Bunyi)',
                    tantangan: 'Bagaimanakah hubungan frekuensi pendengar (f_p) dan frekuensi sumber (f_s) saat terjadi gerak relatif?',
                    rumus: 'f_p = [(v ± v_p) / (v ± v_s)] · f_s',
                    trik: '💡 **Trik Cepat UTBK**: **"Pendengar mendekat = Positif (+)", "Sumber mendekat = Negatif (-)"**.'
                },
                {
                    id: 'fc5',
                    mapel: 'Fisika',
                    topik: 'Efisiensi Mesin Carnot',
                    tantangan: 'Bagaimanakah rumus menghitung efisiensi (η) mesin Carnot ideal dengan suhu reservoir tinggi T₁ dan suhu rendah T₂?',
                    rumus: 'η = (1 - T₂ / T₁) × 100%',
                    trik: '💡 **Trik Cepat UTBK**: Seluruh satuan suhu **WAJIB diubah ke Kelvin (K = °C + 273)** sebelum dimasukkan ke rumus!'
                },
                {
                    id: 'fc6',
                    mapel: 'Fisika',
                    topik: 'Hukum Coulomb (Gaya Listrik Statis)',
                    tantangan: 'Bagaimana perubahan gaya interaksi Coulomb jika jarak antar muatan (r) diperbesar menjadi 2 kali lipat?',
                    rumus: 'F = k · (|q₁ · q₂| / r²)',
                    trik: '💡 **Trik Cepat UTBK**: Gaya berbanding terbalik dengan kuadrat jarak (1/r²). Jika jarak 2×, maka gaya menjadi **(½)² = ¼ kali semula**.'
                },
                {
                    id: 'fc7',
                    mapel: 'Kimia',
                    topik: 'Pengaruh Suhu terhadap Laju Reaksi',
                    tantangan: 'Jika setiap kenaikan ΔT suhu laju reaksi naik n kali lipat, tentukan rumus laju akhir (v₂)!',
                    rumus: 'v₂ = v₁ · n^[ (T₂ - T₁) / ΔT ]',
                    trik: '💡 **Trik Cepat UTBK**: Hitung dulu berapa kali kenaikan suhu terjadi [(T₂-T₁)/ΔT], lalu pangkatan n dengan angka tersebut.'
                },
                {
                    id: 'fc8',
                    mapel: 'Kimia',
                    topik: 'pH Larutan Penyangga / Buffer Asam',
                    tantangan: 'Bagaimanakah rumus menentukan konsentrasi [H⁺] dari campuran Asam Lemah dan Basa Konjugasinya?',
                    rumus: '[H⁺] = Ka · (mol Asam Lemah / mol Basa Konjugasi)',
                    trik: '💡 **Trik Cepat UTBK**: Selalu gunakan jumlah mol (mmol) reaktan yang **BERSISA (Asam Lemah)** setelah reaksi selesai.'
                },
                {
                    id: 'fc9',
                    mapel: 'Kimia',
                    topik: 'Potensial Sel Volta (E°sel)',
                    tantangan: 'Bagaimana rumus menentukan Potensial Sel Standar (E°sel) dari dua elektroda Katoda dan Anoda?',
                    rumus: 'E°sel = E°katoda - E°anoda',
                    trik: '💡 **Trik Cepat UTBK**: Unsur dengan E° lebih **POSITIF** selalu bertindak sebagai **KATODA** (Reduksi).'
                }
            ],

            materiDetails: {
                'mat': [
                    {
                        title: '1. Eksponen, Bentuk Akar & Logaritma (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Pengertian & Konsep Dasar:</strong> Eksponen adalah bentuk perkalian berulang dari suatu bilangan dengan dirinya sendiri. Logaritma adalah invers dari eksponensial (aⁿ = b ⇔ ᵃlog b = n). Digunakan dalam mengukur skala Richter gempa, pH larutan, dan bunga majemuk.',
                        visual: 'ᵃlog(b·c) = ᵃlog b + ᵃlog c | ᵃlog(b/c) = ᵃlog b - ᵃlog c | ᵃlog bⁿ = n · ᵃlog b',
                        tips: '<strong>Langkah Cepat Cerdas:</strong> Jika bertemu persamaan a^(f(x)) = a^(g(x)), samakan bilangan pokoknya terlebih dahulu, lalu f(x) = g(x).',
                        contohSoal: 'Jika ᵃlog b + ᵃlog b² = 12, tentukan nilai ᵃlog(a·b)!<br><strong>Jawaban Terperinci:</strong> ᵃlog b + 2 ᵃlog b = 12 ⇒ 3 ᵃlog b = 12 ⇒ ᵃlog b = 4. Maka ᵃlog(a·b) = ᵃlog a + ᵃlog b = 1 + 4 = 5.'
                    },
                    {
                        title: '2. Persamaan Kuadrat & Fungsi Kuadrat (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '<strong>Pengertian & Konsep Dasar:</strong> Persamaan kuadrat ax² + bx + c = 0. Grafiknya berupa parabola. Diskriminan D = b² - 4ac memprediksi jumlah dan sifat akar real.',
                        visual: 'Akar Vieta: x₁ + x₂ = -b/a | x₁·x₂ = c/a | Puncak Parabola: (-b / 2a , -D / 4a)',
                        tips: '<strong>Langkah Cepat Cerdas:</strong> Gunakan Rumus Vieta tanpa perlu mencari nilai akar satu per satu!',
                        contohSoal: 'x² - (k + 2)x + 16 = 0 memiliki dua akar kembar positif. Tentukan k!<br><strong>Jawaban Terperinci:</strong> D = 0 ⇒ (k+2)² - 64 = 0 ⇒ k+2 = ±8. Karena akar positif, x₁+x₂ = k+2 > 0 ⇒ k = 6.'
                    },
                    {
                        title: '3. Sistem Persamaan & Pertidaksamaan Linear (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'SPLTV terdiri atas 3 variabel. Digunakan untuk pemodelan linier dan optimasi keuntungan pada Program Linier.',
                        visual: 'Fungsi Sasaran: Z = ax + by | Garis Selidik: ax + by = k',
                        tips: 'Gunakan titik acuan (0,0) untuk menentukan daerah arsiran pertidaksamaan ax + by ≤ c.',
                        contohSoal: 'Maksimum f(x,y) = 3x + 4y pada x + y ≤ 5, x ≥ 0, y ≥ 0.<br><strong>Jawaban:</strong> Nilai maksimum di titik (0,5) = 3(0) + 4(5) = 20.'
                    },
                    {
                        title: '4. Matriks & Operasi Matriks (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Matriks adalah susunan bilangan dalam baris dan kolom. Perkalian A × B mensyaratkan kolom A = baris B.',
                        visual: 'Invers Matriks 2x2: A⁻¹ = (1 / det A) · [[d, -b], [-c, a]] | det A = ad - bc',
                        tips: 'Determinan invers matriks det(A⁻¹) = 1 / det(A). Tidak perlu cari bentuk inversnya!',
                        contohSoal: 'A = [[2, 1], [4, 3]]. Tentukan det(A⁻¹)!<br><strong>Jawaban:</strong> det(A) = 6 - 4 = 2. Maka det(A⁻¹) = 1/2.'
                    },
                    {
                        title: '5. Barisan & Deret Aritmetika dan Geometri (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Aritmetika memiliki beda (b) tetap. Geometri memiliki rasio (r) tetap. Deret geometri tak hingga konvergen mensyaratkan -1 < r < 1.',
                        visual: 'Un (Arit) = a + (n-1)b | Un (Geo) = a·rⁿ⁻¹ | S_∞ = a / (1 - r)',
                        tips: 'Hafalkan deret geometri tak hingga sebagai rumus "A-BAH" (a / (1-r)).',
                        contohSoal: 'Bola dijatuhkan dari 12 m dan memantul 2/3 kali tinggi sebelumnya. Hitung panjang lintasan total!<br><strong>Jawaban:</strong> 12 × ((3+2)/(3-2)) = 12 × 5 = 60 meter.'
                    },
                    {
                        title: '6. Turunan Fungsi Aljabar & Aplikasi (Kelas 12 / Fase F Lanjut)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Turunan f\'(x) mengukur laju perubahan instan. Aplikasi: menentukan garis singgung, interval naik/turun, dan titik stasioner (f\'(x) = 0).',
                        visual: 'f(x) = a xⁿ ⇒ f\'(x) = a·n xⁿ⁻¹ | Stasioner: f\'(x) = 0',
                        tips: 'Keuntungan maksimum pada fungsi ekonomi selalu tercapai saat turunan pertamanya sama dengan NOL.',
                        contohSoal: 'Tentukan x stasioner dari f(x) = x³ - 3x² - 9x + 5!<br><strong>Jawaban:</strong> f\'(x) = 3x² - 6x - 9 = 0 ⇒ x² - 2x - 3 = 0 ⇒ x = 3 atau x = -1.'
                    }
                ],
                'fis': [
                    {
                        title: '1. Besaran, Pengukuran & Vektor (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Pengukuran membandingkan besaran dengan standar SI. Alat ukur: Jangka Sorong (ketelitian 0,1 mm) dan Mikrometer Sekrup (ketelitian 0,01 mm).',
                        visual: 'Resultan Dua Vektor Tegak Lurus: R = √(F₁² + F₂²)',
                        tips: 'Skala Mikrometer = Skala Utama (mm) + (Skala Nonius × 0,01 mm).',
                        contohSoal: 'Skala utama 4,5 mm dan nonius 25 berhimpit pada mikrometer. Berapa tebalnya?<br><strong>Jawaban:</strong> 4,5 + (25 × 0,01) = 4,75 mm.'
                    },
                    {
                        title: '2. Kinematika Gerak Lurus & Parabola (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'GLB memiliki v konstan. GLBB memiliki percepatan a konstan. Gerak parabola memadukan GLB sumbu-X dan GLBB sumbu-Y.',
                        visual: 'GLBB: vₜ = v₀ + a·t | s = v₀t + ½at² | vₜ² = v₀² + 2as',
                        tips: 'Pada titik tertinggi gerak parabola, kecepatan arah vertikal v_y selalu sama dengan NOL.',
                        contohSoal: 'Dilempar vertikal ke atas v₀ = 20 m/s (g = 10 m/s²). Hitung h maks!<br><strong>Jawaban:</strong> vₜ² = v₀² - 2gh ⇒ 0 = 400 - 20h ⇒ h = 20 m.'
                    },
                    {
                        title: '3. Dinamika Gerak & Hukum Newton (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Hukum I Newton (Inersia): ΣF = 0. Hukum II Newton: ΣF = m·a. Hukum III Newton: F_aksi = -F_reaksi.',
                        visual: 'ΣF = m · a | Gaya Gesek: f_g = μ · N | Bidang Miring: F = m·g sin θ',
                        tips: 'Pada bidang miring licin, gaya pendorong searah kemiringan bidang selalu m·g·sin θ.',
                        contohSoal: 'Balok 4 kg ditarik gaya 20 N di lantai licin. Hitung percepatan!<br><strong>Jawaban:</strong> a = F/m = 20/4 = 5 m/s².'
                    },
                    {
                        title: '4. Usaha, Energi & Kekekalan Energi (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Usaha W = F · s cos θ. Energi Mekanik EM = EP + EK bernilai konstan jika tidak ada gaya gesekan luar.',
                        visual: 'EM = EP + EK | EP = m·g·h | EK = ½ m v²',
                        tips: 'Saat gerak jatuh bebas, penurunan EP sebanding dengan kenaikan EK (ΔEP = ΔEK).',
                        contohSoal: 'Benda 2 kg jatuh bebas dari 10 m (g=10). Hitung EK saat di ketinggian 2 m!<br><strong>Jawaban:</strong> EK₂ = EP₁ - EP₂ = 2(10)(10) - 2(10)(2) = 200 - 40 = 160 J.'
                    },
                    {
                        title: '5. Gelombang Bunyi & Efek Doppler (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Gelombang bunyi adalah gelombang longitudinal. Efek Doppler menjelaskan perubahan frekuensi akibat gerak relatif sumber dan pendengar.',
                        visual: 'Efek Doppler: f_p = [(v ± v_p) / (v ± v_s)] · f_s',
                        tips: 'Pendengar mendekat (+), Pendengar menjauh (-). Sumber mendekat (-), Sumber menjauh (+).',
                        contohSoal: 'Ambulans v_s = 20 m/s mendekati pengamat diam dengan sirine 640 Hz (v=340 m/s). Hitung f_p!<br><strong>Jawaban:</strong> f_p = (340 / (340 - 20)) × 640 = (340 / 320) × 640 = 680 Hz.'
                    },
                    {
                        title: '6. Listrik Dinamis & Hukum Kirchhoff (Kelas 12 / Fase F Lanjut)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Arus listrik I = Q/t. Hukum Ohm V = I·R. Hukum Kirchhoff I (arus masuk = keluar) & Kirchhoff II (ΣE + ΣI·R = 0 pada loop).',
                        visual: 'V = I · R | Seri: R_total = R₁ + R₂ | Paralel: 1/R_total = 1/R₁ + 1/R₂',
                        tips: 'Hambatan sejajar/paralel identik R terpasang n buah memiliki R_total = R / n.',
                        contohSoal: 'Dua hambatan 6 Ohm dipasang paralel, lalu diseri dengan hambatan 3 Ohm. Hitung R total!<br><strong>Jawaban:</strong> R_paralel = 6/2 = 3 Ohm. R_total = 3 + 3 = 6 Ohm.'
                    }
                ],
                'kim': [
                    {
                        title: '1. Struktur Atom & Konfigurasi Elektron (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Atom terdiri dari proton, neutron, dan elektron. Posisi elektron ditentukan oleh 4 bilangan kuantum: utama (n), azimut (l), magnetik (m), dan spin (s).',
                        visual: 'Konfigurasi: 1s² 2s² 2p⁶ 3s² 3p⁶ 4s² 3d¹⁰ | l: s=0, p=1, d=2, f=3',
                        tips: 'Jari-jari atom makin besar dari atas ke bawah dan makin kecil dari kiri ke kanan.',
                        contohSoal: 'Tentukan 4 bilangan kuantum elektron terakhir ₁₁Na (1s² 2s² 2p⁶ 3s¹)!<br><strong>Jawaban:</strong> n=3, l=0, m=0, s=+½.'
                    },
                    {
                        title: '2. Ikatan Kimia & Bentuk Molekul (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Ikatan Ionik (serah terima elektron) vs Ikatan Kovalen (pemakaian bersama). Teori VSEPR menentukan bentuk molekul berdasarkan PEI dan PEB.',
                        visual: 'AX₂ (Linear) | AX₃ (Trigonal Planar) | AX₄ (Tetrahedral) | AX₃E (Piramida Trigonal)',
                        tips: 'Jika atom pusat memiliki Pasangan Elektron Bebas (PEB > 0), molekul bersifat POLAR.',
                        contohSoal: 'Bentuk molekul CH₄ (C=6, H=1) menurut VSEPR adalah...<br><strong>Jawaban:</strong> PEI=4, PEB=0 ⇒ Tipe AX₄ (Tetrahedral).'
                    },
                    {
                        title: '3. Stoikiometri & Konsep Mol (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Mol adalah satuan jumlah zat. 1 mol = 6,02×10²³ partikel. Massa = mol × Mr. Volume gas STP (0°C, 1 atm) = mol × 22,4 L.',
                        visual: 'n = massa / Mr | n = V / 22.4 (STP) | Molaritas M = n / V(L)',
                        tips: 'Untuk mencari Pereaksi Pembatas, bagilah mol reaktan dengan koefisiennya. Nilai terkecil adalah pembatasnya.',
                        contohSoal: 'Hitung massa 0,5 mol H₂SO₄ (Ar H=1, S=32, O=16)!<br><strong>Jawaban:</strong> Mr = 98 g/mol. Massa = 0,5 × 98 = 49 gram.'
                    },
                    {
                        title: '4. Laju Reaksi & Faktor Pengaruh (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Laju reaksi adalah perubahan konsentrasi per satuan waktu. Ditingkatkan oleh konsentrasi, luas permukaan, suhu, dan katalis (menurunkan Energi Aktivasi Ea).',
                        visual: 'v = k [A]ˣ [B]ʸ | Suhu: v₂ = v₁ · n^[(T₂-T₁)/ΔT]',
                        tips: 'Katalis mempercepat reaksi dengan menurunkan Energi Aktivasi (Ea) tanpa mengubah ΔH reaksi.',
                        contohSoal: 'Suhu naik dari 20°C ke 50°C laju naik 8 kali. Setiap naik 10°C laju naik n kali. Berapa n?<br><strong>Jawaban:</strong> n^(30/10) = 8 ⇒ n³ = 8 ⇒ n = 2.'
                    },
                    {
                        title: '5. Larutan Penyangga / Buffer (Kelas 12 / Fase F Lanjut)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Buffer mempertahankan pH dari penambahan sedikit asam/basa. Terdiri dari Asam Lemah + Basa Konjugasinya.',
                        visual: 'Buffer Asam: [H⁺] = Ka · (mol asam lemah / mol basa konjugasi)',
                        tips: 'Ciri khas buffer adalah menyisakan komponen LEMAH setelah reaksi selesai.',
                        contohSoal: '100 mL CH₃COOH 0,1 M + 50 mL CH₃COONa 0,1 M (Ka=10⁻⁵).<br><strong>Jawaban:</strong> [H⁺] = 10⁻⁵ × (10/5) = 2×10⁻⁵ M ⇒ pH = 5 - log 2.'
                    },
                    {
                        title: '6. Elektrokimia: Sel Volta & Elektrolisis (Kelas 12 / Fase F Lanjut)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Sel Volta mengubah reaksi spontan menjadi energi listrik. KRAP: Katoda Reduksi (Positif). E°sel = E°katoda - E°anoda.',
                        visual: 'E°sel = E°katoda - E°anoda | Hukum Faraday I: w = (e · i · t) / 96500',
                        tips: 'Logaam dengan E° lebih POSITIF bertindak sebagai KATODA.',
                        contohSoal: 'E° Zn²⁺/Zn = -0,76 V, E° Cu²⁺/Cu = +0,34 V. Hitung E°sel!<br><strong>Jawaban:</strong> E°sel = (+0,34) - (-0,76) = +1,10 Volt.'
                    }
                ],
                'bio': [
                    {
                        title: '1. Ruang Lingkup Biologi & Keanekaragaman Hayati (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Keanekaragaman hayati mencakup 3 tingkat: Gen (variasi dalam 1 spesies), Jenis/Spesies (antar spesies dalam 1 famili), dan Ekosistem.',
                        visual: 'Tingkat Gen (Mawar merah/putih) → Tingkat Jenis (Kucing/Harimau) → Tingkat Ekosistem',
                        tips: 'Perbedaan warna atau varietas dalam SATU SPESIES yang sama tergolong tingkat GEN.',
                        contohSoal: 'Keanekaragaman warna mawar merah dan putih tergolong tingkat...<br><strong>Jawaban:</strong> Tingkat Gen.'
                    },
                    {
                        title: '2. Ekologi, Rantai Makanan & Siklus Nitrogen (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Aliran energi bersifat searah (Hukum 10%). Siklus Biogeokimia Nitrogen mencakup Fiksasi N₂, Nitrifikasi (Amunisi → Nitrit → Nitrat), Asimilasi, dan Denitrifikasi.',
                        visual: 'N₂ -> Fiksasi (Rhizobium) -> Amonia -> Nitritasi (Nitrosomonas) -> Nitratasi (Nitrobacter)',
                        tips: 'Bakteri Rhizobium bersimbiosis di bintil akar legum untuk fiksasi Nitrogen bebas.',
                        contohSoal: 'Pengubahan Amonia menjadi Nitrit oleh bakteri dinamakan...<br><strong>Jawaban:</strong> Nitritasi.'
                    },
                    {
                        title: '3. Biologi Sel & Transpor Membran (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Sel adalah unit dasar kehidupan. Transpor Pasif (Difusi, Osmosis) tanpa ATP. Transpor Aktif (Pompa Na-K, Endositosis) butuh ATP.',
                        visual: 'Osmosis: Perpindahan pelarut (air) dari Hipotonis → Hipertonis',
                        tips: 'Sel tumbuhan tidak pecah di lingkungan hipotonis karena memiliki Dinding Sel yang kuat (kondisi Turgid).',
                        contohSoal: 'Organel sel pencetak energi ATP melalui respirasi seluler adalah...<br><strong>Jawaban:</strong> Mitokondria.'
                    },
                    {
                        title: '4. Enzim & Respirasi Seluler (Kelas 12 / Fase F Lanjut)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Respirasi Aerob merombak glukosa menjadi 38 ATP melalui 4 tahap: Glikolisis, Dekarboksilasi Oksidatif, Siklus Krebs, dan Transpor Elektron.',
                        visual: 'Glikolisis (Sitoplasma) -> Krebs (Matriks) -> Transpor Elektron (Krista Mitokondria)',
                        tips: 'Tahap penghasil ATP terbanyak adalah Transpor Elektron (34 ATP).',
                        contohSoal: 'Di bagian sel manakah tahap Glikolisis terjadi?<br><strong>Jawaban:</strong> Sitoplasma (Sitosol).'
                    },
                    {
                        title: '5. Genetika & Sintesis Protein (Kelas 12 / Fase F Lanjut)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Sintesis protein terdiri dari Transkripsi (DNA cetak mRNA di nukleus) dan Translasi (tRNA baca kodon di ribosom). Basa N: A-T/U dan G-C.',
                        visual: 'DNA Antisense -> Transkripsi -> mRNA -> Translasi -> Rantai Asam Amino (Protein)',
                        tips: 'Rasio persilangan dihibrid heterozigot (AaBb × AaBb) selalu 9 : 3 : 3 : 1.',
                        contohSoal: 'Jika DNA antisense 5\'-TAC GGC-3\', tentukan urutan mRNA!<br><strong>Jawaban:</strong> 3\'-AUG CCG-5\'.'
                    }
                ],
                'eko': [
                    {
                        title: '1. Kelangkaan & Biaya Peluang (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Kelangkaan terjadi karena kebutuhan manusia tak terbatas sedangkan alat pemuas terbatas. Biaya Peluang adalah nilai kesempatan terbaik yang dilepaskan.',
                        visual: 'Biaya Peluang = Nilai Kesempatan Terbaik yang Ditinggalkan (Bukan Dijumlah)',
                        tips: 'Pilihlah satu nilai tertinggi di antara alternatif kesempatan yang dibatalkan.',
                        contohSoal: 'Lulusan SMA melepaskan tawaran kerja A (3,5 jt) dan B (4,5 jt) demi kuliah. Berapa biaya peluangnya?<br><strong>Jawaban:</strong> Rp 4.500.000 (Pilihan terbesar yang dilepas).'
                    },
                    {
                        title: '2. Keseimbangan Pasar & Elastisitas (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Harga Keseimbangan terjadi saat Qd = Qs. Elastisitas mengukur kepekaan perubahan jumlah akibat harga (Ed = %ΔQ / %ΔP).',
                        visual: 'Ekuilibrium: Qd = Qs | Ed > 1 (Elastis) | Ed < 1 (Inelastis)',
                        tips: 'Barang kebutuhan pokok (seperti beras) bersifat Inelastis (Ed < 1).',
                        contohSoal: 'Qd = 100 - 2P dan Qs = -20 + 4P. Tentukan harga keseimbangan P!<br><strong>Jawaban:</strong> 100 - 2P = -20 + 4P ⇒ 6P = 120 ⇒ P = 20.'
                    },
                    {
                        title: '3. PDB & Pendapatan Nasional (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'PDB/GDP menghitung total barang/jasa akhir dalam wilayah negara. Pendekatan pengeluaran: Y = C + I + G + (X - M).',
                        visual: 'Y = C + I + G + (X - M) | GNP = GDP + Pendapatan Neto Luar Negeri',
                        tips: 'Jika Ekspor X > Impor M, negara mengalami surplus perdagangan luar negeri.',
                        contohSoal: 'C=300, I=150, G=200, X=100, M=80 (Triliun). Hitung PDB!<br><strong>Jawaban:</strong> Y = 300 + 150 + 200 + (100 - 80) = 670 Triliun.'
                    },
                    {
                        title: '4. Kebijakan Fiskal & Moneter (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Fiskal diatur Pemerintah (Pajak & Belanja Negara). Moneter diatur Bank Sentral BI (Suku Bunga, Operasi Pasar Terbuka SBI, Diskonto).',
                        visual: 'Atasi Inflasi: Naikkan Pajak & Suku Bunga | Atasi Resesi: Turunkan Pajak & Suku Bunga',
                        tips: 'Fiskal berhubungan dengan PAJAK; Moneter berhubungan dengan SUKU BUNGA & UANG BEREDAR.',
                        contohSoal: 'Kebijakan moneter BI menaikkan suku bunga bertujuan untuk...<br><strong>Jawaban:</strong> Mengurangi jumlah uang beredar dan menekan inflasi.'
                    },
                    {
                        title: '5. Akuntansi Dasar & Jurnal Umum (Kelas 12 / Fase F Lanjut)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Persamaan Dasar: Aset = Utang + Modal. Saldo Normal: Aset & Beban bertambah di DEBET; Utang, Modal & Pendapatan bertambah di KREDIT.',
                        visual: 'Aset & Beban (Naik = Debet) | Utang, Modal, Pendapatan (Naik = Kredit)',
                        tips: 'Membeli peralatan secara kredit ⇒ Peralatan (D), Utang Usaha (K).',
                        contohSoal: 'Beli komputer Rp 8 jt secara kredit. Analisis jurnalnya adalah...<br><strong>Jawaban:</strong> Peralatan (D) Rp 8.000.000; Utang Usaha (K) Rp 8.000.000.'
                    }
                ],
                'sos': [
                    {
                        title: '1. Sosiologi Sebagai Ilmu & Ciri-Cirinya (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Sosiologi mempelajari fakta sosial masyarakat. Ciri: Empiris (fakta), Teoritis (abstraksi), Kumulatif (memperbaiki teori), dan Non-Etis.',
                        visual: 'Ciri Sosiologi: Empiris, Teoritis, Kumulatif, Non-Etis',
                        tips: 'Ciri Non-Etis berarti sosiolog tidak menilai baik/buruknya fakta, melainkan menjelaskan alasannya.',
                        contohSoal: 'Sosiolog meneliti kemacetan tanpa menyalahkan siapapun. Ciri sosiologi ini adalah...<br><strong>Jawaban:</strong> Non-Etis.'
                    },
                    {
                        title: '2. Nilai & Tingkatan Norma Sosial (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Norma menjaga nilai sosial. 4 Tingkatan norma berdasarkan sanksinya: Cara (Usage), Kebiasaan (Folkways), Tata Kelakuan (Mores), dan Adat Istiadat (Custom).',
                        visual: 'Sanksi Ringan -> Cara -> Kebiasaan -> Tata Kelakuan -> Adat Istiadat -> Sanksi Berat',
                        tips: 'Teguran ringan atas ketidakrapian Pakaian tergolong pelanggaran norma Cara (Usage).',
                        contohSoal: 'Ditegur karena makan sambil bersendawa merupakan pelanggaran...<br><strong>Jawaban:</strong> Norma Cara (Usage).'
                    },
                    {
                        title: '3. Stratifikasi vs Diferensiasi Sosial (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Stratifikasi adalah pelapisan vertikal (hirarki kekayaan/pendidikan). Diferensiasi adalah pengelompokan horizontal (sejajar suku/agama/profesi).',
                        visual: 'Stratifikasi (Vertikal/Hirarki) vs Diferensiasi (Horizontal/Kesetaraan)',
                        tips: 'Keberagaman Suku Bangsa dan Agama bersifat Diferensiasi Sosial (sejajar).',
                        contohSoal: 'Keragaman profesi seperti guru, dokter, dan petani tergolong...<br><strong>Jawaban:</strong> Diferensiasi Sosial.'
                    },
                    {
                        title: '4. Konflik Sosial & Bentuk Akomodasi (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Akomodasi adalah cara penyelesaian konflik. Mediasi (penasihat netral), Arbitrase (keputusan mengikat), Ajudikasi (pengadilan).',
                        visual: 'Mediasi (Penasihat) | Arbitrase (Mengikat) | Ajudikasi (Pengadilan)',
                        tips: 'Kata kunci Ajudikasi adalah jalur hukum atau Pengadilan Negeri.',
                        contohSoal: 'Penyelesaian sengketa tanah warga melalui Pengadilan Negeri dinamakan...<br><strong>Jawaban:</strong> Ajudikasi.'
                    }
                ],
                'geo': [
                    {
                        title: '1. Prinsip Geografi & 10 Konsep Dasar (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '4 Prinsip: Distribusi (persebaran), Interelasi (sebab-akibat), Deskripsi (penjelasan/peta), dan Korologi (gabungan komprehensif).',
                        visual: 'Prinsip Korologi = Distribusi + Interelasi + Deskripsi secara Komprehensif',
                        tips: 'Konsep Diferensiasi Area membandingkan keunikan dua wilayah berbeda.',
                        contohSoal: 'Banjir Jakarta akibat penggundulan hutan di Bogor sesuai prinsip...<br><strong>Jawaban:</strong> Prinsip Interelasi.'
                    },
                    {
                        title: '2. Dinamika Litosfer & Siklus Batuan (Kelas 10 / Fase E)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Litosfer adalah kulit bumi. Tenaga Endogen (Tektonisme, Vulkanisme, Seisme) vs Tenaga Eksogen (Pelapukan, Erosi, Sedimentasi).',
                        visual: 'Magma -> Batuan Beku -> Batuan Sedimen -> Batuan Metamorf (Suhu/Tekanan Tinggi)',
                        tips: 'Batu Marmer berasal dari batuan sedimen Batu Kapur yang mengalami suhu & tekanan tinggi.',
                        contohSoal: 'Batu kapur yang mengalami suhu dan tekanan tinggi berubah menjadi batu...<br><strong>Jawaban:</strong> Batu Marmer (Metamorf).'
                    },
                    {
                        title: '3. Dinamika Atmosfer & Lapisan Udara (Kelas 11 / Fase F)',
                        kurikulum: 'K13 & Merdeka',
                        summary: '5 Lapisan Atmosfer: Troposfer (cuaca & hujan), Stratosfer (Ozon UV), Mesosfer (pembakar meteor), Termosfer (pemantul radio), Eksosfer.',
                        visual: 'Troposfer (Cuaca) -> Stratosfer (Ozon) -> Mesosfer (Meteor) -> Termosfer (Radio)',
                        tips: 'Dinamika cuaca harian manusia HANYA berlangsung di Troposfer.',
                        contohSoal: 'Lapisan atmosfer tempat terjadinya hujan dan pembentukan awan adalah...<br><strong>Jawaban:</strong> Troposfer.'
                    },
                    {
                        title: '4. Penginderaan Jauh & SIG (Kelas 12 / Fase F Lanjut)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'SIG mengolah data spasial komputer. Penginderaan Jauh merekam citra satelit/udara. Teknik Overlay peta untuk menentukan lokasi potensial.',
                        visual: 'Overlay SIG: Peta Lereng + Peta Hujan -> Peta Rawan Longsor',
                        tips: 'Unsur interpretasi citra: Bentuk, Ukuran, Rona, Tekstur, Pola, Bayangan, Situs, Asosiasi.',
                        contohSoal: 'Lapangan bola pada foto udara dikenali dari bentuk persegi panjang dan rumput halus. Unsur yang digunakan adalah...<br><strong>Jawaban:</strong> Bentuk dan Tekstur.'
                    }
                ],
                'lit': [
                    {
                        title: '1. Bahasa Indonesia: Ide Pokok & Paragraf (SNBT)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Ide Pokok adalah inti paragraf. Paragraf Deduktif (ide utama di awal). Paragraf Induktif (ide utama di akhir, ditandai: oleh karena itu, dengan demikian).',
                        visual: 'Deduktif (Kalimat Pertama) vs Induktif (Kalimat Terakhir)',
                        tips: 'Bacalah kalimat pertama dan kalimat terakhir paragraf terlebih dahulu untuk penentuan cepat.',
                        contohSoal: 'Tentukan kalimat utama paragraf deduktif!<br><strong>Jawaban:</strong> Berada di kalimat pertama paragraf.'
                    },
                    {
                        title: '2. English Comprehension: Main Idea & Author\'s Tone (SNBT)',
                        kurikulum: 'K13 & Merdeka',
                        summary: 'Main idea conveys the primary point. Author\'s Tone expresses feelings/attitudes (Critical, Objective, Optimistic, Neutral).',
                        visual: 'Tone Types: Objective (Factual) | Critical (Disapproving) | Optimistic (Positive)',
                        tips: 'Positive adjectives indicate an optimistic tone; critical adjectives indicate disapproval.',
                        contohSoal: 'Text uses words like "revolutionary" and "unparalleled solution". The author\'s tone is...<br><strong>Jawaban:</strong> Optimistic / Supportive.'
                    }
                ]
            },

            simulasiBank: {
                'utbk-pk': {
                    title: 'UTBK SNBT - Pengetahuan Kuantitatif (PK)',
                    durasiMinutes: 15,
                    soal: [
                        {
                            id: 'q1',
                            pertanyaan: 'Diketahui persamaan kuadrat x² - (k + 2)x + 16 = 0 memiliki dua akar real positif yang sama (kembar). Nilai k yang memenuhi adalah...',
                            pilihan: ['A. 6 atau -10', 'B. 6 saja', 'C. 8 atau -8', 'D. 10 saja', 'E. -6 saja'],
                            kunci: 'B. 6 saja',
                            solusiLengkap: 'D = b² - 4ac = 0 ⇒ (-(k+2))² - 64 = 0 ⇒ k+2 = ±8. Uji syarat positif (x₁+x₂ > 0) menghasilkan k = 6.'
                        },
                        {
                            id: 'q2',
                            pertanyaan: 'Jika 3ⁿ⁺¹ + 3ⁿ = 36, maka nilai dari 2ⁿ adalah...',
                            pilihan: ['A. 2', 'B. 4', 'C. 8', 'D. 16', 'E. 32'],
                            kunci: 'B. 4',
                            solusiLengkap: '3ⁿ(3 + 1) = 36 ⇒ 3ⁿ(4) = 36 ⇒ 3ⁿ = 9 ⇒ n = 2. Maka 2ⁿ = 2² = 4.'
                        }
                    ]
                },
                'tka-saintek': {
                    title: 'TKA Saintek - Fisika HOTS Master',
                    durasiMinutes: 15,
                    soal: [
                        {
                            id: 'q1_tka',
                            pertanyaan: 'Benda bermassa 2 kg ditarik gaya F = 20 N membentuk sudut 60° terhadap horizontal pada lantai licin. Hitung percepatan benda!',
                            pilihan: ['A. 5 m/s²', 'B. 10 m/s²', 'C. 5√3 m/s²', 'D. 20 m/s²', 'E. 10√3 m/s²'],
                            kunci: 'A. 5 m/s²',
                            solusiLengkap: 'F_x = F cos(60°) = 20 × 0,5 = 10 N. a = F_x / m = 10 / 2 = 5 m/s².'
                        }
                    ]
                },
                'lit-ind-eng': {
                    title: 'Literasi Bahasa & Penalaran Teks',
                    durasiMinutes: 10,
                    soal: [
                        {
                            id: 'q1_lit',
                            pertanyaan: 'Pemanasan global memicu percepatan pencairan es kutub yang mengancam pemukiman pesisir. Ide pokok kalimat tersebut adalah...',
                            pilihan: [
                                'A. Pencairan es kutub terjadi di mana-mana.',
                                'B. Dampak pemanasan global terhadap pencairan es dan wilayah pesisir.',
                                'C. Pemukiman pesisir terancam tenggelam.',
                                'D. Kenaikan permukaan air laut hanya di kutub.',
                                'E. Pemanasan global adalah fenomena biasa.'
                            ],
                            kunci: 'B. Dampak pemanasan global terhadap pencairan es dan wilayah pesisir.',
                            solusiLengkap: 'Ide pokok merangkum sebab-akibat fenomena secara utuh.'
                        }
                    ]
                }
            }
        };

        // UI Toast Notification System
        function showToast(message, type = 'success') {
            const container = document.getElementById('toast-container');
            if (!container) return;
            const toast = document.createElement('div');
            toast.className = `px-4 py-3 rounded-2xl shadow-2xl text-xs font-bold text-white flex items-center gap-2 fade-in backdrop-blur-lg border ${type === 'success' ? 'bg-emerald-900/90 border-emerald-500/50' : 'bg-rose-900/90 border-rose-500/50'}`;
            toast.innerHTML = `<i data-lucide="${type === 'success' ? 'check-circle' : 'alert-circle'}" class="w-4 h-4"></i> ${message}`;
            container.appendChild(toast);
            lucide.createIcons();
            setTimeout(() => {
                toast.style.opacity = '0';
                toast.style.transition = 'all 0.3s ease';
                setTimeout(() => toast.remove(), 300);
            }, 3000);
        }

        // View Switcher Engine
        function switchView(viewName) {
            if (state.timerInterval) {
                clearInterval(state.timerInterval);
                state.timerInterval = null;
            }
            if (state.autoFlipTimer) {
                clearInterval(state.autoFlipTimer);
                state.autoFlipTimer = null;
                state.isAutoFlipping = false;
            }

            state.activeView = viewName;
            updateGamificationUI();

            ['home', 'materi', 'flashcards', 'utbk', 'riwayat'].forEach(v => {
                const el = document.getElementById(`nav-${v}`);
                if (el) {
                    if (v === viewName) {
                        el.className = "px-3.5 py-2 rounded-xl text-white bg-purple-600 transition flex items-center gap-1.5 font-bold shadow-md shadow-purple-600/30";
                    } else {
                        el.className = "px-3.5 py-2 rounded-xl text-slate-300 hover:text-white transition flex items-center gap-1.5 font-medium";
                    }
                }

                const mobEl = document.getElementById(`mob-${v}`);
                if (mobEl) {
                    if (v === viewName) {
                        mobEl.className = "flex flex-col items-center gap-1 text-purple-400 font-bold";
                    } else {
                        mobEl.className = "flex flex-col items-center gap-1 text-slate-400 font-medium";
                    }
                }
            });

            const content = document.getElementById('app-content');
            if (viewName === 'home') content.innerHTML = renderHome();
            else if (viewName === 'materi') content.innerHTML = renderMateriScreen();
            else if (viewName === 'flashcards') content.innerHTML = renderFlashcardsScreen();
            else if (viewName === 'utbk') content.innerHTML = renderUTBKScreen();
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
                    <div onclick="selectSearchResult('${res.mapelId}')" class="p-3 hover:bg-slate-800 rounded-xl cursor-pointer transition border-b border-slate-800/60 last:border-0">
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

        // Render Home Component
        function renderHome() {
            return `
                <div class="fade-in">
                    <!-- Hero Banner -->
                    <div class="relative rounded-3xl gradient-brand p-8 sm:p-12 overflow-hidden border border-slate-800/80 shadow-2xl mb-12">
                        <div class="absolute -right-20 -bottom-20 w-96 h-96 bg-purple-600/10 rounded-full blur-3xl pointer-events-none"></div>
                        <div class="relative z-10 max-w-3xl">
                            <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-purple-500/10 border border-purple-500/20 text-purple-300 text-xs font-semibold mb-6">
                                <i data-lucide="sparkles" class="w-4 h-4 text-purple-400"></i>
                                <span>Edisi Terintegrasi Google Gemini AI & Bank Materi Super Lengkap</span>
                            </div>
                            <h1 class="text-3xl sm:text-5xl font-black text-white tracking-tight mb-4 leading-tight">
                                Kuasai Konsep SMA & Taklukkan <span class="bg-clip-text text-transparent gradient-gemini">UTBK SNBT 2026</span>.
                            </h1>
                            <p class="text-slate-300 text-xs sm:text-sm mb-8 leading-relaxed">
                                Bank modul pembelajaran terlengkap seluruh mata pelajaran SMA, **Flashcard Rumus Auto-Flip**, serta pendampingan **Gemini AI Super Tutor**.
                            </p>
                            <div class="flex flex-wrap gap-4">
                                <button onclick="switchView('materi')" class="gradient-gemini text-white font-extrabold px-6 py-3.5 rounded-2xl shadow-lg shadow-purple-500/25 hover:opacity-95 transition flex items-center gap-2 text-xs sm:text-sm">
                                    <i data-lucide="book-open" class="w-4 h-4"></i> Pelajari Modul Terperinci
                                </button>
                                <button onclick="switchView('flashcards')" class="bg-slate-800/90 border border-slate-700 text-white font-extrabold px-6 py-3.5 rounded-2xl hover:bg-slate-800 transition flex items-center gap-2 text-xs sm:text-sm">
                                    <i data-lucide="layers" class="w-4 h-4 text-pink-400"></i> Flashcards Rumus Cepat
                                </button>
                            </div>
                        </div>
                    </div>

                    <!-- Subject Grid Section -->
                    <div class="mb-12">
                        <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4 mb-6">
                            <div>
                                <h2 class="text-2xl font-black text-white tracking-tight">Mata Pelajaran SMA (Lengkap)</h2>
                                <p class="text-slate-400 text-xs sm:text-sm">Pilih kurikulum untuk menyesuaikan struktur Fase/Kelas Anda</p>
                            </div>
                            <div class="bg-slate-900/90 p-1 rounded-2xl border border-slate-800 flex gap-1 text-xs font-bold">
                                <button onclick="setKurikulum('Merdeka')" class="px-4 py-2 rounded-xl transition ${state.selectedKurikulum === 'Merdeka' ? 'bg-purple-600 text-white shadow-md shadow-purple-600/30' : 'text-slate-400 hover:text-white'}">Kurikulum Merdeka</button>
                                <button onclick="setKurikulum('K13')" class="px-4 py-2 rounded-xl transition ${state.selectedKurikulum === 'K13' ? 'bg-purple-600 text-white shadow-md shadow-purple-600/30' : 'text-slate-400 hover:text-white'}">Kurikulum 2013 (K13)</button>
                            </div>
                        </div>

                        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-5">
                            ${db.mapel.map(m => `
                                <div class="gradient-card border border-slate-800 hover:border-purple-500/50 p-5 rounded-2xl transition duration-300 hover:-translate-y-1 group cursor-pointer shadow-lg" onclick="openDetailMapel('${m.id}')">
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
                </div>
            `;
        }

        function setKurikulum(k) {
            state.selectedKurikulum = k;
            switchView('home');
        }

        // FLASHCARDS HAFALAN ENGINE
        function renderFlashcardsScreen() {
            filterFlashcards();
            const currentCard = state.filteredFlashcards[state.flashcardsIndex] || state.filteredFlashcards[0];

            return `
                <div class="fade-in max-w-4xl mx-auto">
                    <div class="flex flex-col md:flex-row md:items-center justify-between gap-4 mb-8">
                        <div>
                            <div class="flex items-center gap-2 mb-1">
                                <span class="text-[10px] font-extrabold uppercase px-2.5 py-0.5 rounded-full bg-pink-500/20 text-pink-300 border border-pink-500/30">Hafalan Cepat</span>
                                <span class="text-xs text-slate-400">Matematika, Fisika, Kimia</span>
                            </div>
                            <h1 class="text-3xl font-black text-white tracking-tight">Flashcard Rumus & Konsep Core</h1>
                        </div>
                        
                        <div class="bg-slate-900/90 p-1.5 rounded-2xl border border-slate-800 flex flex-wrap gap-1 text-xs font-bold">
                            ${['Semua', 'Matematika', 'Fisika', 'Kimia'].map(cat => `
                                <button onclick="setFlashcardCategory('${cat}')" class="px-3.5 py-1.5 rounded-xl transition ${state.flashcardsCategory === cat ? 'bg-purple-600 text-white shadow-md shadow-purple-600/30' : 'text-slate-400 hover:text-white'}">
                                    ${cat}
                                </button>
                            `).join('')}
                        </div>
                    </div>

                    <div class="bg-slate-900/80 border border-slate-800 p-4 rounded-2xl mb-6 flex flex-wrap items-center justify-between gap-4 backdrop-blur-md">
                        <div class="flex items-center gap-3">
                            <button onclick="toggleAutoFlip()" class="px-4 py-2 ${state.isAutoFlipping ? 'bg-rose-600 hover:bg-rose-500' : 'gradient-gemini hover:opacity-90'} text-white font-black text-xs rounded-xl transition shadow-lg flex items-center gap-2">
                                <i data-lucide="${state.isAutoFlipping ? 'pause' : 'play'}" class="w-4 h-4 fill-current"></i>
                                <span>${state.isAutoFlipping ? 'Hentikan Auto-Flip' : 'Mulai Mode Auto-Flip'}</span>
                            </button>
                            
                            <select id="autoflip-speed" onchange="changeAutoFlipSpeed(this.value)" class="bg-slate-950 border border-slate-700 text-slate-300 text-xs rounded-xl px-3 py-2 focus:outline-none focus:border-purple-500 font-semibold">
                                <option value="3000">Cepat (3s / Balik)</option>
                                <option value="5000" selected>Sedang (5s / Balik)</option>
                                <option value="8000">Santai (8s / Balik)</option>
                            </select>
                        </div>

                        <div class="flex items-center gap-3">
                            <button onclick="shuffleFlashcards()" class="px-3.5 py-2 bg-slate-800 hover:bg-slate-700 text-purple-300 border border-purple-500/30 rounded-xl transition text-xs font-bold flex items-center gap-1.5" title="Acak Dek">
                                <i data-lucide="shuffle" class="w-4 h-4"></i> Acak Dek
                            </button>
                            <span class="text-xs font-mono font-extrabold text-slate-400 bg-slate-950 px-3 py-2 rounded-xl border border-slate-800">
                                Kartu <span class="text-purple-400">${state.flashcardsIndex + 1}</span> dari ${state.filteredFlashcards.length}
                            </span>
                        </div>
                    </div>

                    <div class="perspective-1000 w-full h-[380px] sm:h-[340px] cursor-pointer group mb-6" onclick="flipFlashcard()">
                        <div id="flashcard-inner" class="relative w-full h-full transform-style-3d ${state.isFlashcardFlipped ? 'rotate-y-180' : ''}">
                            <div class="absolute inset-0 w-full h-full rounded-3xl gradient-card border-2 border-purple-500/40 p-6 sm:p-8 flex flex-col justify-between backface-hidden shadow-2xl group-hover:border-purple-400 transition">
                                <div class="flex justify-between items-start">
                                    <span class="text-[10px] uppercase font-extrabold px-3 py-1 rounded-full bg-purple-500/20 text-purple-300 border border-purple-500/30">
                                        📌 ${currentCard.mapel}
                                    </span>
                                    <span class="text-xs text-slate-500 font-bold flex items-center gap-1">
                                        <i data-lucide="rotate-cw" class="w-3.5 h-3.5"></i> Ketuk untuk Balik
                                    </span>
                                </div>
                                <div class="my-auto text-center px-4">
                                    <h4 class="text-xs font-extrabold uppercase text-pink-400 mb-2">${currentCard.topik}</h4>
                                    <p class="text-base sm:text-xl font-bold text-white leading-relaxed">${currentCard.tantangan}</p>
                                </div>
                                <div class="text-center text-[11px] text-slate-400 font-semibold border-t border-slate-800/80 pt-3">
                                    💡 *Dapatkah kamu mengingat rumusnya sebelum dibalik?*
                                </div>
                            </div>

                            <div class="absolute inset-0 w-full h-full rounded-3xl bg-slate-900 border-2 border-emerald-500/50 p-6 sm:p-8 flex flex-col justify-between backface-hidden rotate-y-180 shadow-2xl">
                                <div class="flex justify-between items-start">
                                    <span class="text-[10px] uppercase font-extrabold px-3 py-1 rounded-full bg-emerald-500/20 text-emerald-300 border border-emerald-500/30">
                                        ✓ Jawaban & Rumus Utama
                                    </span>
                                    <span class="text-xs text-slate-500 font-bold flex items-center gap-1">
                                        <i data-lucide="rotate-cw" class="w-3.5 h-3.5"></i> Sisi Belakang
                                    </span>
                                </div>

                                <div class="my-auto text-center space-y-4">
                                    <div class="bg-slate-950 p-4 rounded-2xl border border-emerald-500/30 font-mono text-base sm:text-lg text-emerald-300 font-black shadow-inner">
                                        ${currentCard.rumus}
                                    </div>
                                    <p class="text-xs sm:text-sm text-slate-300 leading-relaxed max-w-xl mx-auto">
                                        ${currentCard.trik}
                                    </p>
                                </div>

                                <div class="flex justify-between items-center pt-3 border-t border-slate-800">
                                    <button onclick="event.stopPropagation(); askGeminiTopic('Rumus Hafalan: ${currentCard.topik}')" class="text-purple-400 hover:text-purple-300 text-xs font-extrabold flex items-center gap-1.5">
                                        <i data-lucide="sparkles" class="w-4 h-4 text-pink-400"></i>
                                        <span>Tanyakan Rumus Ini ke Gemini AI</span>
                                    </button>
                                    <span class="text-[10px] text-slate-500 font-mono">Nihiluxxy Formula Engine</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="flex justify-between items-center gap-4">
                        <button onclick="prevFlashcard()" class="flex-1 py-3.5 bg-slate-900 border border-slate-700 text-white font-extrabold text-xs rounded-2xl transition flex items-center justify-center gap-2 shadow-lg">
                            <i data-lucide="chevron-left" class="w-4 h-4"></i> Kartu Sebelumnya
                        </button>
                        <button onclick="nextFlashcard()" class="flex-1 py-3.5 gradient-gemini text-white font-black text-xs rounded-2xl transition flex items-center justify-center gap-2 shadow-lg shadow-purple-500/20">
                            Kartu Berikutnya <i data-lucide="chevron-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>
            `;
        }

        function filterFlashcards() {
            if (state.flashcardsCategory === 'Semua') {
                state.filteredFlashcards = [...db.flashcards];
            } else {
                state.filteredFlashcards = db.flashcards.filter(f => f.mapel === state.flashcardsCategory);
            }
            if (state.flashcardsIndex >= state.filteredFlashcards.length) {
                state.flashcardsIndex = 0;
            }
        }

        function setFlashcardCategory(cat) {
            state.flashcardsCategory = cat;
            state.flashcardsIndex = 0;
            state.isFlashcardFlipped = false;
            switchView('flashcards');
        }

        function flipFlashcard() {
            state.isFlashcardFlipped = !state.isFlashcardFlipped;
            const cardInner = document.getElementById('flashcard-inner');
            if (cardInner) {
                if (state.isFlashcardFlipped) cardInner.classList.add('rotate-y-180');
                else cardInner.classList.remove('rotate-y-180');
            }
        }

        function nextFlashcard() {
            state.isFlashcardFlipped = false;
            state.flashcardsIndex = (state.flashcardsIndex + 1) % state.filteredFlashcards.length;
            if (state.flashcardsIndex === state.filteredFlashcards.length - 1) {
                addXP(10, 'Menamatkan Dek Flashcards');
            }
            switchView('flashcards');
        }

        function prevFlashcard() {
            state.isFlashcardFlipped = false;
            state.flashcardsIndex = (state.flashcardsIndex - 1 + state.filteredFlashcards.length) % state.filteredFlashcards.length;
            switchView('flashcards');
        }

        function shuffleFlashcards() {
            for (let i = db.flashcards.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [db.flashcards[i], db.flashcards[j]] = [db.flashcards[j], db.flashcards[i]];
            }
            state.flashcardsIndex = 0;
            state.isFlashcardFlipped = false;
            showToast('Dek kartu berhasil diacak!');
            switchView('flashcards');
        }

        function toggleAutoFlip() {
            state.isAutoFlipping = !state.isAutoFlipping;
            if (state.isAutoFlipping) {
                showToast('Mode Auto-Flip Diaktifkan!');
                startAutoFlipTimer();
            } else {
                if (state.autoFlipTimer) clearInterval(state.autoFlipTimer);
                state.autoFlipTimer = null;
                showToast('Mode Auto-Flip Dihentikan.');
            }
            switchView('flashcards');
        }

        function changeAutoFlipSpeed(valMs) {
            state.autoFlipIntervalMs = parseInt(valMs);
            if (state.isAutoFlipping) startAutoFlipTimer();
        }

        function startAutoFlipTimer() {
            if (state.autoFlipTimer) clearInterval(state.autoFlipTimer);
            state.autoFlipTimer = setInterval(() => {
                if (!state.isFlashcardFlipped) {
                    flipFlashcard();
                } else {
                    nextFlashcard();
                }
            }, state.autoFlipIntervalMs);
        }

        // Render Modul Materi Screen
        function renderMateriScreen() {
            return `
                <div class="fade-in">
                    <div class="mb-8">
                        <h1 class="text-3xl font-black text-white tracking-tight">Modul Pembelajaran SMA (Kelas 10-12)</h1>
                        <p class="text-slate-400 text-xs sm:text-sm mt-1">Penjelasan mendalam, analogi intuitif, rumus visual, serta pendampingan langsung dari Gemini AI.</p>
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
                                        <span class="text-[10px] text-slate-500 font-medium">${(db.materiDetails[m.id] || []).length} Modul Terperinci</span>
                                    </div>
                                </button>
                            `).join('')}
                        </div>
                        <div id="materi-reader" class="lg:col-span-8 gradient-card border border-slate-800 rounded-3xl p-6 sm:p-8 shadow-2xl">
                        </div>
                    </div>
                </div>
            `;
        }

        function openDetailMapel(mapelId) {
            state.selectedSubject = mapelId;
            if (state.activeView !== 'materi') switchView('materi');

            addXP(5, 'Membaca Modul');

            db.mapel.forEach(m => {
                const btn = document.getElementById(`mapel-btn-${m.id}`);
                if (btn) {
                    if (m.id === mapelId) {
                        btn.className = "w-full text-left p-4 rounded-2xl bg-slate-800 border border-purple-500/80 flex items-center gap-3.5 group shadow-lg";
                    } else {
                        btn.className = "w-full text-left p-4 rounded-2xl bg-slate-900/60 border border-slate-800 hover:bg-slate-800 hover:border-purple-500/50 transition flex items-center gap-3.5 group";
                    }
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
                                <p class="text-xs text-purple-400 font-extrabold mt-0.5">Cakupan Kelas 10, 11, & 12 • Kurikulum K13 & Merdeka</p>
                            </div>
                        </div>
                    </div>
                    <div class="space-y-6">
                        ${materiList.map((mat, idx) => {
                            const isBookmarked = state.bookmarks.includes(mat.title);
                            return `
                                <div class="bg-slate-900/90 border border-slate-800 p-6 rounded-2xl shadow-md relative">
                                    <button onclick="toggleBookmark('${mat.title}')" class="absolute top-6 right-6 text-slate-500 hover:text-amber-400 transition" title="Tandai Favorit">
                                        <i data-lucide="bookmark" class="w-5 h-5 ${isBookmarked ? 'text-amber-400 fill-amber-400' : ''}"></i>
                                    </button>
                                    <div class="flex items-center justify-between mb-3 pr-8">
                                        <span class="text-[10px] font-extrabold uppercase bg-purple-500/20 text-purple-300 px-3 py-1 rounded-full border border-purple-500/30">${mat.kurikulum}</span>
                                        <span class="text-xs text-slate-500 font-mono">Modul #${idx + 1}</span>
                                    </div>
                                    <h3 class="text-lg font-extrabold text-white mb-3 leading-snug">${mat.title}</h3>
                                    <div class="text-slate-300 text-xs sm:text-sm mb-4 leading-relaxed">${mat.summary}</div>
                                    
                                    <div class="bg-slate-950 p-4 rounded-xl font-mono text-xs text-purple-300 mb-4 border border-slate-800/80 text-center overflow-x-auto shadow-inner">
                                        ${mat.visual}
                                    </div>

                                    <div class="bg-amber-500/10 border-l-4 border-amber-500 p-4 rounded-r-xl text-xs text-amber-200 mb-4 leading-relaxed">
                                        ${mat.tips}
                                    </div>

                                    <div class="bg-slate-950/80 border border-slate-800 p-4 rounded-xl text-xs text-slate-300 leading-relaxed mb-4">
                                        <span class="text-emerald-400 font-extrabold block mb-2 text-xs">📝 Contoh Soal & Pembahasan HOTS UTBK:</span>
                                        ${mat.contohSoal}
                                    </div>

                                    <button onclick="askGeminiTopic('${mat.title}')" class="w-full py-2.5 bg-purple-950/60 hover:bg-purple-900/80 border border-purple-500/40 text-purple-300 font-extrabold text-xs rounded-xl transition flex items-center justify-center gap-2">
                                        <i data-lucide="sparkles" class="w-4 h-4 text-pink-400"></i>
                                        <span>💡 Tanyakan Konsep Ini ke Gemini AI</span>
                                    </button>
                                </div>
                            `;
                        }).join('')}
                    </div>
                `;
                lucide.createIcons();
            }
        }

        // Render UTBK & Gemini Quiz Screen
        function renderUTBKScreen() {
            return `
                <div class="fade-in">
                    <div class="mb-8">
                        <h1 class="text-3xl font-black text-white tracking-tight">Simulasi UTBK & Gemini HOTS Generator</h1>
                        <p class="text-slate-400 text-xs sm:text-sm mt-1">Uji pemahaman dengan simulasi standar atau buatkan soal latihan HOTS instan menggunakan Gemini AI.</p>
                    </div>

                    <!-- Gemini HOTS Quiz Generator Card -->
                    <div class="gradient-card border border-purple-500/40 p-6 sm:p-8 rounded-3xl mb-8 shadow-2xl relative overflow-hidden">
                        <div class="flex items-center gap-3 mb-4">
                            <div class="p-3 gradient-gemini rounded-2xl text-white shadow-lg">
                                <i data-lucide="sparkles" class="w-6 h-6"></i>
                            </div>
                            <div>
                                <h3 class="text-lg font-black text-white">Gemini Dynamic HOTS Quiz Generator</h3>
                                <p class="text-xs text-purple-300">Buat soal latihan HOTS baru secara real-time berbasis topik pilihanmu!</p>
                            </div>
                        </div>

                        <div class="grid grid-cols-1 sm:grid-cols-3 gap-3 mb-4">
                            <select id="gen-mapel" class="bg-slate-950 border border-slate-700 text-slate-200 text-xs rounded-xl p-3 focus:outline-none focus:border-purple-500">
                                <option value="Matematika Kuantitatif">Matematika Kuantitatif</option>
                                <option value="Fisika Mekanika">Fisika Mekanika</option>
                                <option value="Kimia Larutan">Kimia Larutan</option>
                                <option value="Biologi Genetika">Biologi Genetika</option>
                                <option value="Literasi Bahasa">Literasi Bahasa</option>
                            </select>
                            <select id="gen-level" class="bg-slate-950 border border-slate-700 text-slate-200 text-xs rounded-xl p-3 focus:outline-none focus:border-purple-500">
                                <option value="Sedang (UTBK Standard)">Tingkat: Sedang (UTBK Standard)</option>
                                <option value="Sangat Tinggi (HOTS Master)">Tingkat: Sangat Tinggi (HOTS Master)</option>
                            </select>
                            <button onclick="generateGeminiQuestion()" class="gradient-gemini hover:opacity-90 text-white font-extrabold text-xs px-5 py-3 rounded-xl transition shadow-lg flex items-center justify-center gap-2">
                                <i data-lucide="cpu" class="w-4 h-4"></i> Generate Soal Gemini
                            </button>
                        </div>

                        <div id="gemini-question-output" class="hidden bg-slate-950 border border-purple-500/30 p-5 rounded-2xl text-xs text-slate-200 leading-relaxed fade-in">
                        </div>
                    </div>

                    <!-- Standard Simulation Cards -->
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                        <div class="gradient-card border border-slate-800 p-6 rounded-3xl flex flex-col justify-between shadow-xl hover:border-amber-500/50 transition duration-300">
                            <div>
                                <div class="w-12 h-12 rounded-2xl bg-amber-500/20 border border-amber-500/30 text-amber-400 flex items-center justify-center mb-4 font-black">
                                    <i data-lucide="calculator" class="w-6 h-6"></i>
                                </div>
                                <span class="text-[10px] uppercase font-extrabold text-amber-400 bg-amber-500/10 px-2.5 py-1 rounded-md">SNBT Standard</span>
                                <h3 class="text-xl font-extrabold text-white mt-3 mb-1">UTBK - Pengetahuan Kuantitatif</h3>
                                <p class="text-slate-400 text-xs mb-6 leading-relaxed">Uji pemahaman aljabar, eksponen, logaritma, & deret matematika HOTS.</p>
                            </div>
                            <button onclick="startSimulasi('utbk-pk')" class="w-full py-3.5 bg-amber-500 hover:bg-amber-400 text-slate-950 font-black text-xs rounded-xl transition flex items-center justify-center gap-2">
                                <i data-lucide="play" class="w-4 h-4 fill-current"></i> Mulai Tes (15 Menit)
                            </button>
                        </div>

                        <div class="gradient-card border border-slate-800 p-6 rounded-3xl flex flex-col justify-between shadow-xl hover:border-indigo-500/50 transition duration-300">
                            <div>
                                <div class="w-12 h-12 rounded-2xl bg-indigo-500/20 border border-indigo-500/30 text-indigo-400 flex items-center justify-center mb-4 font-black">
                                    <i data-lucide="zap" class="w-6 h-6"></i>
                                </div>
                                <span class="text-[10px] uppercase font-extrabold text-indigo-400 bg-indigo-500/10 px-2.5 py-1 rounded-md">TKA High Level</span>
                                <h3 class="text-xl font-extrabold text-white mt-3 mb-1">TKA Saintek - Fisika HOTS</h3>
                                <p class="text-slate-400 text-xs mb-6 leading-relaxed">Uji penalaran fisika mekanika, vektor, dan Hukum Newton.</p>
                            </div>
                            <button onclick="startSimulasi('tka-saintek')" class="w-full py-3.5 bg-indigo-600 hover:bg-indigo-500 text-white font-black text-xs rounded-xl transition flex items-center justify-center gap-2">
                                <i data-lucide="play" class="w-4 h-4 fill-current"></i> Mulai Tes (15 Menit)
                            </button>
                        </div>

                        <div class="gradient-card border border-slate-800 p-6 rounded-3xl flex flex-col justify-between shadow-xl hover:border-emerald-500/50 transition duration-300">
                            <div>
                                <div class="w-12 h-12 rounded-2xl bg-emerald-500/20 border border-emerald-500/30 text-emerald-400 flex items-center justify-center mb-4 font-black">
                                    <i data-lucide="book-marked" class="w-6 h-6"></i>
                                </div>
                                <span class="text-[10px] uppercase font-extrabold text-emerald-400 bg-emerald-500/10 px-2.5 py-1 rounded-md">General Literacy</span>
                                <h3 class="text-xl font-extrabold text-white mt-3 mb-1">Literasi Bahasa & Penalaran</h3>
                                <p class="text-slate-400 text-xs mb-6 leading-relaxed">Uji pemahaman ide pokok, simpulan bacaan, & analisis paragraf.</p>
                            </div>
                            <button onclick="startSimulasi('lit-ind-eng')" class="w-full py-3.5 bg-emerald-600 hover:bg-emerald-500 text-white font-black text-xs rounded-xl transition flex items-center justify-center gap-2">
                                <i data-lucide="play" class="w-4 h-4 fill-current"></i> Mulai Tes (10 Menit)
                            </button>
                        </div>
                    </div>
                </div>
            `;
        }

        async function generateGeminiQuestion() {
            const mapel = document.getElementById('gen-mapel').value;
            const level = document.getElementById('gen-level').value;
            const output = document.getElementById('gemini-question-output');

            output.classList.remove('hidden');
            output.innerHTML = `
                <div class="flex items-center gap-2 text-purple-400 font-bold">
                    <span class="w-2 h-2 rounded-full bg-purple-400 animate-ping"></span>
                    <span>Gemini AI sedang menyusun soal HOTS khusus untukmu...</span>
                </div>
            `;

            const prompt = `Buatkan 1 contoh soal HOTS pilihan ganda (A, B, C, D, E) untuk materi ${mapel} tingkat ${level} sesuai standar UTBK SNBT 2026. Sertakan Kunci Jawaban dan Pembahasan Lengkap di bagian bawahnya.`;
            const result = await callGeminiAPI(prompt);

            output.innerHTML = `
                <div class="flex items-center justify-between border-b border-slate-800 pb-3 mb-3">
                    <span class="text-[10px] uppercase font-extrabold text-pink-400">Hasil Generator Gemini AI (${mapel})</span>
                    <button onclick="generateGeminiQuestion()" class="text-purple-400 hover:underline text-[10px] font-bold">Buat Soal Lain</button>
                </div>
                <div class="leading-relaxed">
                    ${result.replace(/\n/g, '<br>').replace(/\*\*(.*?)\*\*/g, '<strong>$1</strong>')}
                </div>
            `;
            addXP(15, 'Membuat Soal Gemini HOTS');
            lucide.createIcons();
        }

        function startSimulasi(simKey) {
            state.activeSimKey = simKey;
            state.currentSimAnswers = {};
            const currentSim = db.simulasiBank[simKey];
            
            state.timeLeftSeconds = currentSim.durasiMinutes * 60;
            
            const app = document.getElementById('app-content');
            app.innerHTML = `
                <div class="max-w-3xl mx-auto gradient-card border border-slate-800 p-6 sm:p-8 rounded-3xl shadow-2xl fade-in">
                    <div class="sticky top-28 z-40 bg-slate-900/95 border border-purple-500/40 p-4 rounded-2xl mb-6 backdrop-blur-md shadow-lg flex items-center justify-between">
                        <div>
                            <span class="text-[10px] font-extrabold text-purple-400 uppercase block">Simulasi Interaktif</span>
                            <h2 class="text-sm sm:text-base font-black text-white">${currentSim.title}</h2>
                        </div>
                        <div class="bg-purple-950/80 border border-purple-500/50 px-4 py-2 rounded-xl text-center">
                            <span class="text-[9px] text-purple-300 font-extrabold uppercase block">Sisa Waktu</span>
                            <span id="quiz-timer-display" class="text-base sm:text-lg font-black text-amber-400 font-mono">--:--</span>
                        </div>
                    </div>

                    <div id="quiz-container" class="space-y-8">
                        ${currentSim.soal.map((q, idx) => `
                            <div class="bg-slate-900/90 p-6 rounded-2xl border border-slate-800">
                                <span class="text-xs font-bold text-purple-400 font-mono block mb-2">Soal #${idx + 1} dari${currentSim.soal.length}</span>
                                <p class="text-sm sm:text-base text-slate-100 font-medium mb-5 leading-relaxed">${q.pertanyaan}</p>
                                <div class="space-y-3">
                                    ${q.pilihan.map(opt => `
                                        <label id="label_${q.id}_${opt.charAt(0)}" class="flex items-center p-3.5 rounded-xl border border-slate-800 bg-slate-950/40 hover:bg-slate-800 cursor-pointer group">
                                            <input type="radio" name="question_${q.id}" value="${opt}" onchange="recordAnswer('${q.id}', '${opt}')" class="w-4 h-4 text-purple-600 focus:ring-purple-500 bg-slate-900 border-slate-700">
                                            <span class="ml-3.5 text-xs sm:text-sm text-slate-300 font-medium">${opt}</span>
                                        </label>
                                    `).join('')}
                                </div>
                            </div>
                        `).join('')}
                    </div>

                    <div class="mt-8 pt-6 border-t border-slate-800 flex justify-between items-center">
                        <button onclick="switchView('utbk')" class="px-5 py-2.5 border border-slate-800 text-slate-400 hover:text-white text-xs font-extrabold rounded-xl transition">Batal</button>
                        <button onclick="submitSimulasi('${simKey}')" class="px-6 py-3.5 gradient-gemini text-white font-black text-xs rounded-xl shadow-lg shadow-purple-500/25">Selesaikan</button>
                    </div>
                </div>
            `;
            
            lucide.createIcons();
            window.scrollTo({ top: 0, behavior: 'smooth' });

            updateTimerDisplay();
            if (state.timerInterval) clearInterval(state.timerInterval);
            state.timerInterval = setInterval(() => {
                state.timeLeftSeconds--;
                updateTimerDisplay();
                if (state.timeLeftSeconds <= 0) {
                    clearInterval(state.timerInterval);
                    showToast('Waktu simulasi habis!', 'error');
                    submitSimulasi(simKey);
                }
            }, 1000);
        }

        function updateTimerDisplay() {
            const timerEl = document.getElementById('quiz-timer-display');
            if (!timerEl) return;
            const m = Math.floor(state.timeLeftSeconds / 60);
            const s = state.timeLeftSeconds % 60;
            timerEl.innerText = `${m < 10 ? '0' : ''}${m}:${s < 10 ? '0' : ''}${s}`;
        }

        function recordAnswer(qId, val) {
            state.currentSimAnswers[qId] = val;
        }

        function submitSimulasi(simKey) {
            if (state.timerInterval) {
                clearInterval(state.timerInterval);
                state.timerInterval = null;
            }

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
            addXP(score >= 80 ? 50 : 25, 'Menyelesaikan Simulasi UTBK');

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

            showToast('Simulasi berhasil diselesaikan!');
            switchView('riwayat');
            openDetailRiwayat(state.attempts.length - 1);
        }

        // Render History Screen
        function renderRiwayatScreen() {
            if (state.attempts.length === 0) {
                return `
                    <div class="fade-in text-center py-12">
                        <h1 class="text-2xl font-black text-white">Belum Ada Riwayat Tersimpan</h1>
                        <p class="text-xs text-slate-400 mt-2 mb-6">Selesaikan simulasi TKA/UTBK untuk mencatat riwayat jawaban Anda.</p>
                        <button onclick="switchView('utbk')" class="px-6 py-3 bg-purple-600 text-white text-xs font-bold rounded-xl">Mulai Simulasi</button>
                    </div>
                `;
            }

            return `
                <div class="fade-in">
                    <h1 class="text-3xl font-black text-white tracking-tight mb-8">Riwayat Pengerjaan</h1>
                    <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
                        <div class="lg:col-span-4 space-y-3">
                            ${state.attempts.map((att, idx) => `
                                <button onclick="openDetailRiwayat(${idx})" class="w-full text-left p-4 rounded-2xl bg-slate-900 border border-slate-800 hover:bg-slate-800 transition flex items-center justify-between">
                                    <div>
                                        <span class="text-[10px] text-slate-500 font-mono block">${att.tanggal}</span>
                                        <h4 class="font-extrabold text-sm text-white mt-0.5">${att.judulSimulasi}</h4>
                                    </div>
                                    <span class="text-sm font-black text-purple-300 font-mono">${att.skor}%</span>
                                </button>
                            `).join('')}
                        </div>
                        <div id="riwayat-detail-container" class="lg:col-span-8 gradient-card border border-slate-800 rounded-3xl p-6 sm:p-8 shadow-2xl">
                        </div>
                    </div>
                </div>
            `;
        }

        function openDetailRiwayat(index) {
            const att = state.attempts[index];
            const container = document.getElementById('riwayat-detail-container');
            if (!container || !att) return;

            container.innerHTML = `
                <div class="flex items-center justify-between pb-6 border-b border-slate-800 mb-6">
                    <div>
                        <span class="text-xs text-purple-400 font-mono block">${att.tanggal}</span>
                        <h2 class="text-xl font-black text-white mt-0.5">${att.judulSimulasi}</h2>
                    </div>
                    <span class="text-3xl font-black text-purple-300 font-mono">${att.skor}%</span>
                </div>

                <div class="space-y-6">
                    ${att.detail.map((d, i) => `
                        <div class="bg-slate-900 border ${d.isCorrect ? 'border-emerald-500/40' : 'border-rose-500/40'} p-5 rounded-2xl">
                            <span class="text-xs font-bold text-slate-400 font-mono block mb-2">Soal #${i + 1}</span>
                            <p class="text-xs sm:text-sm text-slate-200 font-medium mb-4">${d.pertanyaan}</p>
                            <div class="bg-purple-950/30 p-4 rounded-xl text-xs text-slate-300">
                                <strong>Pembahasan Akurat:</strong><br>${d.solusi}
                            </div>
                        </div>
                    `).join('')}
                </div>
            `;
            lucide.createIcons();
        }

        // Initialize App Engine
        document.addEventListener('DOMContentLoaded', () => {
            switchView('home');
        });
    </script>
</body>
</html>
