[index.html](https://github.com/user-attachments/files/34114412/index.html)
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>基隆雙層觀巴~上山下海一日遊 🚌🎨</title>
    
    <!-- Google Fonts: Huninn (粉圓) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Mochiy+Pop+One&family=Zen+Maru+Gothic:wght@400;700;900&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        paper: '#FFFCF6',
                        ink: '#3E3A39',
                        coral: '#F2A497',
                        yamabuki: '#F6D27A',
                        aqua: '#A8D3E6',
                        wakatake: '#B9DAA5',
                        cream: '#FFF9E6'
                    },
                    fontFamily: {
                        huninn: ['"Zen Maru Gothic"', 'sans-serif'],
                    },
                    boxShadow: {
                        'picture': '4px 4px 0px #3E3A39',
                        'picture-sm': '2px 2px 0px #3E3A39',
                        'picture-lg': '6px 6px 0px #3E3A39',
                    }
                }
            }
        }
    </script>

    <style>
        body {
            background-color: #FFFCF6;
            color: #3E3A39;
            font-family: 'Zen Maru Gothic', sans-serif;
            background-image: radial-gradient(#3E3A39 0.75px, transparent 0.75px);
            background-size: 16px 16px;
            background-color: #FFFCF6;
        }

        /* 3px Ink Borders */
        .border-ink {
            border: 3px solid #3E3A39;
        }

        .border-ink-2 {
            border: 2px solid #3E3A39;
        }

        /* Animations */
        @keyframes floatSlow {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-8px) rotate(2deg); }
        }

        @keyframes bounceSpring {
            0% { transform: scale(0.9); opacity: 0; }
            70% { transform: scale(1.05); }
            100% { transform: scale(1); opacity: 1; }
        }

        .animate-float {
            animation: floatSlow 4s ease-in-out infinite;
        }

        .bounce-in {
            animation: bounceSpring 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275) forwards;
        }

        /* Reduced Motion Support */
        @media (prefers-reduced-motion: reduce) {
            .animate-float, .bounce-in {
                animation: none !important;
                transition: none !important;
            }
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
            height: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #FFFCF6;
        }
        ::-webkit-scrollbar-thumb {
            background: #F6D27A;
            border-radius: 10px;
            border: 2px solid #3E3A39;
        }
    </style>
