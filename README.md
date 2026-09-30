[index (2).html](https://github.com/user-attachments/files/32846112/index.2.html)
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>이정민 | 연성대학교 포트폴리오 & 게임 허브</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome CDN -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;600;700;900&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Noto Sans KR', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#eef2ff',
                            100: '#e0e7ff',
                            500: '#6366f1',
                            600: '#4f46e5',
                            700: '#4338ca',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Noto Sans KR', sans-serif;
            transition: background-color 0.3s, color 0.3s;
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        .dark .glass-card {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        /* Custom scrollbars */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: transparent;
        }
        ::-webkit-scrollbar-thumb {
            background: #a5f3fc;
            border-radius: 4px;
        }
        .dark ::-webkit-scrollbar-thumb {
            background: #334155;
        }
        /* Card flip animation */
        .perspective-1000 {
            perspective: 1000px;
        }
        .transform-style-3d {
            transform-style: preserve-3d;
        }
        .backface-hidden {
            backface-visibility: hidden;
        }
        .rotate-y-180 {
            transform: rotateY(180deg);
        }
    </style>
</head>
<body class="bg-slate-50 dark:bg-slate-900 text-slate-800 dark:text-slate-100 min-h-screen flex flex-col">

    <header class="sticky top-0 z-50 glass-card border-b border-slate-200 dark:border-slate-800 transition-colors">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-indigo-500 to-purple-600 flex items-center justify-center text-white font-black text-xl shadow-md">
                    JM
                </div>
                <div>
                    <h1 class="text-lg font-bold leading-tight">이정민</h1>
                    <p class="text-xs text-indigo-600 dark:text-indigo-400 font-medium">연성대학교 (Yeonsung Univ)</p>
                </div>
            </div>

            <nav class="hidden md:flex items-center gap-6 text-sm font-semibold">
                <a href="#about" class="hover:text-indigo-600 dark:hover:text-indigo-400 transition">소개</a>
                <a href="#hobby" class="hover:text-indigo-600 dark:hover:text-indigo-400 transition">취미 (운동)</a>
                <a href="#games" class="hover:text-indigo-600 dark:hover:text-indigo-400 transition">미니게임 센터</a>
            </nav>

            <div class="flex items-center gap-3">
                <button id="themeToggleBtn" onclick="toggleDarkMode()" class="p-2.5 rounded-xl bg-slate-200 dark:bg-slate-800 text-slate-700 dark:text-slate-200 hover:bg-slate-300 dark:hover:bg-slate-700 transition" aria-label="다크모드 토글">
                    <i id="themeIcon" class="fa-solid fa-moon text-lg"></i>
                </button>
            </div>
        </div>
    </header>

    <main class="flex-grow max-w-6xl w-full mx-auto px-4 sm:px-6 lg:px-8 py-8 space-y-12">

        <section id="about" class="glass-card rounded-3xl p-6 sm:p-10 shadow-xl relative overflow-hidden">
            <div class="absolute -top-10 -right-10 w-48 h-48 bg-indigo-500/10 rounded-full blur-3xl pointer-events-none"></div>
            <div class="flex flex-col md:flex-row items-center gap-8">
                <div class="relative">
                    <div class="w-36 h-36 sm:w-44 sm:h-44 rounded-3xl bg-gradient-to-br from-indigo-500 via-purple-500 to-pink-500 p-1 shadow-2xl">
                        <div class="w-full h-full bg-slate-100 dark:bg-slate-800 rounded-[22px] flex flex-col items-center justify-center text-slate-700 dark:text-slate-200">
                            <i class="fa-solid fa-user-graduate text-6xl text-indigo-500 mb-2"></i>
                            <span class="text-xs font-semibold px-2 py-0.5 bg-indigo-100 dark:bg-indigo-900/50 text-indigo-600 dark:text-indigo-300 rounded-full">연성대학교</span>
                        </div>
                    </div>
                </div>
                <div class="flex-1 text-center md:text-left space-y-4">
                    <div class="inline-block px-3 py-1 bg-indigo-100 dark:bg-indigo-950 text-indigo-600 dark:text-indigo-300 text-xs font-bold rounded-full">
                        👋 안녕하세요!
                    </div>
                    <h2 class="text-3xl sm:text-4xl font-black tracking-tight">
                        안녕하세요, <span class="text-indigo-600 dark:text-indigo-400">이정민</span>입니다.
                    </h2>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed max-w-2xl text-sm sm:text-base">
                        <strong>연성대학교</strong> 학생으로 열정적으로 배움을 이어나가고 있습니다. 
                        건강한 신체에 건강한 정신이 숙든다는 마인드로 일상 속에서 **운동**을 즐기며, 
                        창의적이고 재미있는 웹 인터랙션에도 관심이 많습니다.
                    </p>
                    <div class="flex flex-wrap items-center justify-center md:justify-start gap-4 pt-2">
                        <div class="flex items-center gap-2 text-xs font-semibold px-3 py-1.5 bg-slate-100 dark:bg-slate-800 rounded-lg">
                            <i class="fa-solid fa-graduation-cap text-indigo-500"></i> 연성대학교 소속
                        </div>
                        <div class="flex items-center gap-2 text-xs font-semibold px-3 py-1.5 bg-slate-100 dark:bg-slate-800 rounded-lg">
                            <i class="fa-solid fa-dumbbell text-emerald-500"></i> 운동 매니아
                        </div>
                        <div class="flex items-center gap-2 text-xs font-semibold px-3 py-1.5 bg-slate-100 dark:bg-slate-800 rounded-lg">
                            <i class="fa-solid fa-gamepad text-purple-500"></i> 미니게임 메이커
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="hobby" class="space-y-6">
            <div class="flex items-center justify-between">
                <div>
                    <h2 class="text-2xl font-bold flex items-center gap-2">
                        <i class="fa-solid fa-heart-pulse text-rose-500"></i> 나의 취미: 운동 (Workout)
                    </h2>
                    <p class="text-sm text-slate-500 dark:text-slate-400">꾸준한 운동을 통해 체력과 집중력을 키우고 있습니다.</p>
                </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Card 1 -->
                <div class="glass-card rounded-2xl p-6 shadow-md hover:shadow-lg transition">
                    <div class="w-12 h-12 bg-rose-100 dark:bg-rose-900/30 text-rose-500 rounded-xl flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-dumbbell"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">웨이트 트레이닝</h3>
                    <p class="text-xs text-slate-600 dark:text-slate-400 mb-4">
                        근력 향상과 바른 자세를 위한 웨이트 운동. 점진적 과부하를 통한 꾸준한 성장을 목표로 합니다.
                    </p>
                    <div class="w-full bg-slate-200 dark:bg-slate-700 h-2 rounded-full overflow-hidden">
                        <div class="bg-rose-500 h-full w-[85%] rounded-full"></div>
                    </div>
                    <span class="text-[10px] text-slate-400 mt-1 block text-right">주 4회 이상 실천 중</span>
                </div>

                <!-- Card 2 -->
                <div class="glass-card rounded-2xl p-6 shadow-md hover:shadow-lg transition">
                    <div class="w-12 h-12 bg-sky-100 dark:bg-sky-900/30 text-sky-500 rounded-xl flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-person-running"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">러닝 & 유산소</h3>
                    <p class="text-xs text-slate-600 dark:text-slate-400 mb-4">
                        맑은 공기를 마시며 달리는 유산소 운동. 심폐 지구력과 머리를 비우는 리프레시 시간을 가집니다.
                    </p>
                    <div class="w-full bg-slate-200 dark:bg-slate-700 h-2 rounded-full overflow-hidden">
                        <div class="bg-sky-500 h-full w-[70%] rounded-full"></div>
                    </div>
                    <span class="text-[10px] text-slate-400 mt-1 block text-right">목표: 5km 러닝</span>
                </div>

                <!-- Card 3 -->
                <div class="glass-card rounded-2xl p-6 shadow-md hover:shadow-lg transition">
                    <div class="w-12 h-12 bg-emerald-100 dark:bg-emerald-900/30 text-emerald-500 rounded-xl flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-apple-whole"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">건강한 라이프스타일</h3>
                    <p class="text-xs text-slate-600 dark:text-slate-400 mb-4">
                        충분한 수면과 균형 잡힌 영양 섭취. 운동만큼 중요한 휴식과 수분 섭취를 규칙적으로 챙깁니다.
                    </p>
                    <div class="w-full bg-slate-200 dark:bg-slate-700 h-2 rounded-full overflow-hidden">
                        <div class="bg-emerald-500 h-full w-[90%] rounded-full"></div>
                    </div>
                    <span class="text-[10px] text-slate-400 mt-1 block text-right">Daily Check Complted</span>
                </div>
            </div>
        </section>

        <section id="games" class="space-y-6 pt-6 border-t border-slate-200 dark:border-slate-800">
            <div class="text-center space-y-2">
                <span class="px-3 py-1 bg-purple-100 dark:bg-purple-900/50 text-purple-600 dark:text-purple-300 text-xs font-bold rounded-full">
                    🎮 Arcade Zone
                </span>
                <h2 class="text-3xl font-black">이정민의 미니게임 아케이드 (6 Games)</h2>
                <p class="text-slate-500 dark:text-slate-400 text-sm max-w-lg mx-auto">
                    직접 제작한 6가지 미니게임을 즐겨보세요! 원하는 게임을 클릭하여 플레이할 수 있습니다.
                </p>
            </div>

            <!-- Game Selector Navigation Buttons -->
            <div class="flex flex-wrap items-center justify-center gap-2 p-2 glass-card rounded-2xl">
                <button onclick="switchGame(1)" id="tab-btn-1" class="game-tab-btn active px-4 py-2.5 rounded-xl text-xs sm:text-sm font-bold flex items-center gap-2 transition bg-indigo-600 text-white shadow-md">
                    <i class="fa-solid fa-hand-back-fist"></i> 1. 가위바위보
                </button>
                <button onclick="switchGame(2)" id="tab-btn-2" class="game-tab-btn px-4 py-2.5 rounded-xl text-xs sm:text-sm font-bold flex items-center gap-2 transition hover:bg-slate-200 dark:hover:bg-slate-700">
                    <i class="fa-solid fa-staff-snake"></i> 2. 스네이크
                </button>
                <button onclick="switchGame(3)" id="tab-btn-3" class="game-tab-btn px-4 py-2.5 rounded-xl text-xs sm:text-sm font-bold flex items-center gap-2 transition hover:bg-slate-200 dark:hover:bg-slate-700">
                    <i class="fa-solid fa-clone"></i> 3. 카드 맞추기
                </button>
                <button onclick="switchGame(4)" id="tab-btn-4" class="game-tab-btn px-4 py-2.5 rounded-xl text-xs sm:text-sm font-bold flex items-center gap-2 transition hover:bg-slate-200 dark:hover:bg-slate-700">
                    <i class="fa-solid fa-stopwatch"></i> 4. 반응속도
                </button>
                <button onclick="switchGame(5)" id="tab-btn-5" class="game-tab-btn px-4 py-2.5 rounded-xl text-xs sm:text-sm font-bold flex items-center gap-2 transition hover:bg-slate-200 dark:hover:bg-slate-700">
                    <i class="fa-solid fa-xmark-large"></i> 5. 틱택토
                </button>
                <button onclick="switchGame(6)" id="tab-btn-6" class="game-tab-btn px-4 py-2.5 rounded-xl text-xs sm:text-sm font-bold flex items-center gap-2 transition hover:bg-slate-200 dark:hover:bg-slate-700">
                    <i class="fa-solid fa-baseball"></i> 6. 숫자 야구
                </button>
            </div>

            <div class="glass-card rounded-3xl p-4 sm:p-8 shadow-2xl min-h-[460px] flex flex-col justify-center items-center relative overflow-hidden">

                <!-- GAME 1: 가위바위보 -->
                <div id="game-1" class="game-container w-full max-w-lg space-y-6 text-center">
                    <h3 class="text-xl font-bold text-indigo-600 dark:text-indigo-400">✌️ 가위바위보 게임</h3>
                    <div class="flex items-center justify-around bg-slate-100 dark:bg-slate-800/80 p-4 rounded-2xl">
                        <div>
                            <p class="text-xs text-slate-400 mb-1">나 (YOU)</p>
                            <div id="rpsPlayerDisplay" class="text-5xl">❔</div>
                        </div>
                        <div class="text-2xl font-black text-slate-400">VS</div>
                        <div>
                            <p class="text-xs text-slate-400 mb-1">AI 컴퓨터</p>
                            <div id="rpsAiDisplay" class="text-5xl">🤖</div>
                        </div>
                    </div>

                    <div id="rpsResultText" class="text-lg font-bold h-8 text-slate-600 dark:text-slate-300">
                        가위, 바위, 보 중 하나를 선택하세요!
                    </div>

                    <div class="grid grid-cols-3 gap-3">
                        <button onclick="playRPS('rock')" class="py-4 bg-slate-200 dark:bg-slate-700 hover:bg-indigo-500 hover:text-white rounded-2xl text-2xl transition shadow">
                            ✊<span class="block text-xs font-semibold mt-1">바위</span>
                        </button>
                        <button onclick="playRPS('paper')" class="py-4 bg-slate-200 dark:bg-slate-700 hover:bg-indigo-500 hover:text-white rounded-2xl text-2xl transition shadow">
                            ✋<span class="block text-xs font-semibold mt-1">보</span>
                        </button>
                        <button onclick="playRPS('scissors')" class="py-4 bg-slate-200 dark:bg-slate-700 hover:bg-indigo-500 hover:text-white rounded-2xl text-2xl transition shadow">
                            ✌️<span class="block text-xs font-semibold mt-1">가위</span>
                        </button>
                    </div>

                    <div class="flex justify-around text-xs font-bold pt-2 border-t border-slate-200 dark:border-slate-700">
                        <span class="text-emerald-500">승리: <span id="rpsWins">0</span></span>
                        <span class="text-amber-500">무승부: <span id="rpsDraws">0</span></span>
                        <span class="text-rose-500">패배: <span id="rpsLosses">0</span></span>
                    </div>
                </div>

                <!-- GAME 2: 스네이크 게임 -->
                <div id="game-2" class="game-container hidden w-full max-w-md space-y-4 text-center">
                    <div class="flex items-center justify-between">
                        <h3 class="text-xl font-bold text-indigo-600 dark:text-indigo-400">🐍 스네이크 게임</h3>
                        <div class="text-xs font-semibold space-x-3">
                            <span>점수: <span id="snakeScore" class="text-indigo-500 font-bold">0</span></span>
                            <span>최고: <span id="snakeHighScore" class="text-amber-500 font-bold">0</span></span>
                        </div>
                    </div>
                    
                    <div class="relative mx-auto flex justify-center">
                        <canvas id="snakeCanvas" width="300" height="300" class="bg-slate-900 rounded-2xl border-4 border-slate-700 shadow-inner"></canvas>
                        <div id="snakeOverlay" class="absolute inset-0 bg-slate-900/80 backdrop-blur-sm rounded-2xl flex flex-col items-center justify-center text-white p-4">
                            <p class="font-bold text-lg mb-2">스네이크 게임</p>
                            <p class="text-xs text-slate-300 mb-4 text-center">방향키나 아래 컨트롤러 버튼으로 먹이를 드세요!</p>
                            <button onclick="startSnakeGame()" class="px-5 py-2.5 bg-indigo-600 hover:bg-indigo-500 text-white font-bold rounded-xl text-sm transition shadow-lg">
                                게임 시작
                            </button>
                        </div>
                    </div>

                    <!-- Mobile Controller for Snake -->
                    <div class="grid grid-cols-3 gap-2 w-48 mx-auto pt-2">
                        <div></div>
                        <button onclick="setSnakeDir('UP')" class="p-3 bg-slate-200 dark:bg-slate-700 rounded-xl hover:bg-indigo-500 hover:text-white"><i class="fa-solid fa-arrow-up"></i></button>
                        <div></div>
                        <button onclick="setSnakeDir('LEFT')" class="p-3 bg-slate-200 dark:bg-slate-700 rounded-xl hover:bg-indigo-500 hover:text-white"><i class="fa-solid fa-arrow-left"></i></button>
                        <button onclick="setSnakeDir('DOWN')" class="p-3 bg-slate-200 dark:bg-slate-700 rounded-xl hover:bg-indigo-500 hover:text-white"><i class="fa-solid fa-arrow-down"></i></button>
                        <button onclick="setSnakeDir('RIGHT')" class="p-3 bg-slate-200 dark:bg-slate-700 rounded-xl hover:bg-indigo-500 hover:text-white"><i class="fa-solid fa-arrow-right"></i></button>
                    </div>
                </div>

                <!-- GAME 3: 메모리 카드 게임 -->
                <div id="game-3" class="game-container hidden w-full max-w-md space-y-4 text-center">
                    <div class="flex items-center justify-between">
                        <h3 class="text-xl font-bold text-indigo-600 dark:text-indigo-400">🎴 카드 뒤집기 메모리 게임</h3>
                        <button onclick="resetMemoryGame()" class="text-xs px-3 py-1 bg-indigo-100 dark:bg-indigo-900 text-indigo-600 dark:text-indigo-300 rounded-lg font-bold">
                            다시 시작
                        </button>
                    </div>
                    <p class="text-xs text-slate-500">같은 짝의 짝을 찾아 카드를 완성하세요!</p>
                    
                    <div id="memoryGrid" class="grid grid-cols-4 gap-3 perspective-1000">
                        <!-- Cards dynamically generated -->
                    </div>
                    <div class="text-xs font-semibold text-slate-500">
                        시도 횟수: <span id="memoryFlips" class="text-indigo-500 font-bold">0</span> 회
                    </div>
                </div>

                <!-- GAME 4: 반응속도 테스트 -->
                <div id="game-4" class="game-container hidden w-full max-w-md space-y-4 text-center">
                    <h3 class="text-xl font-bold text-indigo-600 dark:text-indigo-400">⚡ 반응속도 테스트</h3>
                    
                    <div id="reactionArea" onclick="handleReactionClick()" class="w-full h-64 rounded-3xl bg-rose-500 text-white flex flex-col items-center justify-center cursor-pointer select-none transition-all p-6 shadow-inner">
                        <i id="reactionIcon" class="fa-solid fa-hand-pointer text-4xl mb-3"></i>
                        <p id="reactionTitle" class="text-xl font-bold">클릭하여 시작하세요!</p>
                        <p id="reactionSub" class="text-xs opacity-80 mt-1">화면이 초록색으로 바뀌면 즉시 클릭하세요.</p>
                    </div>

                    <div class="text-sm font-semibold">
                        최근 기록: <span id="reactionTimeResult" class="text-indigo-500 font-bold">- ms</span>
                    </div>
                </div>

                <!-- GAME 5: 틱택토 -->
                <div id="game-5" class="game-container hidden w-full max-w-sm space-y-4 text-center">
                    <div class="flex items-center justify-between">
                        <h3 class="text-xl font-bold text-indigo-600 dark:text-indigo-400">❌⭕ 틱택토 (Tic-Tac-Toe)</h3>
                        <button onclick="resetTicTacToe()" class="text-xs px-3 py-1 bg-indigo-100 dark:bg-indigo-900 text-indigo-600 dark:text-indigo-300 rounded-lg font-bold">
                            리셋
                        </button>
                    </div>
                    <p id="tttStatus" class="text-sm font-bold text-slate-600 dark:text-slate-300">당신의 차례입니다 (X)</p>

                    <div class="grid grid-cols-3 gap-2 max-w-[280px] mx-auto">
                        <button onclick="makeTTTMove(0)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                        <button onclick="makeTTTMove(1)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                        <button onclick="makeTTTMove(2)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                        <button onclick="makeTTTMove(3)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                        <button onclick="makeTTTMove(4)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                        <button onclick="makeTTTMove(5)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                        <button onclick="makeTTTMove(6)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                        <button onclick="makeTTTMove(7)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                        <button onclick="makeTTTMove(8)" class="ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition"></button>
                    </div>
                </div>

                <!-- GAME 6: 숫자 야구 -->
                <div id="game-6" class="game-container hidden w-full max-w-md space-y-4 text-center">
                    <div class="flex items-center justify-between">
                        <h3 class="text-xl font-bold text-indigo-600 dark:text-indigo-400">⚾ 숫자 야구 게임</h3>
                        <button onclick="resetBaseballGame()" class="text-xs px-3 py-1 bg-indigo-100 dark:bg-indigo-900 text-indigo-600 dark:text-indigo-300 rounded-lg font-bold">
                            새 게임
                        </button>
                    </div>
                    <p class="text-xs text-slate-500">서로 다른 3자리 숫자를 맞춰보세요!</p>

                    <form onsubmit="handleBaseballSubmit(event)" class="flex gap-2">
                        <input type="text" id="baseballInput" maxlength="3" placeholder="예: 123" pattern="[1-9]{3}" required class="flex-1 px-4 py-2.5 rounded-xl border border-slate-300 dark:border-slate-700 bg-slate-50 dark:bg-slate-800 text-center text-lg font-bold focus:outline-none focus:ring-2 focus:ring-indigo-500">
                        <button type="submit" class="px-5 py-2.5 bg-indigo-600 hover:bg-indigo-500 text-white font-bold rounded-xl text-sm transition">
                            구속!
                        </button>
                    </form>

                    <div class="bg-slate-100 dark:bg-slate-800/80 rounded-2xl p-4 h-44 overflow-y-auto border border-slate-200 dark:border-slate-700 text-left text-xs font-mono space-y-1.5" id="baseballLog">
                        <div class="text-slate-400 text-center py-4">게임 기록이 여기에 표시됩니다.</div>
                    </div>
                </div>

            </div>
        </section>
    </main>

    <footer class="mt-auto border-t border-slate-200 dark:border-slate-800 py-6 text-center text-xs text-slate-500">
        <div class="max-w-6xl mx-auto px-4 flex flex-col sm:flex-row items-center justify-between gap-2">
            <p>© 2026 이정민 (Yeonsung University). All rights reserved.</p>
            <p class="flex items-center gap-1">
                Made with <i class="fa-solid fa-heart text-rose-500"></i> & Sports Spirit
            </p>
        </div>
    </footer>

    <script>
        // --- 0. Theme Toggle ---
        function toggleDarkMode() {
            const html = document.documentElement;
            const icon = document.getElementById('themeIcon');
            if (html.classList.contains('dark')) {
                html.classList.remove('dark');
                icon.className = 'fa-solid fa-moon text-lg';
            } else {
                html.classList.add('dark');
                icon.className = 'fa-solid fa-sun text-lg text-amber-400';
            }
        }

        // --- Tab Switcher ---
        function switchGame(gameNum) {
            document.querySelectorAll('.game-container').forEach(el => el.classList.add('hidden'));
            document.querySelectorAll('.game-tab-btn').forEach(btn => {
                btn.classList.remove('bg-indigo-600', 'text-white', 'shadow-md');
                btn.classList.add('hover:bg-slate-200', 'dark:hover:bg-slate-700');
            });

            document.getElementById(`game-${gameNum}`).classList.remove('hidden');
            const activeBtn = document.getElementById(`tab-btn-${gameNum}`);
            activeBtn.classList.add('bg-indigo-600', 'text-white', 'shadow-md');
            activeBtn.classList.remove('hover:bg-slate-200', 'dark:hover:bg-slate-700');

            if (gameNum === 3) initMemoryGame();
            if (gameNum === 5) resetTicTacToe();
            if (gameNum === 6) resetBaseballGame();
        }

        // --- GAME 1: Rock Paper Scissors ---
        let rpsStats = { wins: 0, draws: 0, losses: 0 };
        const rpsIcons = { rock: '✊', paper: '✋', scissors: '✌️' };

        function playRPS(playerChoice) {
            const choices = ['rock', 'paper', 'scissors'];
            const aiChoice = choices[Math.floor(Math.random() * 3)];

            document.getElementById('rpsPlayerDisplay').textContent = rpsIcons[playerChoice];
            document.getElementById('rpsAiDisplay').textContent = rpsIcons[aiChoice];

            const resultText = document.getElementById('rpsResultText');

            if (playerChoice === aiChoice) {
                rpsStats.draws++;
                resultText.textContent = "🤝 비겼습니다!";
                resultText.className = "text-lg font-bold h-8 text-amber-500";
            } else if (
                (playerChoice === 'rock' && aiChoice === 'scissors') ||
                (playerChoice === 'paper' && aiChoice === 'rock') ||
                (playerChoice === 'scissors' && aiChoice === 'paper')
            ) {
                rpsStats.wins++;
                resultText.textContent = "🎉 이겼습니다!";
                resultText.className = "text-lg font-bold h-8 text-emerald-500";
            } else {
                rpsStats.losses++;
                resultText.textContent = "😅 졌습니다. 다시 도전해보세요!";
                resultText.className = "text-lg font-bold h-8 text-rose-500";
            }

            document.getElementById('rpsWins').textContent = rpsStats.wins;
            document.getElementById('rpsDraws').textContent = rpsStats.draws;
            document.getElementById('rpsLosses').textContent = rpsStats.losses;
        }

        // --- GAME 2: Snake Game ---
        const snakeCanvas = document.getElementById('snakeCanvas');
        const ctx = snakeCanvas.getContext('2d');
        const grid = 15;
        let snake = [{x: 150, y: 150}];
        let dx = grid, dy = 0;
        let food = {x: 60, y: 60};
        let snakeScore = 0;
        let snakeHighScore = localStorage.getItem('snakeHighScore') || 0;
        let snakeInterval = null;
        document.getElementById('snakeHighScore').textContent = snakeHighScore;

        function startSnakeGame() {
            document.getElementById('snakeOverlay').classList.add('hidden');
            snake = [{x: 150, y: 150}];
            dx = grid; dy = 0;
            snakeScore = 0;
            document.getElementById('snakeScore').textContent = snakeScore;
            spawnFood();
            if (snakeInterval) clearInterval(snakeInterval);
            snakeInterval = setInterval(snakeLoop, 100);
        }

        function spawnFood() {
            food = {
                x: Math.floor(Math.random() * (snakeCanvas.width / grid)) * grid,
                y: Math.floor(Math.random() * (snakeCanvas.height / grid)) * grid
            };
        }

        function setSnakeDir(dir) {
            if (dir === 'UP' && dy === 0) { dx = 0; dy = -grid; }
            if (dir === 'DOWN' && dy === 0) { dx = 0; dy = grid; }
            if (dir === 'LEFT' && dx === 0) { dx = -grid; dy = 0; }
            if (dir === 'RIGHT' && dx === 0) { dx = grid; dy = 0; }
        }

        document.addEventListener('keydown', (e) => {
            if (e.key === 'ArrowUp') setSnakeDir('UP');
            if (e.key === 'ArrowDown') setSnakeDir('DOWN');
            if (e.key === 'ArrowLeft') setSnakeDir('LEFT');
            if (e.key === 'ArrowRight') setSnakeDir('RIGHT');
        });

        function snakeLoop() {
            const head = {x: snake[0].x + dx, y: snake[0].y + dy};

            // Wall Collision
            if (head.x < 0 || head.x >= snakeCanvas.width || head.y < 0 || head.y >= snakeCanvas.height) {
                return endSnakeGame();
            }

            // Self Collision
            for (let segment of snake) {
                if (head.x === segment.x && head.y === segment.y) return endSnakeGame();
            }

            snake.unshift(head);

            // Eat Food
            if (head.x === food.x && head.y === food.y) {
                snakeScore += 10;
                document.getElementById('snakeScore').textContent = snakeScore;
                if (snakeScore > snakeHighScore) {
                    snakeHighScore = snakeScore;
                    localStorage.setItem('snakeHighScore', snakeHighScore);
                    document.getElementById('snakeHighScore').textContent = snakeHighScore;
                }
                spawnFood();
            } else {
                snake.pop();
            }

            // Render Canvas
            ctx.fillStyle = '#0f172a';
            ctx.fillRect(0, 0, snakeCanvas.width, snakeCanvas.height);

            // Draw Food
            ctx.fillStyle = '#ef4444';
            ctx.beginPath();
            ctx.arc(food.x + grid/2, food.y + grid/2, grid/2 - 1, 0, Math.PI * 2);
            ctx.fill();

            // Draw Snake
            snake.forEach((seg, index) => {
                ctx.fillStyle = index === 0 ? '#6366f1' : '#818cf8';
                ctx.fillRect(seg.x, seg.y, grid - 1, grid - 1);
            });
        }

        function endSnakeGame() {
            clearInterval(snakeInterval);
            document.getElementById('snakeOverlay').classList.remove('hidden');
        }

        // --- GAME 3: Memory Matching Game ---
        const memoryEmojis = ['🏀', '⚽', '🥊', '🏊', '🚴', '🏋️'];
        let memoryCards = [];
        let flippedCards = [];
        let matchedPairs = 0;
        let flipsCount = 0;

        function initMemoryGame() {
            const gridEl = document.getElementById('memoryGrid');
            gridEl.innerHTML = '';
            memoryCards = [...memoryEmojis, ...memoryEmojis].sort(() => Math.random() - 0.5);
            flippedCards = [];
            matchedPairs = 0;
            flipsCount = 0;
            document.getElementById('memoryFlips').textContent = flipsCount;

            memoryCards.forEach((emoji, idx) => {
                const card = document.createElement('div');
                card.className = 'h-20 bg-slate-200 dark:bg-slate-700 rounded-2xl flex items-center justify-center text-2xl font-bold cursor-pointer transition-all duration-300 transform select-none';
                card.dataset.index = idx;
                card.dataset.emoji = emoji;
                card.innerHTML = '❓';
                card.onclick = () => flipMemoryCard(card);
                gridEl.appendChild(card);
            });
        }

        function flipMemoryCard(card) {
            if (flippedCards.length >= 2 || card.classList.contains('matched') || flippedCards.includes(card)) return;

            card.innerHTML = card.dataset.emoji;
            card.classList.add('bg-indigo-500', 'text-white');
            flippedCards.push(card);

            if (flippedCards.length === 2) {
                flipsCount++;
                document.getElementById('memoryFlips').textContent = flipsCount;
                const [c1, c2] = flippedCards;

                if (c1.dataset.emoji === c2.dataset.emoji) {
                    c1.classList.add('matched', 'bg-emerald-500');
                    c2.classList.add('matched', 'bg-emerald-500');
                    flippedCards = [];
                    matchedPairs++;
                    if (matchedPairs === memoryEmojis.length) {
                        setTimeout(() => alert(`🎉 축하합니다! ${flipsCount}번 만에 모두 맞추셨습니다!`), 300);
                    }
                } else {
                    setTimeout(() => {
                        c1.innerHTML = '❓';
                        c2.innerHTML = '❓';
                        c1.classList.remove('bg-indigo-500', 'text-white');
                        c2.classList.remove('bg-indigo-500', 'text-white');
                        flippedCards = [];
                    }, 800);
                }
            }
        }

        function resetMemoryGame() {
            initMemoryGame();
        }

        // --- GAME 4: Reaction Time Test ---
        let reactionState = 'idle'; // idle, waiting, ready
        let reactionStartTime = 0;
        let reactionTimeout = null;

        function handleReactionClick() {
            const area = document.getElementById('reactionArea');
            const title = document.getElementById('reactionTitle');
            const sub = document.getElementById('reactionSub');
            const icon = document.getElementById('reactionIcon');

            if (reactionState === 'idle') {
                reactionState = 'waiting';
                area.className = 'w-full h-64 rounded-3xl bg-amber-500 text-white flex flex-col items-center justify-center cursor-pointer select-none transition-all p-6 shadow-inner';
                title.textContent = '초록색이 될 때까지 기다리세요...';
                sub.textContent = '너무 빨리 누르면 패널티!';
                icon.className = 'fa-solid fa-hourglass-start text-4xl mb-3 animate-spin';

                const randomDelay = Math.floor(Math.random() * 3000) + 2000;
                reactionTimeout = setTimeout(() => {
                    reactionState = 'ready';
                    reactionStartTime = Date.now();
                    area.className = 'w-full h-64 rounded-3xl bg-emerald-500 text-white flex flex-col items-center justify-center cursor-pointer select-none transition-all p-6 shadow-inner';
                    title.textContent = '지금 클릭하세요!!';
                    sub.textContent = '클릭!';
                    icon.className = 'fa-solid fa-bolt text-4xl mb-3';
                }, randomDelay);

            } else if (reactionState === 'waiting') {
                clearTimeout(reactionTimeout);
                reactionState = 'idle';
                area.className = 'w-full h-64 rounded-3xl bg-rose-500 text-white flex flex-col items-center justify-center cursor-pointer select-none transition-all p-6 shadow-inner';
                title.textContent = '너무 빨랐습니다! 😅';
                sub.textContent = '다시 시도하려면 클릭하세요.';
                icon.className = 'fa-solid fa-triangle-exclamation text-4xl mb-3';

            } else if (reactionState === 'ready') {
                const reactionTime = Date.now() - reactionStartTime;
                reactionState = 'idle';
                area.className = 'w-full h-64 rounded-3xl bg-indigo-600 text-white flex flex-col items-center justify-center cursor-pointer select-none transition-all p-6 shadow-inner';
                title.textContent = `${reactionTime} ms!`;
                sub.textContent = '다시하려면 클릭하세요.';
                icon.className = 'fa-solid fa-trophy text-4xl mb-3';
                document.getElementById('reactionTimeResult').textContent = `${reactionTime} ms`;
            }
        }

        // --- GAME 5: Tic-Tac-Toe ---
        let tttBoard = Array(9).fill(null);
        let tttGameActive = true;

        function makeTTTMove(index) {
            if (!tttBoard[index] && tttGameActive) {
                tttBoard[index] = 'X';
                renderTTTBoard();
                if (checkTTTWin('X')) {
                    document.getElementById('tttStatus').textContent = '🎉 플레이어 승리!';
                    tttGameActive = false;
                    return;
                }
                if (tttBoard.every(cell => cell !== null)) {
                    document.getElementById('tttStatus').textContent = '🤝 무승부!';
                    tttGameActive = false;
                    return;
                }

                // AI Turn
                document.getElementById('tttStatus').textContent = 'AI 생각 중...';
                setTimeout(tttAiMove, 400);
            }
        }

        function tttAiMove() {
            if (!tttGameActive) return;
            const emptyIndices = tttBoard.map((val, idx) => val === null ? idx : null).filter(val => val !== null);
            if (emptyIndices.length > 0) {
                const randomIndex = emptyIndices[Math.floor(Math.random() * emptyIndices.length)];
                tttBoard[randomIndex] = 'O';
                renderTTTBoard();

                if (checkTTTWin('O')) {
                    document.getElementById('tttStatus').textContent = '🤖 AI 승리!';
                    tttGameActive = false;
                } else {
                    document.getElementById('tttStatus').textContent = '당신의 차례입니다 (X)';
                }
            }
        }

        function checkTTTWin(player) {
            const wins = [
                [0,1,2],[3,4,5],[6,7,8],
                [0,3,6],[1,4,7],[2,5,8],
                [0,4,8],[2,4,6]
            ];
            return wins.some(combination => combination.every(i => tttBoard[i] === player));
        }

        function renderTTTBoard() {
            const cells = document.querySelectorAll('.ttt-cell');
            cells.forEach((cell, idx) => {
                cell.textContent = tttBoard[idx] || '';
                cell.className = `ttt-cell w-20 h-20 bg-slate-200 dark:bg-slate-700 text-3xl font-black rounded-2xl flex items-center justify-center hover:bg-slate-300 dark:hover:bg-slate-600 transition ${
                    tttBoard[idx] === 'X' ? 'text-indigo-600' : 'text-rose-500'
                }`;
            });
        }

        function resetTicTacToe() {
            tttBoard = Array(9).fill(null);
            tttGameActive = true;
            document.getElementById('tttStatus').textContent = '당신의 차례입니다 (X)';
            renderTTTBoard();
        }

        // --- GAME 6: Number Baseball ---
        let baseballSecret = [];

        function resetBaseballGame() {
            baseballSecret = [];
            while(baseballSecret.length < 3) {
                let r = Math.floor(Math.random() * 9) + 1;
                if(!baseballSecret.includes(r)) baseballSecret.push(r);
            }
            document.getElementById('baseballLog').innerHTML = '<div class="text-slate-400 text-center py-4">게임 기록이 여기에 표시됩니다.</div>';
            document.getElementById('baseballInput').value = '';
        }

        function handleBaseballSubmit(e) {
            e.preventDefault();
            const inputEl = document.getElementById('baseballInput');
            const val = inputEl.value;

            if (val.length !== 3 || new Set(val).size !== 3) {
                alert('중복 없는 3자리 숫자를 입력해 주세요 (1~9)');
                return;
            }

            const guess = val.split('').map(Number);
            let strike = 0, ball = 0;

            guess.forEach((num, idx) => {
                if (num === baseballSecret[idx]) strike++;
                else if (baseballSecret.includes(num)) ball++;
            });

            const logEl = document.getElementById('baseballLog');
            if (logEl.querySelector('.text-center')) logEl.innerHTML = '';

            const entry = document.createElement('div');
            entry.className = 'flex justify-between items-center py-1 border-b border-slate-200 dark:border-slate-700';

            if (strike === 3) {
                entry.innerHTML = `<span class="font-bold text-indigo-500">${val}</span> <span class="text-emerald-500 font-bold">🎉 3 스트라이크! 정답입니다!</span>`;
            } else {
                entry.innerHTML = `<span>시도: <strong>${val}</strong></span> <span class="font-semibold text-amber-500">${strike}S ${ball}B</span>`;
            }

            logEl.prepend(entry);
            inputEl.value = '';
        }
    </script>
</body>
</html>