</head>
<body class="pb-24 pt-16">

    <!-- Top Fixed Navigation Bar -->
    <nav class="fixed top-0 left-0 right-0 z-50 bg-[#FFFCF6] border-b-4 border-ink px-4 py-2 shadow-sm">
        <div class="max-w-md mx-auto flex justify-between items-center">
            <a href="#home" class="flex items-center gap-2 font-bold text-lg text-ink">
                <!-- Bus SVG Icon -->
                <svg class="w-7 h-7" viewBox="0 0 64 64" fill="none">
                    <rect x="8" y="16" width="48" height="32" rx="8" fill="#F2A497" stroke="#3E3A39" stroke-width="3"/>
                    <rect x="14" y="22" width="14" height="12" rx="3" fill="#A8D3E6" stroke="#3E3A39" stroke-width="3"/>
                    <rect x="36" y="22" width="14" height="12" rx="3" fill="#A8D3E6" stroke="#3E3A39" stroke-width="3"/>
                    <circle cx="20" cy="48" r="6" fill="#F6D27A" stroke="#3E3A39" stroke-width="3"/>
                    <circle cx="44" cy="48" r="6" fill="#F6D27A" stroke="#3E3A39" stroke-width="3"/>
                </svg>
                <span>基隆觀巴一日遊</span>
            </a>
            <div class="flex gap-2 text-sm font-bold">
                <a href="#bus" class="px-2 py-1 bg-yamabuki rounded-xl border-ink-2 shadow-picture-sm hover:translate-y-0.5">交通</a>
                <a href="#itinerary" class="px-2 py-1 bg-aqua rounded-xl border-ink-2 shadow-picture-sm hover:translate-y-0.5">行程</a>
                <a href="#todo" class="px-2 py-1 bg-wakatake rounded-xl border-ink-2 shadow-picture-sm hover:translate-y-0.5">清單</a>
            </div>
        </div>
    </nav>

    <main class="max-w-md mx-auto px-4 space-y-6 mt-4">

        <!-- Hero Section -->
        <section id="home" class="bg-cream rounded-3xl p-5 border-ink shadow-picture text-center relative overflow-hidden">
            <!-- Decorative SVG Clouds & Birds -->
            <div class="absolute top-2 left-3 animate-float opacity-80">
                <svg width="40" height="24" viewBox="0 0 40 24" fill="none">
                    <path d="M8 18 C 0 18, 0 10, 8 10 C 8 4, 20 4, 24 8 C 28 2, 38 4, 38 12 C 42 12, 42 18, 36 18 Z" fill="#ffffff" stroke="#3E3A39" stroke-width="2"/>
                </svg>
            </div>
            <div class="absolute top-4 right-4 animate-float" style="animation-delay: 1.5s;">
                <svg width="28" height="20" viewBox="0 0 28 20" fill="none">
                    <path d="M2 10 Q 7 2, 14 10 Q 21 2, 26 10" stroke="#3E3A39" stroke-width="2.5" stroke-linecap="round" fill="none"/>
                </svg>
            </div>

            <!-- Hand Drawn Main Hero Illustration: Keelung Open Top Bus & Mountain/Sea -->
            <div class="w-full h-44 my-2 flex items-center justify-center">
                <svg viewBox="0 0 300 160" class="w-full h-full">
                    <!-- Sea / Waves -->
                    <path d="M 10 130 Q 30 120, 60 130 T 110 130 T 160 130 T 210 130 T 260 130 T 290 130 L 290 150 L 10 150 Z" fill="#A8D3E6" stroke="#3E3A39" stroke-width="3"/>
                    <!-- Mountain -->
                    <path d="M 180 130 Q 220 50, 270 130 Z" fill="#B9DAA5" stroke="#3E3A39" stroke-width="3"/>
                    <path d="M 230 130 Q 255 80, 290 130 Z" fill="#9BC48A" stroke="#3E3A39" stroke-width="3"/>
                    
                    <!-- Keelung Tower Silhouette in background -->
                    <rect x="235" y="45" width="8" height="45" fill="#F2A497" stroke="#3E3A39" stroke-width="2" />
                    <polygon points="230,45 249,45 239,30" fill="#F2A497" stroke="#3E3A39" stroke-width="2" />
                    
                    <!-- Open-Top Bus -->
                    <g transform="translate(35, 65)">
                        <!-- Bus Body Bottom -->
                        <rect x="10" y="30" width="130" height="35" rx="8" fill="#F2A497" stroke="#3E3A39" stroke-width="3"/>
                        <!-- Bus Open Top Rail -->
                        <path d="M 15 30 L 15 15 L 135 15 L 135 30" fill="none" stroke="#3E3A39" stroke-width="3"/>
                        <line x1="45" y1="15" x2="45" y2="30" stroke="#3E3A39" stroke-width="2"/>
                        <line x1="75" y1="15" x2="75" y2="30" stroke="#3E3A39" stroke-width="2"/>
                        <line x1="105" y1="15" x2="105" y2="30" stroke="#3E3A39" stroke-width="2"/>
                        
                        <!-- Passengers Emojis/Faces -->
                        <circle cx="30" cy="22" r="6" fill="#F6D27A" stroke="#3E3A39" stroke-width="2"/>
                        <circle cx="60" cy="22" r="6" fill="#FFF" stroke="#3E3A39" stroke-width="2"/>
                        <circle cx="90" cy="22" r="6" fill="#A8D3E6" stroke="#3E3A39" stroke-width="2"/>
                        
                        <!-- Windows -->
                        <rect x="20" y="38" width="25" height="15" rx="3" fill="#FFF" stroke="#3E3A39" stroke-width="2"/>
                        <rect x="52" y="38" width="25" height="15" rx="3" fill="#FFF" stroke="#3E3A39" stroke-width="2"/>
                        <rect x="84" y="38" width="25" height="15" rx="3" fill="#FFF" stroke="#3E3A39" stroke-width="2"/>
                        
                        <!-- Wheels -->
                        <circle cx="35" cy="65" r="10" fill="#3E3A39"/>
                        <circle cx="35" cy="65" r="4" fill="#FFF"/>
                        <circle cx="110" cy="65" r="10" fill="#3E3A39"/>
                        <circle cx="110" cy="65" r="4" fill="#FFF"/>
                        
                        <!-- Headlight -->
                        <circle cx="138" cy="48" r="3" fill="#F6D27A"/>
                    </g>
                </svg>
            </div>

            <span class="inline-block px-3 py-1 bg-yamabuki rounded-full border-ink text-xs font-bold mb-1">
                2026.11.14（六）雙層觀巴特別篇
            </span>
            <h1 class="text-2xl font-black text-ink mb-2">基隆觀巴~上山下海遊 ↠</h1>
            <p class="text-xs font-bold text-gray-700 mb-4">有隨車導覽員 ＋ 茶飲 & 點心 🦩</p>

            <!-- Countdown Box -->
            <div class="bg-paper border-ink rounded-2xl p-3 shadow-picture-sm flex justify-around items-center">
                <div class="text-center">
                    <span id="cd-days" class="text-2xl font-black text-coral">00</span>
                    <span class="text-xs block font-bold">天</span>
                </div>
                <span class="text-lg font-black">:</span>
                <div class="text-center">
                    <span id="cd-hours" class="text-2xl font-black text-yamabuki">00</span>
                    <span class="text-xs block font-bold">時</span>
                </div>
                <span class="text-lg font-black">:</span>
                <div class="text-center">
                    <span id="cd-mins" class="text-2xl font-black text-aqua">00</span>
                    <span class="text-xs block font-bold">分</span>
                </div>
                <span class="text-lg font-black">:</span>
                <div class="text-center">
                    <span id="cd-secs" class="text-2xl font-black text-wakatake">00</span>
                    <span class="text-xs block font-bold">秒</span>
                </div>
            </div>
        </section>

        <!-- Transportation & Flight/Bus Info Card -->
        <section id="bus" class="bg-paper border-ink rounded-3xl p-5 shadow-picture space-y-4">
            <div class="flex items-center gap-2 border-b-2 border-ink pb-2">
                <span class="w-8 h-8 rounded-full bg-coral flex items-center justify-center border-ink text-white font-bold">
                    <i class="fa-solid fa-bus"></i>
                </span>
                <h2 class="text-lg font-black">觀光巴士與集合資訊</h2>
            </div>

            <!-- Departure Info -->
            <div class="bg-cream border-ink rounded-2xl p-3 text-sm space-y-2">
                <div class="flex justify-between items-center">
                    <span class="font-bold text-coral">📍 集合地點</span>
                    <span class="font-black text-xs bg-yamabuki px-2 py-0.5 rounded-full border-ink">09:45 準時發車</span>
                </div>
                <p class="font-bold text-ink">江子翠捷運 2 號出口（怡客前）</p>
                <div class="text-xs text-red-600 bg-white p-2 rounded-xl border-ink-2 font-bold flex items-center gap-1">
                    <span>🙏 觀巴不等人，請務必準時抵達！</span>
                </div>
            </div>

            <!-- Parking & Toilet Alert -->
            <div class="grid grid-cols-2 gap-2 text-xs">
                <a href="https://maps.app.goo.gl/DLXfjKCejVa5roMK6?g_st=il" target="_blank" class="bg-aqua border-ink rounded-2xl p-2.5 flex items-center gap-2 hover:opacity-90 font-bold">
                    <i class="fa-solid fa-square-p text-lg"></i>
                    <div>
                        <p class="font-black">中山路A區🅿️</p>
                        <p class="text-[10px] text-gray-700">基隆港灣停車場</p>
                    </div>
                </a>
                <div class="bg-coral/30 border-ink rounded-2xl p-2.5 flex items-center gap-2 font-bold">
                    <i class="fa-solid fa-restroom text-lg text-coral"></i>
                    <div>
                        <p class="font-black text-red-700">🆘 上車前洗手間</p>
                        <p class="text-[10px] text-gray-700">巴士上無衛生設備</p>
                    </div>
                </div>
            </div>

            <!-- Route Map Table -->
            <div class="bg-white border-ink rounded-2xl p-3 text-xs space-y-2">
                <p class="font-black text-gray-700 flex justify-between items-center">
                    <span>🚌 雙層觀巴停靠站別</span>
                    <a href="https://www.keelungcitytour.com.tw/guide" target="_blank" class="text-blue-600 underline text-[11px]">官網指南</a>
                </p>
                <div class="flex flex-wrap gap-1.5 font-bold">
                    <span class="px-2 py-1 bg-yamabuki rounded-lg border-ink-2">K1 城際轉運站(11月台)</span>
                    <span class="px-2 py-1 bg-wakatake rounded-lg border-ink-2">K7 八斗子車站</span>
                    <span class="px-2 py-1 bg-coral rounded-lg border-ink-2">K5 正濱漁港</span>
                    <span class="px-2 py-1 bg-aqua rounded-lg border-ink-2">K4 沙灣歷史園區</span>
                    <span class="px-2 py-1 bg-cream rounded-lg border-ink-2">K3 東岸遊客中心</span>
                </div>
            </div>
        </section>

        <!-- Daily Itinerary Timeline Section -->
        <section id="itinerary" class="space-y-4">
            
            <!-- Date Switcher Tabs -->
            <div class="flex justify-between items-center bg-paper border-ink rounded-2xl p-1.5 shadow-picture-sm">
                <button onclick="switchTab('day1')" id="tab-day1" class="w-full py-2 font-black rounded-xl border-ink bg-yamabuki text-sm transition-all">
                    11/14（六）基隆全日遊
                </button>
            </div>

            <!-- Control Bar (Add Stop & Reset) -->
            <div class="flex justify-between items-center px-1">
                <span class="text-xs font-bold text-gray-600">💡 點擊「編輯」可修改時間或地圖連結</span>
                <button onclick="openAddModal()" class="px-3 py-1 bg-wakatake border-ink rounded-xl text-xs font-black shadow-picture-sm hover:scale-105 active:scale-95 transition-transform flex items-center gap-1">
                    <i class="fa-solid fa-plus"></i> 新增行程
                </button>
            </div>

            <!-- Timeline Items Container -->
            <div id="timeline-container" class="space-y-4 relative before:absolute before:inset-0 before:left-5 before:w-1 before:bg-ink">
                <!-- Timeline items will be rendered by JavaScript -->
            </div>
        </section>

        <!-- Checklist & Accommodation Info -->
        <section id="todo" class="bg-paper border-ink rounded-3xl p-5 shadow-picture space-y-4">
            <div class="flex items-center gap-2 border-b-2 border-ink pb-2">
                <span class="w-8 h-8 rounded-full bg-wakatake flex items-center justify-center border-ink text-ink font-bold">
                    <i class="fa-solid fa-list-check"></i>
                </span>
                <h2 class="text-lg font-black">行前備忘錄 & 隨身清單</h2>
            </div>

            <!-- Checkbox List -->
            <div id="todo-list" class="space-y-2 text-xs font-bold">
                <!-- Javascript will populate interactive checkboxes -->
            </div>

            <!-- Quick Note / Accommodation -->
            <div class="bg-cream border-ink rounded-2xl p-3 text-xs space-y-1">
                <p class="font-black text-coral"><i class="fa-solid fa-triangle-exclamation"></i> 特別提醒與訂位資訊</p>
                <p>• 12:30 午餐《望海巷石頭火鍋》已訂位海景位（低消 $400/人）</p>
                <p>• 19:30 晚餐《豬剛鬣脆皮豬》已訂位</p>
                <p>• 建議攜帶：悠遊卡（搭公車）、雨具、防風外套、相機</p>
            </div>
        </section>

    </main>

    <!-- Modal for Editing/Adding Itinerary Stop -->
    <div id="edit-modal" class="fixed inset-0 bg-black/40 z-50 hidden flex items-center justify-center p-4">
        <div class="bg-paper border-ink rounded-3xl p-5 w-full max-w-sm shadow-picture bounce-in space-y-3">
            <h3 id="modal-title" class="text-lg font-black border-b-2 border-ink pb-2">編輯行程內容</h3>
            
            <input type="hidden" id="edit-id">
            
            <div>
                <label class="text-xs font-bold block mb-1">時間 (如: 11:00)</label>
                <input type="text" id="edit-time" class="w-full border-ink rounded-xl p-2 text-xs bg-white focus:outline-none">
            </div>

            <div>
                <label class="text-xs font-bold block mb-1">行程名稱</label>
                <input type="text" id="edit-title" class="w-full border-ink rounded-xl p-2 text-xs bg-white focus:outline-none">
            </div>

            <div>
                <label class="text-xs font-bold block mb-1">交通標籤 / 公車站點</label>
                <input type="text" id="edit-transport" class="w-full border-ink rounded-xl p-2 text-xs bg-white focus:outline-none" placeholder="例如: 觀巴 K5 下車 / 步行3分鐘">
            </div>

            <div>
                <label class="text-xs font-bold block mb-1">詳細說明 & 亮點</label>
                <textarea id="edit-desc" rows="3" class="w-full border-ink rounded-xl p-2 text-xs bg-white focus:outline-none"></textarea>
            </div>

            <div>
                <label class="text-xs font-bold block mb-1">Google 地圖連結</label>
                <input type="text" id="edit-map" class="w-full border-ink rounded-xl p-2 text-xs bg-white focus:outline-none" placeholder="https://maps.app.goo.gl/...">
            </div>

            <div class="flex items-center gap-2">
                <input type="checkbox" id="edit-mustgo" class="w-4 h-4 accent-coral">
                <label for="edit-mustgo" class="text-xs font-bold text-coral">標記為「必去 🌟」</label>
            </div>

            <div class="flex gap-2 pt-2">
                <button onclick="saveItem()" class="flex-1 py-2 bg-wakatake border-ink rounded-xl text-xs font-black shadow-picture-sm">儲存</button>
                <button onclick="deleteItem()" id="btn-delete" class="py-2 px-3 bg-coral border-ink rounded-xl text-xs font-black text-white shadow-picture-sm">刪除</button>
                <button onclick="closeModal()" class="py-2 px-3 bg-gray-200 border-ink rounded-xl text-xs font-black">取消</button>
            </div>
        </div>
    </div>

    <!-- Toast Notification -->
    <div id="toast" class="fixed bottom-6 left-1/2 -translate-x-1/2 bg-ink text-white text-xs font-bold px-4 py-2 rounded-full shadow-lg opacity-0 pointer-events-none transition-opacity z-50">
        提示訊息
    </div>

    <script>
        // Initial Itinerary Data from the provided schedule
        const defaultItinerary = [
            {
                id: '1',
                time: '09:45',
                title: '江子翠捷運 2 號出口（怡客前）',
                transport: '遊覽車 / 專車出發 🚘',
                desc: '準時出發🙏 觀巴不等人🦩（車程約45分鐘）',
                map: 'https://maps.app.goo.gl/DLXfjKCejVa5roMK6?g_st=il',
                mustGo: true
            },
            {
                id: '2',
                time: '10:35',
                title: '基隆港灣中山路A區停車場 🅿️',
                transport: '步行 3 分鐘 🚶‍♂️',
                desc: '停好車後步行前往基隆城際轉運站。🆘 上車前先去洗手間！',
                map: 'https://maps.app.goo.gl/DLXfjKCejVa5roMK6?g_st=il',
                mustGo: false
            },
            {
                id: '3',
                time: '10:50',
                title: '基隆城際轉運站（11月台）K1 上車報到 ☝️',
                transport: '基隆雙層觀光巴士 🚌',
                desc: '11:00 出發 - 車上巡遊一小時。隨車導覽員 + 附茶飲 & 點心 🦩',
                map: 'https://www.keelungcitytour.com.tw/guide',
                mustGo: true
            },
            {
                id: '4',
                time: '11:45',
                title: '八斗子車站 K7 下車 📷',
                transport: '觀巴 K7 停靠站',
                desc: '停留約 15 分鐘，人車團體合影留念！12:00 上車搭一站前往正濱漁港。',
                map: '',
                mustGo: false
            },
            {
                id: '5',
                time: '12:15',
                title: '正濱漁港色彩屋 K5 下車 🎨',
                transport: '觀巴 K5 站 🐾 停留3小時',
                desc: '精彩重點行程區！準備用餐與周邊漫步散策。',
                map: 'https://charles.com.tw/基隆中正-彩虹灣-望海巷石頭火鍋、咖啡/',
                mustGo: true
            },
            {
                id: '6',
                time: '12:30',
                title: '午餐：彩虹灣餐飲 - 望海巷石頭火鍋 🍲',
                transport: '已訂海景位 🌊',
                desc: '白飯/醬料/古早味芋冰免費！人頭費 $30，以盤計價共鍋，低消 $400/人。飯後可至 4 樓欣賞 270 度無敵海景 📷',
                map: 'https://charles.com.tw/基隆中正-彩虹灣-望海巷石頭火鍋、咖啡/',
                mustGo: true
            },
            {
                id: '7',
                time: '14:00',
                title: '正濱漁港周邊漫步 🕊️',
                transport: '徒步巡禮 🚶‍♀️',
                desc: '台畜熱狗堡公車站📷、元山・城市美術館［正濱館］、基隆青年夢工場🚾',
                map: '',
                mustGo: false
            },
            {
                id: '8',
                time: '15:15',
                title: '正濱漁港 K5 上車 ☝️',
                transport: '觀巴巡遊一小時 🚌',
                desc: '享受車上記者視野巡遊基隆海岸。',
                map: '',
                mustGo: false
            },
            {
                id: '9',
                time: '16:15',
                title: '沙灣歷史文化園區 K4 下車 👇',
                transport: '觀巴 K4 站 🐾',
                desc: '步行周邊約半小時：大沙灣考古遺址、元山·美學［中正館］。17:20 K4 上車搭 1 站。',
                map: '',
                mustGo: false
            },
            {
                id: '10',
                time: '17:25',
                title: '東岸遊客中心 K3 下車 🚌',
                transport: '觀巴 Say Goodbye 👋',
                desc: '海洋廣場看黃阿瑪 🚾 -> 步行 6 分鐘前往基隆塔（免費）。',
                map: 'https://woment.com.tw/28944/keelung-tower/amp/',
                mustGo: true
            },
            {
                id: '11',
                time: '18:00',
                title: '基隆塔 & 傘人家族 🗼',
                transport: '高空景觀電梯 🛗',
                desc: '乘電梯直通觀景台俯瞰基隆港無敵夜景！4樓遠見人文空間，頂樓「崆書屋」五感體驗。',
                map: 'https://woment.com.tw/28944/keelung-tower/amp/',
                mustGo: true
            },
            {
                id: '12',
                time: '19:00',
                title: '返回基隆市政府搭公車 🚌',
                transport: '悠遊卡搭乘公車 1 站',
                desc: '搭電梯返至傘人家族，步行 3 分鐘至柯達飯店前等公車，至城際轉運站下車，步行5分鐘至餐廳。',
                map: '',
                mustGo: false
            },
            {
                id: '13',
                time: '19:30',
                title: '晚餐：豬剛鬣脆皮豬 🍖',
                transport: '已訂位 🍽️',
                desc: '美味招牌：脆皮豬炙燒牛 ｜ 沙拉 ｜ 軟法。',
                map: 'https://linnote.com/zhu-ganglie-crispy-roast-pork/',
                mustGo: true
            },
            {
                id: '14',
                time: '20:45',
                title: '取車賦歸 🅿️ ➔ 21:45 返抵江子翠',
                transport: '返程車程 🚘',
                desc: '步行至停車場，滿載美好回憶返回台北江子翠站！記得給車手250/人(含停車費)',
                map: '',
                mustGo: false
            }
        ];

        // Default Checklist Data
        const defaultTodos = [
            { text: '悠遊卡（加值至少 $200）', checked: true },
            { text: '雙層觀巴預約憑證 / 身分證件', checked: true },
            { text: '水壺與隨身雨具 / 摺疊傘', checked: false },
            { text: '相機 & 隨身行動電源', checked: true },
            { text: '薄外套（觀巴上層海風較大）', checked: false }
        ];

        // Load or initialize localStorage
        let itinerary = JSON.parse(localStorage.getItem('keelung_itinerary')) || defaultItinerary;
        let todos = JSON.parse(localStorage.getItem('keelung_todos')) || defaultTodos;

        // Render Timeline
        function renderItinerary() {
            const container = document.getElementById('timeline-container');
            container.innerHTML = '';

            itinerary.forEach((item, index) => {
                const card = document.createElement('div');
                card.className = "relative pl-10 bounce-in";
                card.style.animationDelay = `${index * 0.05}s`;

                card.innerHTML = `
                    <!-- Timeline Node Pin -->
                    <div class="absolute left-3.5 top-3 -translate-x-1/2 w-4 h-4 rounded-full border-ink bg-yamabuki z-10"></div>

                    <div class="bg-paper border-ink rounded-2xl p-4 shadow-picture space-y-2">
                        <div class="flex justify-between items-start gap-2">
                            <div class="flex items-center gap-2">
                                <span class="font-black text-sm px-2 py-0.5 bg-coral/30 rounded-lg border-ink-2">${item.time}</span>
                                ${item.mustGo ? '<span class="px-2 py-0.5 bg-coral text-white font-black text-[10px] rounded-full border-ink-2">必去 🌟</span>' : ''}
                            </div>
                            <button onclick="openEditModal('${item.id}')" class="text-xs font-bold text-gray-500 hover:text-ink px-2 py-0.5 border-ink-2 bg-cream rounded-lg">
                                編輯 ✏️
                            </button>
                        </div>

                        <h3 class="font-black text-base text-ink">${item.title}</h3>

                        ${item.transport ? `<div class="inline-block text-xs font-bold px-2.5 py-1 bg-aqua rounded-xl border-ink-2">${item.transport}</div>` : ''}

                        <p class="text-xs font-bold text-gray-700 leading-relaxed">${item.desc}</p>

                        ${item.map ? `
                            <div class="pt-1">
                                <a href="${item.map}" target="_blank" class="inline-flex items-center gap-1 text-xs font-black text-blue-600 bg-blue-50 px-2.5 py-1 rounded-xl border-ink-2 hover:bg-blue-100">
                                    <i class="fa-solid fa-map-location-dot"></i> 開啟地圖 / 連結
                                </a>
                            </div>
                        ` : ''}
                    </div>
                `;
                container.appendChild(card);
            });
        }

        // Render Todo Checklist
        function renderTodos() {
            const container = document.getElementById('todo-list');
            container.innerHTML = '';

            todos.forEach((todo, idx) => {
                const item = document.createElement('div');
                item.className = "flex items-center gap-2 bg-white p-2.5 rounded-xl border-ink";
                item.innerHTML = `
                    <input type="checkbox" id="todo-${idx}" ${todo.checked ? 'checked' : ''} onchange="toggleTodo(${idx})" class="w-4 h-4 accent-wakatake cursor-pointer">
                    <label for="todo-${idx}" class="cursor-pointer ${todo.checked ? 'line-through text-gray-400' : 'text-ink'}">${todo.text}</label>
                `;
                container.appendChild(item);
            });
        }

        function toggleTodo(idx) {
            todos[idx].checked = !todos[idx].checked;
            localStorage.setItem('keelung_todos', JSON.stringify(todos));
            renderTodos();
        }

        // Modal Controls
        function openEditModal(id) {
            const item = itinerary.find(i => i.id === id);
            if (!item) return;

            document.getElementById('edit-id').value = item.id;
            document.getElementById('edit-time').value = item.time;
            document.getElementById('edit-title').value = item.title;
            document.getElementById('edit-transport').value = item.transport || '';
            document.getElementById('edit-desc').value = item.desc || '';
            document.getElementById('edit-map').value = item.map || '';
            document.getElementById('edit-mustgo').checked = item.mustGo || false;

            document.getElementById('modal-title').innerText = "編輯行程項目";
            document.getElementById('btn-delete').classList.remove('hidden');
            document.getElementById('edit-modal').classList.remove('hidden');
        }

        function openAddModal() {
            document.getElementById('edit-id').value = '';
            document.getElementById('edit-time').value = '12:00';
            document.getElementById('edit-title').value = '';
            document.getElementById('edit-transport').value = '';
            document.getElementById('edit-desc').value = '';
            document.getElementById('edit-map').value = '';
            document.getElementById('edit-mustgo').checked = false;

            document.getElementById('modal-title').innerText = "新增行程項目";
            document.getElementById('btn-delete').classList.add('hidden');
            document.getElementById('edit-modal').classList.remove('hidden');
        }

        function closeModal() {
            document.getElementById('edit-modal').classList.add('hidden');
        }

        function saveItem() {
            const id = document.getElementById('edit-id').value;
            const time = document.getElementById('edit-time').value;
            const title = document.getElementById('edit-title').value;
            const transport = document.getElementById('edit-transport').value;
            const desc = document.getElementById('edit-desc').value;
            const map = document.getElementById('edit-map').value;
            const mustGo = document.getElementById('edit-mustgo').checked;

            if (!title) {
                showToast("請輸入行程名稱！");
                return;
            }

            if (id) {
                // Update
                const idx = itinerary.findIndex(i => i.id === id);
                if (idx !== -1) {
                    itinerary[idx] = { id, time, title, transport, desc, map, mustGo };
                }
            } else {
                // Add new
                const newId = Date.now().toString();
                itinerary.push({ id: newId, time, title, transport, desc, map, mustGo });
                // Sort by time
                itinerary.sort((a, b) => a.time.localeCompare(b.time));
            }

            localStorage.setItem('keelung_itinerary', JSON.stringify(itinerary));
            renderItinerary();
            closeModal();
            showToast("行程儲存成功！");
        }

        function deleteItem() {
            const id = document.getElementById('edit-id').value;
            if (!id) return;

            itinerary = itinerary.filter(i => i.id !== id);
            localStorage.setItem('keelung_itinerary', JSON.stringify(itinerary));
            renderItinerary();
            closeModal();
            showToast("已刪除項目");
        }

        function showToast(msg) {
            const toast = document.getElementById('toast');
            toast.innerText = msg;
            toast.classList.remove('opacity-0');
            setTimeout(() => {
                toast.classList.add('opacity-0');
            }, 2000);
        }

        // Live Countdown Timer
        function updateCountdown() {
            const targetDate = new Date('2026-11-14T09:45:00').getTime();
            const now = new Date().getTime();
            const diff = targetDate - now;

            if (diff <= 0) {
                document.getElementById('cd-days').innerText = "00";
                document.getElementById('cd-hours').innerText = "00";
                document.getElementById('cd-mins').innerText = "00";
                document.getElementById('cd-secs').innerText = "00";
                return;
            }

            const days = Math.floor(diff / (1000 * 60 * 60 * 24));
            const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const mins = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            const secs = Math.floor((diff % (1000 * 60)) / 1000);

            document.getElementById('cd-days').innerText = String(days).padStart(2, '0');
            document.getElementById('cd-hours').innerText = String(hours).padStart(2, '0');
            document.getElementById('cd-mins').innerText = String(mins).padStart(2, '0');
            document.getElementById('cd-secs').innerText = String(secs).padStart(2, '0');
        }

        // Tab Switch Animation Demo
        function switchTab(tab) {
            const btn = document.getElementById('tab-day1');
            btn.classList.add('bounce-in');
            setTimeout(() => btn.classList.remove('bounce-in'), 400);
        }

        // Initialize App
        window.onload = function() {
            renderItinerary();
            renderTodos();
            updateCountdown();
            setInterval(updateCountdown, 1000);
        };
    </script>
</body>
</html>
