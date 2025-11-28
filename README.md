<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
b    <meta name="description" content="اختبار الرخصة المهنية التفاعلي للمعلمين - إعداد المعلم فهد الخالدي">
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            /* ألوان متطورة وجذابة */
            --primary: #6366F1;
            --primary-dark: #4F46E5;
            --primary-light: #8B5CF6;
            --accent: #EC4899;
            --accent-dark: #DB2777;
            --accent-light: #F472B6;
            --secondary: #10B981;
            --secondary-dark: #059669;
            --tertiary: #F59E0B;
            --quaternary: #8B5CF6;
            --bg: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            --card-bg: rgba(255, 255, 255, 0.95);
            --text: #1F2937;
            --light-text: #6B7280;
            --border: rgba(255, 255, 255, 0.2);
            --shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            --shadow-hover: 0 20px 40px rgba(0, 0, 0, 0.2);
            --gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            --gradient-dark: linear-gradient(135deg, #5a67d8 0%, #6b46c1 100%);
            --gradient-light: linear-gradient(135deg, #a78bfa 0%, #c4b5fd 100%);
            --accent-gradient: linear-gradient(135deg, #EC4899, #8B5CF6);
            --success-gradient: linear-gradient(135deg, #10B981, #34D399);
            --warning-gradient: linear-gradient(135deg, #F59E0B, #FBBF24);
            --primary-gradient: linear-gradient(135deg, #6366F1, #8B5CF6);
        }

        .dark-theme {
            --bg: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            --card-bg: rgba(30, 41, 59, 0.95);
            --text: #F1F5F9;
            --light-text: #CBD5E1;
            --border: rgba(255, 255, 255, 0.1);
            --shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
            --shadow-hover: 0 20px 40px rgba(0, 0, 0, 0.4);
        }

        * {
            box-sizing: border-box;
            font-family: 'Tajawal', Tahoma, Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        body {
            background: var(--bg);
            color: var(--text);
            line-height: 1.7;
            overflow-x: hidden;
            padding-top: 80px;
            transition: all 0.5s ease;
            min-height: 100vh;
        }

        /* Header بتصميم شفاف وجذاب */
        header {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            color: white;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: var(--shadow);
            border-bottom: 1px solid var(--border);
            padding: 15px 0;
        }

        .header-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 20px;
        }

        .title-section h1 {
            font-size: 1.5rem;
            font-weight: 800;
            background: var(--accent-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-shadow: 0 2px 10px rgba(236, 72, 153, 0.3);
        }

        .header-actions {
            display: flex;
            gap: 10px;
        }

        .theme-btn, .back-btn {
            background: rgba(255, 255, 255, 0.15);
            color: white;
            border: 1px solid rgba(255, 255, 255, 0.2);
            padding: 8px 15px;
            border-radius: 12px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 6px;
            backdrop-filter: blur(10px);
            text-decoration: none;
        }

        .theme-btn:hover, .back-btn:hover {
            background: rgba(255, 255, 255, 0.25);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        /* Main Content */
        main {
            max-width: 1000px;
            margin: 30px auto;
            padding: 0 20px;
        }

        .hero-section {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            color: white;
            border-radius: 24px;
            padding: 40px;
            margin-bottom: 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
        }

        .hero-section::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: var(--accent-gradient);
            opacity: 0.1;
            z-index: -1;
        }

        .hero-content {
            position: relative;
            z-index: 1;
        }

        .hero-title {
            font-size: 2.2rem;
            font-weight: 800;
            margin-bottom: 15px;
            background: linear-gradient(135deg, #fff 0%, #f0f0f0 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-subtitle {
            font-size: 1.1rem;
            margin-bottom: 25px;
            opacity: 0.9;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        /* Cards بتصميم زجاجي */
        .card {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            border-radius: 20px;
            padding: 30px;
            margin-bottom: 25px;
            box-shadow: var(--shadow);
            transition: all 0.4s ease;
            border: 1px solid var(--border);
            position: relative;
            overflow: hidden;
        }

        .card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--accent-gradient);
        }

        .card:hover {
            transform: translateY(-8px) scale(1.02);
            box-shadow: var(--shadow-hover);
        }

        .section-title {
            text-align: center;
            color: var(--text);
            margin-bottom: 30px;
            font-size: 2rem;
            font-weight: 800;
            position: relative;
            padding-bottom: 15px;
        }

        .section-title::after {
            content: "";
            position: absolute;
            bottom: 0;
            right: 50%;
            transform: translateX(50%);
            width: 100px;
            height: 4px;
            background: var(--accent-gradient);
            border-radius: 2px;
        }

        /* تصميم الأسئلة المتطور */
        .question-box {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            padding: 30px;
            margin-bottom: 25px;
            border-radius: 20px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }

        .question-box::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 5px;
            background: var(--primary-gradient);
        }

        .question-box:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-hover);
        }

        .question-number {
            font-size: 1.3em;
            color: var(--primary);
            margin-bottom: 15px;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .question-number i {
            color: var(--accent);
            font-size: 1.2em;
        }

        .question-text {
            font-size: 1.2em;
            margin-bottom: 25px;
            line-height: 1.7;
            color: var(--text);
            font-weight: 500;
        }

        .options {
            position: relative;
        }

        .options label {
            display: flex;
            align-items: center;
            padding: 18px 20px;
            margin: 12px 0;
            border: 2px solid var(--border);
            border-radius: 15px;
            cursor: pointer;
            transition: all 0.3s ease;
            background: var(--card-bg);
            position: relative;
            overflow: hidden;
            font-weight: 500;
        }

        .options label::before {
            content: "";
            position: absolute;
            left: 0;
            top: 0;
            height: 100%;
            width: 0;
            background: var(--primary-gradient);
            transition: width 0.3s ease;
            z-index: 0;
        }

        .options label:hover {
            border-color: var(--primary);
            transform: translateX(-8px);
            box-shadow: 0 5px 15px rgba(99, 102, 241, 0.2);
        }

        .options label:hover::before {
            width: 4px;
        }

        .options input[type="radio"] {
            margin-left: 12px;
            transform: scale(1.3);
            z-index: 1;
        }

        /* عندما تكون الإجابة مقفولة */
        .options label.locked {
            cursor: not-allowed;
            opacity: 0.8;
        }

        .options label.selected {
            background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(139, 92, 246, 0.1));
            border-color: var(--primary);
            box-shadow: 0 5px 15px rgba(99, 102, 241, 0.2);
        }

        .options label.selected::before {
            width: 6px;
            background: var(--success-gradient);
        }

        .options label.correct-answer {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.15), rgba(52, 211, 153, 0.15));
            border-color: var(--secondary);
            box-shadow: 0 5px 15px rgba(16, 185, 129, 0.2);
        }

        .options label.correct-answer::before {
            width: 6px;
            background: var(--success-gradient);
        }

        .options label.wrong-answer {
            background: linear-gradient(135deg, rgba(236, 72, 153, 0.1), rgba(244, 114, 182, 0.1));
            border-color: var(--accent);
            box-shadow: 0 5px 15px rgba(236, 72, 153, 0.2);
        }

        .options label.wrong-answer::before {
            width: 6px;
            background: var(--accent-gradient);
        }

        .correct {
            color: var(--secondary);
            font-weight: bold;
        }

        .wrong {
            color: var(--accent);
            font-weight: bold;
        }

        .explanation {
            margin-top: 25px;
            padding: 25px;
            border-radius: 15px;
            display: none;
            background: linear-gradient(135deg, rgba(99, 102, 241, 0.05), rgba(236, 72, 153, 0.05));
            border-left: 4px solid var(--secondary);
            animation: slideDown 0.5s ease;
            backdrop-filter: blur(10px);
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-15px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .explanation-line {
            padding: 15px;
            margin: 10px 0;
            border-radius: 10px;
            transition: all 0.3s ease;
        }

        .explanation-correct {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.1), rgba(52, 211, 153, 0.1));
            border-right: 3px solid var(--secondary);
        }

        .explanation-wrong-1 {
            background: linear-gradient(135deg, rgba(236, 72, 153, 0.1), rgba(244, 114, 182, 0.1));
            border-right: 3px solid var(--accent);
        }

        .explanation-wrong-2 {
            background: linear-gradient(135deg, rgba(245, 158, 11, 0.1), rgba(251, 191, 36, 0.1));
            border-right: 3px solid var(--tertiary);
        }

        .explanation-wrong-3 {
            background: linear-gradient(135deg, rgba(139, 92, 246, 0.1), rgba(196, 181, 253, 0.1));
            border-right: 3px solid var(--quaternary);
        }

        /* Navigation Buttons */
        .navigation {
            display: flex;
            justify-content: space-between;
            margin-top: 30px;
            gap: 20px;
        }

        .btn {
            padding: 15px 30px;
            border-radius: 15px;
            font-weight: 700;
            text-decoration: none;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            font-size: 1rem;
            border: none;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .btn::before {
            content: "";
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            transition: left 0.6s;
        }

        .btn:hover::before {
            left: 100%;
        }

        .btn-primary {
            background: var(--accent-gradient);
            color: white;
            box-shadow: 0 8px 25px rgba(236, 72, 153, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 35px rgba(236, 72, 153, 0.4);
        }

        .btn-secondary {
            background: var(--primary-gradient);
            color: white;
            box-shadow: 0 8px 25px rgba(99, 102, 241, 0.3);
        }

        .btn-secondary:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 35px rgba(99, 102, 241, 0.4);
        }

        .btn:disabled {
            background: #9CA3AF;
            cursor: not-allowed;
            transform: none;
            box-shadow: none;
        }

        .btn:disabled:hover::before {
            left: -100%;
        }

        /* Progress Bar متطور */
        .progress-bar {
            height: 15px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            margin-bottom: 30px;
            overflow: hidden;
            box-shadow: inset 0 2px 5px rgba(0, 0, 0, 0.1);
            position: relative;
            backdrop-filter: blur(10px);
        }

        .progress {
            height: 100%;
            background: var(--accent-gradient);
            width: 0%;
            transition: width 0.5s ease;
            border-radius: 10px;
            position: relative;
            overflow: hidden;
        }

        .progress::after {
            content: "";
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
            animation: shimmer 1.5s infinite;
        }

        @keyframes shimmer {
            0% { left: -100%; }
            100% { left: 100%; }
        }

        /* Results Box */
        #result-box, #current-score {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            padding: 30px;
            margin-top: 30px;
            border-radius: 20px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
            display: none;
            animation: slideUp 0.6s ease;
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .controls {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 30px;
            flex-wrap: wrap;
            gap: 20px;
        }

        .quiz-info {
            font-size: 1rem;
            color: var(--light-text);
            background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(236, 72, 153, 0.1));
            padding: 10px 20px;
            border-radius: 25px;
            font-weight: 600;
            backdrop-filter: blur(10px);
        }

        /* Timer متطور */
        #timer {
            font-size: 1.1rem;
            font-weight: bold;
            color: white;
            margin-left: 20px;
            display: flex;
            align-items: center;
            gap: 8px;
            background: rgba(255, 255, 255, 0.2);
            padding: 10px 20px;
            border-radius: 25px;
            backdrop-filter: blur(10px);
        }

        .timer-warning {
            color: #FECACA !important;
            animation: pulse 0.8s infinite;
            background: rgba(254, 202, 202, 0.3) !important;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        /* Questions List متطور */
        #questions-list {
            margin-top: 25px;
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            padding: 30px;
            border-radius: 20px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
            display: none;
        }

        #questions-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(60px, 1fr));
            gap: 12px;
            margin: 20px 0;
        }

        .question-status-grid {
            width: 60px;
            height: 60px;
            border: 2px solid var(--border);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-weight: 700;
            transition: all 0.3s ease;
            background: var(--card-bg);
            position: relative;
            overflow: hidden;
            font-size: 1.1rem;
        }

        .question-status-grid::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--accent-gradient);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .question-status-grid:hover {
            transform: translateY(-3px) scale(1.1);
            box-shadow: var(--shadow);
        }

        .question-status-grid.current {
            border-color: var(--accent);
            background: var(--accent);
            color: white;
            transform: scale(1.1);
        }

        .question-status-grid.answered {
            border-color: var(--secondary);
            background: var(--secondary);
            color: white;
        }

        .question-status-grid.flagged {
            border-color: var(--tertiary);
            background: var(--tertiary);
            color: var(--text);
        }

        .question-status-grid span {
            position: relative;
            z-index: 1;
        }

        .legend {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
            font-size: 0.9rem;
        }

        .legend-item {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        /* تحسينات للوضع الداكن */
        .dark-theme .question-status-grid {
            border-color: var(--border);
        }

        .dark-theme .options label {
            background: var(--card-bg);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            body {
                padding-top: 70px;
            }
            
            .header-container {
                padding: 0 15px;
                flex-direction: column;
                gap: 15px;
            }
            
            .title-section h1 {
                font-size: 1.3rem;
            }
            
            .hero-title {
                font-size: 1.8rem;
            }
            
            .hero-subtitle {
                font-size: 1rem;
            }
            
            .card, .question-box {
                padding: 25px;
            }
            
            .navigation {
                flex-direction: column;
                gap: 15px;
            }
            
            .btn {
                width: 100%;
                justify-content: center;
            }
            
            .controls {
                flex-direction: column;
                align-items: stretch;
            }
            
            #questions-grid {
                grid-template-columns: repeat(auto-fill, minmax(50px, 1fr));
            }
            
            .question-status-grid {
                width: 50px;
                height: 50px;
                font-size: 1rem;
            }
        }

        @media (max-width: 480px) {
            .header-container {
                text-align: center;
            }
            
            .header-actions {
                justify-content: center;
            }
            
            .question-box {
                padding: 20px;
            }
            
            .options label {
                padding: 15px;
            }
            
            .hero-section {
                padding: 25px;
            }
            
            .section-title {
                font-size: 1.6rem;
            }
        }

        /* تأثيرات إضافية */
        .fade-in {
            animation: fadeIn 0.8s ease;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .bounce-in {
            animation: bounceIn 0.8s ease;
        }

        @keyframes bounceIn {
            0% {
                opacity: 0;
                transform: scale(0.3);
            }
            50% {
                opacity: 1;
                transform: scale(1.05);
            }
            70% {
                transform: scale(0.95);
            }
            100% {
                opacity: 1;
                transform: scale(1);
            }
        }

        /* تأثيرات الجلاس مورفيزم */
        .glass-effect {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        /* رسوم متحركة للخلفية */
        .bg-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            opacity: 0.3;
        }

        .floating-shapes {
            position: absolute;
            width: 100%;
            height: 100%;
        }

        .shape {
            position: absolute;
            background: var(--accent-gradient);
            border-radius: 50%;
            opacity: 0.1;
            animation: float 6s ease-in-out infinite;
        }

        .shape:nth-child(1) {
            width: 100px;
            height: 100px;
            top: 10%;
            left: 10%;
            animation-delay: 0s;
        }

        .shape:nth-child(2) {
            width: 150px;
            height: 150px;
            top: 60%;
            right: 10%;
            animation-delay: 2s;
        }

        .shape:nth-child(3) {
            width: 80px;
            height: 80px;
            bottom: 20%;
            left: 20%;
            animation-delay: 4s;
        }

        @keyframes float {
            0%, 100% {
                transform: translateY(0) rotate(0deg);
            }
            50% {
                transform: translateY(-20px) rotate(180deg);
            }
        }
    </style>
</head>
<body>
    <!-- رسوم متحركة للخلفية -->
    <div class="bg-animation">
        <div class="floating-shapes">
            <div class="shape"></div>
            <div class="shape"></div>
            <div class="shape"></div>
        </div>
    </div>

    <!-- Header -->
    <header class="glass-effect">
        <div class="header-container">
            <div class="title-section">
                <h1>اختبار الرخصة المهنية التفاعلي</h1>
            </div>
            <div class="header-actions">
                <button class="theme-btn" id="themeBtn">
                    <i class="fas fa-moon"></i>
                </button>
                <a href="#" class="back-btn">
                    <i class="fas fa-arrow-right"></i>
                    العودة للرئيسية
                </a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <!-- Hero Section -->
        <section class="hero-section glass-effect">
            <div class="hero-content">
                <h1 class="hero-title">اختبار الرخصة المهنية للمعلمين</h1>
                <p class="hero-subtitle">تم إعداد هذا الاختبار التفاعلي لمحاكاة الاختبار الرسمي للرخصة المهنية، ويقدم تغذية راجعة فورية لجميع الإجابات</p>
                <div class="quiz-info">إعداد: المعلم فهد الخالدي</div>
            </div>
        </section>

        <!-- Progress Bar -->
        <div class="progress-bar glass-effect">
            <div class="progress" id="progress"></div>
        </div>

        <!-- Quiz Container -->
        <div id="quiz"></div>

        <!-- Controls -->
        <div class="controls">
            <div class="quiz-info" id="quiz-info"></div>
            <div id="timer">⏱️ <span id="time-display">45:00</span></div>
            <div style="display: flex; gap: 15px; flex-wrap: wrap;">
                <button class="btn btn-primary" onclick="showQuestionsList()">
                    <i class="fas fa-list"></i>
                    قائمة الأسئلة
                </button>
                <button class="btn btn-secondary" onclick="toggleMarkForReview()" id="mark-review-btn">
                    <i class="fas fa-flag"></i>
                    وضع علامة للمراجعة
                </button>
                <button class="btn btn-primary" onclick="finishQuiz()">
                    <i class="fas fa-flag-checkered"></i>
                    إنهاء الاختبار
                </button>
                <button class="btn btn-secondary" onclick="showCurrentScore()">
                    <i class="fas fa-chart-bar"></i>
                    عرض الدرجات الحالية
                </button>
            </div>
        </div>

        <!-- Questions List -->
        <div id="questions-list" class="card">
            <h3 style="color: var(--text); margin-bottom: 20px; display: flex; align-items: center; gap: 12px;">
                <i class="fas fa-th-list"></i>
                قائمة الأسئلة
            </h3>
            <div id="questions-grid"></div>
            <div class="legend">
                <div class="legend-item">
                    <div class="question-status-grid" style="background: var(--accent); color: white;"></div>
                    <span>السؤال الحالي</span>
                </div>
                <div class="legend-item">
                    <div class="question-status-grid" style="background: var(--secondary); color: white;"></div>
                    <span>تمت الإجابة</span>
                </div>
                <div class="legend-item">
                    <div class="question-status-grid" style="background: var(--tertiary); color: var(--text);"></div>
                    <span>معلم للمراجعة</span>
                </div>
                <div class="legend-item">
                    <div class="question-status-grid" style="background: var(--card-bg); border-color: var(--border);"></div>
                    <span>لم يتم الإجابة</span>
                </div>
            </div>
            <button class="btn btn-primary" onclick="hideQuestionsList()" style="margin-top:20px; width: 100%;">
                <i class="fas fa-times"></i>
                إغلاق القائمة
            </button>
        </div>

        <!-- Current Score -->
        <div id="current-score" class="card">
            <h3 style="color: var(--text); margin-bottom: 20px; display: flex; align-items: center; gap: 12px;">
                <i class="fas fa-chart-bar"></i>
                الدرجات الحالية
            </h3>
            <p id="current-correct" style="margin-bottom: 15px; font-size: 1.1rem;"></p>
            <p id="current-percentage" style="font-weight: bold; font-size: 1.3rem; color: var(--primary);"></p>
        </div>

        <!-- Final Results -->
        <div id="result-box" class="card">
            <h3 id="result" style="color: var(--text); margin-bottom: 20px;"></h3>
            <p id="percentage" style="font-size: 1.4rem; margin-bottom: 15px;"></p>
            <p id="evaluation" style="font-weight: bold; font-size: 1.3rem;"></p>
        </div>
    </main>

    <script>
        // مصفوفة الأسئلة
        const questions=[
  {
    "id": 1,
    "q": "إذا كنت تخطط لاستثارة التفكير الإبداعي لدى الطلاب، فيجب أن تكلف الطلاب بنشاطات وتطرح أسئلة تركز على التفكير:",
    "options": ["التباعدي", "التقاربي", "التقييمي", "الاستقرائي"],
    "answer": 0,
    "explanations": {
      "correct": "التفكير التباعدي هو الأنسب لاستثارة الإبداع لأنه يشجع على توليد أكبر عدد ممكن من الأفكار والحلول المتنوعة والمبتكرة. هذا النوع من التفكير يتسم بالمرونة والأصالة والطلاقة في توليد الأفكار، حيث لا يقتصر على إجابة واحدة صحيحة بل يفتح المجال لاحتمالات متعددة. يعمل التفكير التباعدي على تنمية القدرة على النظر للمشكلات من زوايا مختلفة وإنتاج حلول غير تقليدية.",
      "wrong1": "التفكير التقاربي يركز على الوصول لإجابة واحدة صحيحة ومحددة، مما يحد من الإبداع والابتكار. هذا النوع من التفكير يتناسب مع المسائل ذات الحل الوحيد ولكنه لا يشجع على توليد أفكار جديدة ومتنوعة. يعتمد على المنطق والتحليل الضيق بدلاً من التوسع في الاحتمالات والبدائل المبتكرة.",
      "wrong2": "التفكير التقييمي مهم لتقييم جودة الأفكار ولكن لا يناسب مرحلة توليد الأفكار الإبداعية. يركز هذا النوع على الحكم على الأفكار وتقييمها وفق معايير محددة مما قد يحد من حرية التفكير والتعبير. يعد مناسباً للمراحل المتأخرة من عملية التفكير وليس لمرحلة الاستثارة والإبداع الأولى.",
      "wrong3": "التفكير الاستقرائي يعتمد على الانتقال من الجزء إلى الكل ومن الأمثلة إلى القواعد العامة، وهو مفيد للتحليل ولكن ليس الأفضل للإبداع. يساعد في استخلاص النتائج من الملاحظات ولكنه لا يشجع بالضرورة على توليد أفكار جديدة ومبتكرة. يعتبر أداة جيدة للفهم والاستدلال لكنه لا يخدم هدف استثارة التفكير الإبداعي بشكل مباشر."
    }
  },
  {
    "id": 2,
    "q": "أراد معلم ترتيب البيئة الصفية للأطفال ذوي التوحد، وإن من أفضل الأساليب الرائدة عالمياً لتحقيق ذلك:",
    "options": ["المنظم", "العقلي", "الجماعي", "غير المباشر"],
    "answer": 0,
    "explanations": {
      "correct": "أسلوب البيئة المنظمة هو الأفضل للأطفال ذوي التوحد لأنه يوفر بيئة متوقعة ومنظمة تقلل من القلق وتزيد الشعور بالأمان. يعتمد هذا الأسلوب على تنظيم واضح للمكان والزمان والأنشطة مما يساعد الطفل على فهم التوقعات والتكيف مع البيئة الصفية. يشمل استخدام الجداول البصرية والمناطق المحددة بوضوح وإجراءات روتينية منتظمة تناسب احتياجات الأطفال ذوي التوحد.",
      "wrong1": "الأسلوب العقلي يركز على العمليات الذهنية والمعرفية المجردة التي قد تكون صعبة على الأطفال ذوي التوحد. لا يأخذ في الاعتبار الصعوبات التي يواجهها أطفال التوحد في فهم المفاهيم المجردة والتواصل الاجتماعي. يعتبر غير مناسب لأنهم يحتاجون إلى دعم ملموس وبصري أكثر من التركيز على الجانب العقلي المجرد.",
      "wrong2": "الأسلوب الجماعي يتطلب مهارات اجتماعية وتفاعلية قد تكون محدودة عند الأطفال ذوي التوحد. يعتمد على العمل المشترك والتواصل المستمر مما يشكل تحدياً كبيراً لهذه الفئة. لا يراعي الحاجة الفردية للطفل التوحدي وصعوباته في التفاعل الاجتماعي والاستجابة للمؤثرات الجماعية.",
      "wrong3": "الأسلوب غير المباشر يعتمد على التلميحات والتوجيه الضمني الذي قد لا يفهمه الأطفال ذوي التوحد. يحتاج هؤلاء الأطفال إلى توجيه مباشر وواضح وتعليمات صريحة بسبب صعوباتهم في فهم الإشارات غير المباشرة. يعتبر هذا الأسلوب غير فعال معهم لأنه يفترض قدرة على استنتاج المعاني الضمنية والتي تكون محدودة لدى many أطفال التوحد."
    }
  },
  {
    "id": 3,
    "q": "أي من العبارات الآتية تمثل رأياً لا حقيقة؟",
    "options": ["أنزل القرآن بلسان عربي مبين", "تتفاوت درجات الحرارة بين منطقة وأخرى", "كثرة القراءة تسهم في نمو العقل وتزيد المعرفة", "التسامح أجل الأخلاق التي يتصف بها الإنسان"],
    "answer": 3,
    "explanations": {
      "correct": "عبارة 'التسامح أجل الأخلاق التي يتصف بها الإنسان' تمثل رأياً لأنها تعبر عن تقييم ذاتي وقيمة أخلاقية تختلف باختلاف الثقافات والمنظورات الشخصية. الرأي يعبر عن وجهة نظر شخصية وقناعة فردية يمكن أن تختلف من شخص لآخر ولا يمكن إثباتها بشكل موضوعي مطلق. يعتمد تقييم الأخلاق على المعايير الثقافية والاجتماعية والدينية المختلفة مما يجعل هذه العبارة قابلة للنقاش والاختلاف.",
      "wrong1": "عبارة 'أنزل القرآن بلسان عربي مبين' تمثل حقيقة دينية وتاريخية مثبتة في القرآن الكريم والسنة النبوية. هذه حقيقة ثابتة لا تقبل الجدل أو الاختلاف بين المسلمين وهي مدونة في المصادر الإسلامية الموثوقة. تعتبر من الحقائق الدينية القطعية التي وردت في النصوص الشرعية بشكل واضح وصريح.",
      "wrong2": "عبارة 'تتفاوت درجات الحرارة بين منطقة وأخرى' تمثل حقيقة علمية قابلة للقياس والملاحظة والتأكد التجريبي. يمكن إثبات هذه الحقيقة من خلال القياسات العلمية والبيانات المناخية المسجلة في مختلف المناطق. تعتبر ظاهرة طبيعية مثبتة علمياً ولا تعتمد على الرأي الشخصي أو التقييم الذاتي.",
      "wrong3": "عبارة 'كثرة القراءة تسهم في نمو العقل وتزيد المعرفة' تمثل حقيقة تربوية وعلمية مدعومة بالأبحاث والدراسات العلمية. هناك إجماع علمي على تأثير القراءة في تنمية القدرات العقلية وزيادة المخزون المعرفي للإنسان. تعتمد على أدلة بحثية ونتائج دراسات متعددة تؤكد العلاقة الإيجابية بين القراءة وتطور المعرفة."
    }
  },
  {
    "id": 4,
    "q": "أسلوب يستخدم للإخبار عن قصة خيالية أو واقعية وفقا لترتيب أحداثها. العبارة تصف نوعاً من الكتابة:",
    "options": ["التوضيحية", "الإقناعية", "السردية", "الوصفية"],
    "answer": 2,
    "explanations": {
      "correct": "الكتابة السردية هي التي تعتمد على سرد الأحداث وفق تسلسل زمني ومنطقي سواء كانت قصة خيالية أو واقعية. تتميز بتتابع الأحداث ووجود بداية ووسط ونهاية، وتهدف إلى نقل تجربة أو قصة للقارئ. تحتوي على عناصر أساسية مثل الشخصيات والزمان والمكان والحبكة الدرامية التي تطور الأحداث نحو الذروة ثم الحل.",
      "wrong1": "الكتابة التوضيحية تركز على شرح فكرة أو مفهوم أو عملية بشكل موضوعي وواضح. تهدف إلى إيضاح المعلومات وتقديم解释 مفصلة دون وجود قصة أو تسلسل أحداث. تعتمد على الحقائق والبيانات والمعلومات الدقيقة أكثر من الاعتماد على السرد القصصي.",
      "wrong2": "الكتابة الإقناعية تهدف إلى تغيير آراء القارئ أو دفعه لاتخاذ موقف معين through الحجج والبراهين. تركز على تقديم الأدلة والمنطق لإقناع القارئ بوجهة نظر معينة rather than سرد قصة. تعتمد على المنطق والعاطفة والأخلاق لتؤثر في القارئ وتغير معتقداته أو سلوكه.",
      "wrong3": "الكتابة الوصفية تهتم بتصوير المشاهد والأشخاص والأماكن باستخدام التفاصيل الحسية. تهدف إلى خلق صورة ذهنية حية في خيال القارئ من خلال وصف دقيق للعناصر. تركز على الجوانب الحسية والمشاعر أكثر من التركيز على تسلسل الأحداث والقصة."
    }
  },
  {
    "id": 5,
    "q": "يمكن للمعلم تشجيع الطلاب على استخدام أسلوب تقويم الأقران بهدف:",
    "options": ["استثمار زمن الحصة الدراسية", "تعزيز العلاقات الاجتماعية بين الطلاب", "تعزيز قيمة اعتماد الطالب على الآخرين", "جعل الطالب قادراً على نقد عمله وعمل الآخرين"],
    "answer": 3,
    "explanations": {
      "correct": "الهدف الرئيسي من تقويم الأقران هو تنمية قدرة الطالب على النقد البناء لعملهم وعمل زملائهم، مما يعزز مهارات التفكير الناقد. يساعد هذا الأسلوب الطلاب على تطوير مهارات التقييم الذاتي والفهم الأعمق لمعايير الجودة في العمل. يعزز القدرة على تقديم ملاحظات بناءة واستقبال النقد بشكل إيجابي، وهي مهارات أساسية للتعلم المستمر.",
      "wrong1": "استثمار زمن الحصة الدراسية قد يكون نتيجة ثانوية لتقويم الأقران وليس الهدف الأساسي منه. بينما يمكن أن يوفر الوقت للمعلم، إلا أن الفائدة التعليمية تتجاوز مجرد توفير الوقت. الهدف الحقيقي هو التعلم النشط وتنمية المهارات وليس فقط الكفاءة الزمنية.",
      "wrong2": "تعزيز العلاقات الاجتماعية قد يحدث كنتيجة ثانوية ولكن ليس الهدف الأساسي من تقويم الأقران. العملية تركز على الجوانب التعليمية والتقييمية أكثر من الجوانب الاجتماعية. العلاقات الاجتماعية المحسنة تكون نتيجة للتفاعل الإيجابي وليس الهدف الرئيسي للتقييم.",
      "wrong3": "تعزيز اعتماد الطالب على الآخرين ليس الهدف المنشود، بل المطلوب هو تعزيز الاستقلالية والمسؤولية الذاتية. تقويم الأقران يهدف إلى بناء الثقة بالنفس والقدرة على التقييم الذاتي أكثر من الاعتماد على الآخرين. العملية تهدف إلى تمكين الطالب وليس جعله معتمداً على تقييم زملائه."
    }
  },
  {
    "id": 6,
    "q": "طلب المعلم علي من طلابه أثناء أنشطة استخدام التقنية لإنجاز مهام تعليمية أن يوظفوا إستراتيجية التفكير الناقد:",
    "options": ["طرح قضايا نقاشية واقتراح حلول", "استثارة تفكير الطلاب من خلال التفكر", "تقسيم الطلاب إلى مجموعات وجمع معلومات", "تقويم المواقع الإلكترونية للتمييز بين المعلومات الصحيحة وغير الصحيحة"],
    "answer": 3,
    "explanations": {
      "correct": "تقويم المواقع الإلكترونية والتمييز بين المعلومات الصحيحة والخاطئة يمثل تطبيقاً مباشراً للتفكير الناقد في عصر المعلومات. يتطلب هذا المهارات التحليلية والتقييمية الأساسية في التفكير الناقد مثل التحقق من المصادر وتمييز الحقائق من الآراء. ينمي قدرة الطلاب على الحكم على مصداقية المعلومات واتخاذ قرارات مستنيرة بناءً على أدلة موثوقة.",
      "wrong1": "طرح قضايا نقاشية واقتراح حلول يمثل تفكيراً إبداعياً وحل مشكلات أكثر من كونه تفكيراً ناقداً. بينما يتضمن بعض عناصر النقد، إلا أنه يركز على توليد الحلول أكثر من تحليل المعلومات وتقييمها. يعتبر جزءاً من عملية التفكير الشاملة ولكن لا يعكس الجوهر التحليلي للتفكير الناقد.",
      "wrong2": "استثارة تفكير الطلاب من خلال التفكر يمثل تفكيراً تأملياً وليس بالضرورة تفكيراً ناقداً. التفكر يركز على التأمل الذاتي والاستبطان أكثر من التحليل المنطقي المنهجي. يعتبر مهماً للوعي الذاتي ولكن لا يعادل المهارات التحليلية والتقييمية للتفكير الناقد.",
      "wrong3": "تقسيم الطلاب إلى مجموعات وجمع المعلومات يركز على العمل التعاوني وجمع البيانات أكثر من التفكير الناقد. بينما يمكن أن يكون خطوة أولى في عملية البحث، إلا أنه لا يتضمن بالضرورة التحليل النقدي والتقييم. يعتبر إعداداً للتفكير الناقد وليس تطبيقاً مباشراً لمهاراته."
    }
  },
  {
    "id": 7,
    "q": "عند التخطيط لتدريس وحدة الأدب العربي الحديث، المعلم استخدم منظم متقدم للوحدة لتهيئة أذهان الطلاب:",
    "options": ["توجيهية", "تنشيطية", "افتتاحية", "انتقالية"],
    "answer": 2,
    "explanations": {
      "correct": "المنظم الافتتاحي هو الأنسب لتهيئة أذهان الطلاب حيث يقدم نظرة عامة شاملة عن الوحدة الدراسية وأهدافها ومحتواها. يعمل هذا المنظم على ربط المعرفة السابقة بالمعرفة الجديدة ويساعد في بناء إطار مفاهيمي ينظم فيه الطلاب معلوماتهم. يسهل عملية الفهم والاستيعاب من خلال تقديم خريطة ذهنية مسبقة للموضوعات التي سيتم دراستها في الوحدة.",
      "wrong1": "المنظم التوجيهي يركز على توجيه الطلاب نحو المهام والإجراءات الصفية وليس على البنية المفاهيمية للوحدة. يعطي تعليمات حول كيفية تنفيذ الأنشطة أكثر من تركيزه على المحتوى المعرفي. لا يخدم الغرض الأساسي من المنظم المتقدم المتمثل في تهيئة الأذهان للمفاهيم الأساسية.",
      "wrong2": "المنظم التنشيطي يهدف إلى تحفيز الطلاب وجذب انتباههم ولكن لا يقدم الإطار المفاهيمي الشامل للوحدة. يركز على الجانب الوجداني والدافعي أكثر من الجانب المعرفي التنظيمي. يعتبر مكملاً للمنظم الافتتاحي وليس بديلاً عنه في بناء الإطار المفاهيمي.",
      "wrong3": "المنظم الانتقالي يستخدم للربط بين أجزاء الدرس أو الانتقال بين المفاهيم وليس لبداية الوحدة. يعمل على تسهيل الانتقال بين أجزاء المحتوى التعليمي بعد أن يكون الطلاب قد بدأوا في التعلم. لا يناسب مرحلة البداية والتهيئة للوحدة الدراسية الجديدة."
    }
  },
  {
    "id": 8,
    "q": "أعلن المعلم نايف عن دورة استخدام الحاسوب، ما التصرف الأنسب للمعلم عبد الله صاحب الخبرة:",
    "options": ["حضور الدورة والمشاركة بفاعلية", "الاعتذار عن عدم حضور الدورة", "حضور الدورة مجاملة بدون مشاركة", "الاعتذار لقناعته بأفضلية خبرته"],
    "answer": 0,
    "explanations": {
      "correct": "حضور الدورة والمشاركة بفاعلية هو التصرف الأنسب للمعلم عبد الله، لأنه يعكس روح التعلم المستمر والتعاون المهني. حتى المعلمون ذوو الخبرة يمكنهم الاستفادة من الدورات التدريبية لاكتساب وجهات نظر جديدة، وتحديث معارفهم، وتبادل الخبرات مع الزملاء. كما أن مشاركته الفاعلة يمكن أن تثري الدورة بخبراته العملية وتظهر قدوة إيجابية للزملاء الأقل خبرة. التعلم المستمر هو سمة المعلم الناجح، والخبرة السابقة لا تعني أن المعلم لا يحتاج إلى تطوير مهاراته باستمرار.",
      "wrong1": "الاعتذار عن عدم حضور الدورة يفوت فرصة للتطوير المهني وتبادل الخبرات. هذا التصرف يعكس عدم الاهتمام بالتعلم المستمر وقد يرسل رسالة سلبية للزملاء حول أهمية التطوير المهني. كما أنه يحرم المعلم من فرصة تحديث معارفه والتعرف على المستجدات في مجال تخصصه.",
      "wrong2": "حضور الدورة مجاملة بدون مشاركة لا يحقق الفائدة المرجوة ولا يظهر الاحترام الحقيقي للمجهود المبذول في تنظيم الدورة. المشاركة السلبية لا تثري التجربة التعليمية للمشارك ولا تساهم في تطوير الزملاء. كما أن هذا التصرف يعتبر إهداراً للوقت والجهد دون تحقيق أي فائدة حقيقية.",
      "wrong3": "الاعتذار لقناعته بأفضلية خبرته يعكس غروراً مهنياً ويتعارض مع مبدأ التعلم المستمر. الخبرة السابقة لا تعني المعرفة الكاملة، فالتقنية تتطور باستمرار وهناك دائماً جوانب جديدة يمكن تعلمها. هذا الموقف قد يعزز العزلة المهنية ويحد من فرص النمو والتطور المهني."
    }
  },
  {
    "id": 9,
    "q": "من سمات المتحدث الجيد:",
    "options": ["يتنبه لردود أفعال الجمهور", "يكثر من الشواهد الخارجية", "يبتعد عن النقاش والحوار", "يوصي ويشير بيده كثيراً"],
    "answer": 0,
    "explanations": {
      "correct": "التنبه لردود أفعال الجمهور من أهم سمات المتحدث الجيد لأنه يمكنه من تعديل أسلوبه وفقاً لاستجابة المستمعين. يساعد هذا التنبه في بناء تواصل فعال وتفاعل إيجابي مع الجمهور، حيث يمكن للمتحدث أن يلاحظ علامات الملل أو عدم الفهم فيعدل طريقة عرضه. القدرة على قراءة لغة الجسد وتعبيرات الوجه تمكن المتحدث من تلبية احتياجات الجمهور وتحقيق التواصل الفعال.",
      "wrong1": "الإكثار من الشواهد الخارجية قد يشوش على الرسالة الرئيسية ويجعل العرض ممللاً وغير مركز. الاستشهاد المناسب مفيد لكن الإفراط فيه يشتت انتباه الجمهور ويضعف ترابط الأفكار. الجودة في اختيار الشواهد أهم من الكمية، والشواهد يجب أن تخدم الفكرة الأساسية لا أن تطغى عليها.",
      "wrong2": "الابتعاد عن النقاش والحوار يحد من فرص التفاعل مع الجمهور ويجعل العرض أحادي الاتجاه. النقاش والحوار يثريان الموضوع ويساعدان في توضيح الأفكار وتبادل الخبرات. التفاعل مع الجمهور يجعلهم شركاء في العملية التواصلية ويزيد من فعالية الرسالة.",
      "wrong3": "الإكثار من الإشارة باليد قد يكون مشتتاً للانتباه ويظهر المتحدث بمظهر غير متزن. الإيماءات المعتدلة والمتناسقة مع الكلام مفيدة، لكن الإفراط فيها يضعف المصداقية ويشغل الجمهور عن المحتوى. لغة الجسد يجب أن تكون متوازنة ومدروسة لتعزيز الرسالة لا لإضعافها."
    }
  },
  {
    "id": 10,
    "q": "أي من النشاطات غير الصفية لا يصلح لتعزيز قضية المحافظة على المباني التراثية?",
    "options": ["حث أصحاب المباني التراثية على تجديد مظهرها", "تقديم مبادرات لتحويل المباني التراثية إلى مبان حديثة", "إعداد فيلم وثائقي عن المباني التراثية", "توزيع مطويات للتوعية بأهمية المباني التراثية"],
    "answer": 1,
    "explanations": {
      "correct": "تقديم مبادرات لتحويل المباني التراثية إلى مبان حديثة لا يصلح لتعزيز قضية المحافظة عليها لأنه يتعارض مع الهدف الأساسي من الحفاظ على التراث. تحويل المباني التراثية إلى مبان حديثة يفقدها قيمتها التاريخية والمعمارية المميزة ويشوه طابعها الأصلي. الحفاظ على المباني التراثية يعني المحافظة على شكلها ومكوناتها الأصلية مع ترميمها بشكل علمي يحافظ على هويتها التاريخية.",
      "wrong1": "حث أصحاب المباني التراثية على تجديد مظهرها يساهم في الحفاظ عليها وتحسين حالتها مع المحافظة على طابعها الأصلي. التجديد المدروس الذي يحافظ على العناصر المعمارية والزخرفية الأصلية يعزز قيمة المبنى التراثي. هذا النشاط يشجع الملاك على الاهتمام بمبانيهم والمحافظة على تراثهم المعماري.",
      "wrong2": "إعداد فيلم وثائقي عن المباني التراثية وسيلة فعالة لنشر الوعي بأهميتها وقيمتها التاريخية والمعمارية. يساعد في توثيق التراث المعماري وتعريف الجمهور بأهمية الحفاظ عليه للأجيال القادمة. الأفلام الوثائقية أداة توعوية مهمة تجذب اهتمام مختلف شرائح المجتمع بقضايا التراث.",
      "wrong3": "توزيع مطويات للتوعية بأهمية المباني التراثية وسيلة مباشرة وفعالة لنشر الثقافة التراثية في المجتمع. تساعد في تعريف الناس بقيمة التراث المعماري وأهمية الحفاظ عليه كجزء من الهوية الوطنية. المطويات تصل لشرائح واسعة من المجتمع وتقدم معلومات مبسطة عن أهمية التراث وكيفية المحافظة عليه."
    }
  },
  {
    "id": 11,
    "q": "مصدر كلمة (تعلم):",
    "options": ["علم", "تعلم", "علوم", "تعليم"],
    "answer": 1,
    "explanations": {
      "correct": "مصدر كلمة (تعلم) هو (تعلم) نفسه لأنه مصدر الفعل الخماسي تعلم يتعلم. المصدر في اللغة العربية هو الاسم الدال على الحدث المجرد من الزمن، وكلمة تعلم تمثل المصدر الأساسي للفعل. الفعل تعلم من الأفعال الخماسية التي يكون مصدرها على وزن تفعل، وهذا يتوافق مع القواعد الصرفية العربية.",
      "wrong1": "كلمة (علم) ليست مصدراً لكلمة (تعلم) بل هي مصدر الفعل الثلاثي علم يعلم. هناك فرق صرفي بين الفعل الثلاثي المزيد بحرفين والخماسي، فالمصادر تختلف حسب وزن الفعل. علم تمثل المصدر للفعل الثلاثي بينما تعلم فعل خماسي يحتاج لمصدر مختلف.",
      "wrong2": "كلمة (علوم) ليست مصدراً للفعل تعلم بل هي جمع لكلمة علم. العلوم تمثل المجال المعرفي أو الجمع من العلم، ولا يمكن اعتبارها مصدراً لفعل التعلم. المصدر يجب أن يكون اسماً مجرداً للحدث وليس اسماً لجمع المعرفة.",
      "wrong3": "كلمة (تعليم) ليست مصدراً للفعل تعلم بل هي مصدر للفعل علم الذي يتعدى بنفسه أو بالهمزة. التعليم يمثل عملية إيصال المعرفة من المعلم إلى المتعلم، بينما التعلم يمثل عملية اكتساب المعرفة من قبل المتعلم نفسه."
    }
  },
  {
    "id": 12,
    "q": "ضع علامات الترقيم المناسبة للجملة: أعجب معلم بإجابة أحد طلابه فقال ( ) ما أجمل هذه الإجابة ( )",
    "options": [":  !", "/  !", "،  /", "/  ."],
    "answer": 0,
    "explanations": {
      "correct": "النقطتان الرأسيتان (:) تناسب بعد كلمة (فقال) لأنها تسبق كلاماً منقولاً مباشراً، وعلامة التعجب (!) تناسب نهاية الجملة لأنها تعبر عن الانبهار والإعجاب. هذه العلامات تساعد في توضيح المعنى وإبراز المشاعر التي يعبر عنها المعلم. الترقيم الصحيح يجعل النص أكثر وضوحاً وسلاسة في القراءة.",
      "wrong1": "استخدام الشرطة (/) غير مناسب في هذا الموضع لأنها تستخدم للأغراض المختلفة عن الترقيم الأساسي. الشرطة تستخدم في الفواصل الثانوية أو في حالات خاصة مثل المقابلات والحوارات، وليس للربط بين القول والمقول. لا تعبر الشرطة عن العلاقة المنطقية بين الفعل والكلام المنقول.",
      "wrong2": "استخدام الفاصلة (،) مع الشرطة (/) لا يحقق الغرض من الترقيم الصحيح للجملة. الفاصلة تستخدم للفصل بين الجمل القصيرة أو العناصر المتعاطفة، وليس قبل الكلام المنقول المباشر. هذا الخيار لا يعبر عن المشاعر التي تتضمنها الجملة بشكل مناسب.",
      "wrong3": "استخدام الشرطة (/) والنقطة (.) لا يناسب معنى الجملة لأن النقطة تعبر عن نهاية الجملة التقريرية العادية. الجملة تحتاج إلى علامة تعجب للتعبير عن الانفعال والإعجاب، والنقطة تجعل المعنى باهتاً وضعيفاً. الترقيم يجب أن يعكس المشاعر والمعاني الكامنة في النص."
    }
  },
  {
    "id": 13,
    "q": "كتبت الألف المتطرفة خطأ في كلمة:",
    "options": ["عصا", "رحى", "قفى", "طنطا"],
    "answer": 3,
    "explanations": {
      "correct": "كلمة (طنطا) كُتبت خطأ بالألف لأنها اسم علم أعجمي ينتهي بالتاء المربوطة. الأسماء الأعجمية التي تنتهي بالتاء المربوطة يجب أن تُكتب بالتاء وليس بالألف. الصواب هو كتابتها (طنطاً) أو (طنطة) حسب القواعد الإملائية للأسماء الأعجمية.",
      "wrong1": "كلمة (عصا) كُتبت بشكل صحيح لأنها اسم مقصور ينتهي بألف لينة. الأسماء المقصورة التي تنتهي بألف أصلية تُكتب بالألف الطويلة. هذه الكلمة تخضع للقاعدة الإملائية الخاصة بالأسماء المنتهية بألف مقصورة.",
      "wrong2": "كلمة (رحى) كُتبت بشكل صحيح لأنها اسم منقوص ينتهي بياء. الأسماء المنتهية بياء قبلها كسرة تُكتب بالياء وتُقدّر حركتها. هذه الكلمة تتبع القاعدة الإملائية للأسماء المنتهية بياء مشددة.",
      "wrong3": "كلمة (قفى) كُتبت بشكل صحيح لأنها اسم منقوص ينتهي بألف مقصورة. الأسماء التي تنتهي بألف مقصورة أصلية تُكتب بالألف. هذه الكلمة تخضع للقواعد الإملائية الخاصة بالأسماء المنتهية بألف لينة."
    }
  },
  {
    "id": 14,
    "q": "أراد معلم تصنيف المعلومات والبيانات لاستبانة على 1000 طالب وتحليلها للوصول لنتائج:",
    "options": ["Word", "Visio", "Excel", "Access"],
    "answer": 2,
    "explanations": {
      "correct": "برنامج Excel هو الأنسب لتصنيف المعلومات والبيانات وتحليلها لأنه مصمم خصيصاً للمعالجة الحسابية والإحصائية. يمكنه التعامل مع كميات كبيرة من البيانات وتصنيفها وفرزها وتحليلها إحصائياً. يوفر Excel أدوات متقدمة للتحليل الإحصائي والرسوم البيانية التي تساعد في استخلاص النتائج من البيانات المجمعة.",
      "wrong1": "برنامج Word مصمم primarily لمعالجة النصوص والكتابة وليس لتحليل البيانات. بينما يمكن إنشاء جداول بسيطة في Word، إلا أنه يفتقر للأدوات الإحصائية والتحليلية المتقدمة. لا يناسب معالجة البيانات الرقمية بكميات كبيرة أو إجراء التحليلات الإحصائية المعقدة.",
      "wrong2": "برنامج Visio مصمم لإنشاء المخططات والرسوم البيانية التخطيطية وليس لتحليل البيانات الرقمية. يركز على التمثيل المرئي للعمليات والهياكل التنظيمية أكثر من التحليل الإحصائي. لا يمتلك القدرة على معالجة البيانات الرقمية أو إجراء العمليات الحسابية المعقدة.",
      "wrong3": "برنامج Access مصمم لقواعد البيانات العلاقية وإدارة قواعد البيانات الكبيرة. بينما يمكنه تحليل البيانات، إلا أنه أكثر تعقيداً ويتطلب معرفة متخصصة في قواعد البيانات. Excel أكثر ملاءمة للتحليلات الإحصائية البسيطة إلى المتوسطة والتعامل مع البيانات الرقمية مباشرة."
    }
  },
  {
    "id": 15,
    "q": "يمكن التنبؤ بأن درجات الطالب الذي حصل على درجة ذكاء 110 بأنها:",
    "options": ["تبقى كما هي", "ترتفع بالعمر", "ترتفع بالخبرات المنظمة", "تنخفض بالعمر"],
    "answer": 2,
    "explanations": {
      "correct": "درجات الذكاء يمكن أن ترتفع بالخبرات المنظمة والتدريب والتعلم المستمر لأن الذكاء ليس ثابتاً تماماً. الخبرات التعليمية المنظمة والبيئة المحفزة تساهم في تطوير القدرات العقلية والذكاء. الأبحاث الحديثة تشير إلى أن الذكاء يمكن تطويره من خلال الممارسة المستمرة والتعرض لخبرات تعليمية غنية.",
      "wrong1": "الفكرة أن درجات الذكاء تبقى كما هي تعتمد على النظرة التقليدية للذكاء الثابت. الأبحاث المعاصرة تثبت أن الذكاء قابل للتطور والتغيير مع الخبرات والتعلم. البيئة المحفزة والتدريب المناسب يمكن أن يحسنا من الأداء على اختبارات الذكاء.",
      "wrong2": "الذكاء لا يرتفع تلقائياً مع العمر فقط، بل يحتاج إلى عوامل مساعدة مثل الخبرات التعليمية. التقدم في العمر وحده لا يضمن تحسن الذكاء دون ممارسة وتعلم مستمر. النمو المعرفي مرتبط بالخبرات النوعية وليس فقط بالتقدم العمري.",
      "wrong3": "درجات الذكاء لا تنخفض بالعمر بالضرورة، فالكثير من القدرات العقلية تبقى مستقرة أو حتى تتحسن مع التقدم بالعمر. الانخفاض المعرفي المرتبط بالعمر يؤثر على بعض القدرات وليس كلها، ويمكن التخفيف منه بالتدريب المستمر. الذكاء المتبلور يتحسن مع العمر بينما الذكاء السائل قد يتأثر سلباً."
    }
  },
  {
    "id": 16,
    "q": "طلب معلم من الطلاب تصفح الدرس سريعاً ثم إعادة قراءته بعمق مع تحديد المصطلحات ورسم مخطط:",
    "options": ["المعرفي", "السلوكي", "الاجتماعي", "الشخصي"],
    "answer": 0,
    "explanations": {
      "correct": "هذا النشاط ينتمي للنظرية المعرفية لأنه يركز على عمليات المعالجة الذهنية والتنظيم المعرفي. التصفح السريع ثم القراءة المتعمقة يتوافق مع مبادئ المعالجة العميقة للمعلومات. تحديد المصطلحات ورسم المخططات يساعد في بناء البنى المعرفية وتنظيم المعلومات في الذاكرة.",
      "wrong1": "النظرية السلوكية تركز على المثير والاستجابة والتعزيز وليس على العمليات الذهنية الداخلية. النشاط المذكور لا يتضمن تعزيزاً أو تكراراً آلياً بل عمليات عقلية معقدة. السلوكيون يهتمون بالسلوك الظاهر وليس بالعمليات المعرفية الداخلية.",
      "wrong2": "النظرية الاجتماعية تركز على التعلم من خلال التفاعل مع الآخرين والملاحظة. النشاط الموصوف فردي ولا يتضمن تفاعلاً اجتماعياً أو تعلماً من النماذج. فيجوتسكي وباندورا يؤكدان على أهمية السياق الاجتماعي في التعلم وهو غير موجود هنا.",
      "wrong3": "النظرية الشخصية تركز على الجوانب الوجدانية والدافعية والفردية في التعلم. النشاط المذكور إجرائي معرفي ولا يراعي الفروق الفردية أو الجوانب الشخصية. يعالج العمليات المعرفية العامة وليس الخصائص الشخصية الفردية."
    }
  },
  {
    "id": 17,
    "q": "إذا لاحظت أن ورقتين اختباريتين لهما نفس الأجوبة والطالبان أنكروا الغش، أي إجراء مناسب?",
    "options": ["تعطيهم صفراً", "تطلب إعادة الاختبار", "تصححها وتحولها لإدارة المدرسة", "تحول للجنة الاختبار قبل التصحيح"],
    "answer": 3,
    "explanations": {
      "correct": "تحويل القضية للجنة الاختبار قبل التصحيح هو الإجراء الأنسب لأنه يحافظ على الحيادية ويضمن العدالة. اللجنة تمتلك الصلاحية للتحقيق بشكل موضوعي واتخاذ القرار المناسب. هذا الإجراء يحمي حقوق الطلاب ويضمن تطبيق اللوائح بشكل عادل ومنظم.",
      "wrong1": "إعطاء الصفر مباشرة دون تحقيق يعتبر إجراءً تعسفياً وقد يكون غير عادل. قد يكون هناك تفسيرات منطقية للتشابه في الإجابات دون وجود غش. هذا القرار يتعارض مع مبدأ افتراض البراءة حتى يثبت العكس.",
      "wrong2": "طلب إعادة الاختبار قد يكون غير عملي وقد يعاقب الطلاب الأبرياء إذا كان التشابه صدفة. لا يحقق العدالة الكاملة وقد لا يحل المشكلة الجذرية للغش. يحتاج إلى تخطيط logistically وقد يسبب إرباكاً للطلاب والمدرسة.",
      "wrong3": "تصحيح الأوراق ثم تحويلها للإدارة يتعارض مع مبدأ الوقاية وقد يجعل القرار نهائياً. بمجرد التصحيح قد يصبح من الصعب التراجع عن النتائج أو إثبات حالة الغش. الإدارة قد لا تملك الصلاحية الكاملة للبت في مثل هذه القضايا."
    }
  },
  {
    "id": 18,
    "q": "استراتيجية لماذا? وماذا? وكيف? للعالم:",
    "options": ["هيرمان", "كولب", "ماكافي", "مكارثي"],
    "answer": 1,
    "explanations": {
      "correct": "استراتيجية لماذا وماذا وكيف تعود للعالم كولب وتتعلق بنظريته في أنماط التعلم. هذه الاستراتيجية تمثل دورة التعلم التجريبي التي تشمل التجربة الملموسة والملاحظة reflective والتجريد المفاهيمي والتجريب النشط. كولب يؤكد على أهمية هذه المراحل في عملية التعلم الفعال.",
      "wrong1": "هيرمان معروف بنموذج تفكير الدماغ الكلي وليس باستراتيجية لماذا وماذا وكيف. نموذجه يركز على تفضيلات التفكير في أربعة أرباع دماغية. لا يرتبط مباشرة باستراتيجيات الأسئلة الثلاثية المذكورة.",
      "wrong2": "ماكافي ليس معروفاً بهذه الاستراتيجية بل له إسهامات في مجال تقنية المعلومات والاقتصاد الرقمي. إسهاماته تركز على الجوانب التكنولوجية والاقتصادية أكثر من نظريات التعلم. لا ينسب إليه تطوير استراتيجيات تربوية بهذا الشكل.",
      "wrong3": "مكارثي معروف بنموذج 4Mat System الذي يدمج أنماط التعلم وليس باستراتيجية الأسئلة الثلاثية. نموذجه يركز على كيفية معالجة المعلومات وأنماط التعلم المفضلة. استراتيجيته مختلفة عن استراتيجية لماذا وماذا وكيف الخاصة بكولب."
    }
  },
  {
    "id": 19,
    "q": "من مهارات القراءة الجهرية التي تميزها عن الصامتة:",
    "options": ["الطلاقة", "الضبط السليم", "تحريك الشفتين", "إدراك رسم العبارة"],
    "answer": 1,
    "explanations": {
      "correct": "الضبط السليم للنطق من أهم مهارات القراءة الجهرية التي تميزها عن الصامتة. يتضمن النطق الصحيح للحروف والكلمات مع مراعاة مخارج الحروف وصفاتها. يشمل أيضاً تطبيق قواعد التجويد والوقف والابتداء المناسبة لنوع النص.",
      "wrong1": "الطلاقة مهارة مشتركة بين القراءة الجهرية والصامتة وليست مميزة للجهرية فقط. الطلاقة في القراءة الصامتة تعني سرعة الفهم والاستيعاب. في الجهرية تضيف بعداً صوتياً ولكنها ليست الفارق الأساسي.",
      "wrong2": "تحريك الشفتين ظاهرة غير مرغوب فيها في القراءة الصامتة وليست مهارة في الجهرية. يعتبر تحريك الشفتين أثناء القراءة الصامتة عادة سيئة تبطئ السرعة. ليست من المهارات التي يتم التدريب عليها في القراءة الجهرية.",
      "wrong3": "إدراك رسم العبارة مهارة بصرية مشتركة بين نوعي القراءة وليست حصرية للجهرية. تعتمد على القدرة على تمييز الكلمات والجمل بصرياً وفهم تركيبها. تطور هذه المهارة في كلا النوعين من القراءة."
    }
  },
  {
    "id": 20,
    "q": "عند التخطيط لدرس 'حقوق وواجبات' لموضوع ضعف روابط الصلة بين أبناء الحي، أنسب نشاط للطلاب:",
    "options": ["كتابة مقال عن أسباب ضعف الروابط واقتراح الحلول", "جمع قصص ونوادر عن الجيرة الحسنة", "تنظيم مسابقة 'أحب جاري'", "شرح حديث 'مازال جبريل يوصيني بالجار'"],
    "answer": 0,
    "explanations": {
      "correct": "كتابة مقال عن أسباب ضعف الروابط واقتراح الحلول يناسب موضوع حقوق وواجبات الجوار بشكل مباشر. يشجع الطلاب على التحليل النقدي للمشكلة والتفكير في حلول عملية. ينمي مهارات التفكير العليا والكتابة الإبداعية مع معالجة المشكلة جذرياً.",
      "wrong1": "جمع قصص عن الجيرة الحسنة نشاط جيد لكنه يركز على الجانب العاطفي أكثر من الجانب الحقوقي. لا يتعمق في تحليل الأسباب والحلول للمشكلة المطروحة. يعزز القيم الإيجابية لكنه لا يعالج بشكل مباشر موضوع الحقوق والواجبات.",
      "wrong2": "تنظيم مسابقة 'أحب جاري' يركز على الجانب العاطفي والتنافسي أكثر من الجانب الحقوقي. قد يكون تحفيزياً لكنه لا يضمن الفهم العميق للحقوق والواجبات. يعزز السلوك الإيجابي لكنه لا ينمي الوعي الحقوقي بشكل منهجي.",
      "wrong3": "شرح الحديث الشريف مهم للتربية الإسلامية لكنه لا يشمل الجانب التطبيقي التحليلي. يركز على الجانب النظري والديني دون معالجة المشكلة المجتمعية بشكل عملي. مفيد للقيم لكنه لا ينمي مهارات التحليل واقتراح الحلول."
    }
  },
  {
    "id": 21,
    "q": "إذا أراد المعلم تدريس الطلاب ظاهرة خسوف القمر، فإن أفضل طريقة لدعم تعلم الطلاب هذا الموضوع هي:",
    "options": ["عرض فيديو توضيحي للظاهرة", "عرض لوحة للظاهرة أمام الطلاب", "تلخيص الظاهرة في خطوات على السبورة", "توجيه الطلاب لملاحظة الظاهرة عند حدوثها في الليل"],
    "answer": 0,
    "explanations": {
      "correct": "عرض فيديو توضيحي للظاهرة هو الأفضل لأنه يقدم تمثيلاً مرئياً ديناميكياً يوضح آلية الخسوف خطوة بخطوة. الفيديو يمكنه عرض الحركة الدورانية للأجرام السماوية والظلال بشكل واضح ومشوق للطلاب. الوسائط المتعددة تجعل المفاهيم الفلكية المجردة ملموسة ومفهومة، خاصة للظواهر التي تحدث في أوقات متأخرة يصعب على الطلاب ملاحظتها مباشرة.",
      "wrong1": "عرض لوحة للظاهرة يوفر تمثيلاً ثابتاً لا يوضح الحركة والديناميكية التي تتميز بها الظواهر الفلكية. اللوحات الثابتة لا تستطيع إظهار التغيرات الزمنية والحركات النسبية بين الأرض والقمر والشمس. قد توفر فكرة عامة لكنها لا تعطي الفهم الكامل للعملية المتكاملة للخسوف.",
      "wrong2": "التلخيص على السبورة يعتمد على الشرح النظري المجرد الذي قد لا يصل للطلاب بالوضوح المطلوب. الظواهر الفلكية تحتاج لتمثيل بصري واضح أكثر من الاعتماد على الشرح اللفظي فقط. الطلاب قد يواجهون صعوبة في تصور الحركات السماوية المعقدة من خلال الخطوات المكتوبة فقط.",
      "wrong3": "توجيه الطلاب للملاحظة المباشرة غير عملي لأن الخسوف يحدث في أوقات متأخرة وغير منتظمة وقد لا يناسب جميع الطلاب. الاعتماد على الملاحظة المباشرة فقط يحرم الطلاب من فهم الآلية العلمية الكامنة وراء الظاهرة. قد تكون الظروف الجوية غير مناسبة للملاحظة أو قد يحدث الخسوف في توقيت غير مناسب للطلاب."
    }
  },
  {
    "id": 22,
    "q": "يؤدي المعلم دورًا في تنمية المجتمع المحلي، أي مما يلي ليس في هذا المجال?",
    "options": ["المساعدة في برامج محو الأمية", "نشر الثقافة العلمية", "تنمية الوعي البيئي", "بناء المفاهيم العلمية"],
    "answer": 3,
    "explanations": {
      "correct": "بناء المفاهيم العلمية يعد من صميم العملية التعليمية داخل الصف الدراسي وليس من أدوار المعلم في تنمية المجتمع المحلي مباشرة. هذا النشاط يركز على تحقيق الأهداف التعليمية للمناهج داخل المؤسسة التعليمية. يعتبر من المهام الأساسية للمعلم في التدريس وليس من الأنشطة المجتمعية الخارجية.",
      "wrong1": "المساعدة في برامج محو الأمية تمثل دوراً مجتمعياً واضحاً للمعلم خارج نطاق المدرسة. يساهم المعلم من خلالها في رفع مستوى المجتمع التعليمي والثقافي. يعتبر من أشكال المشاركة المجتمعية الفعالة التي تنعكس إيجاباً على المجتمع المحلي.",
      "wrong2": "نشر الثقافة العلمية من الأدوار المجتمعية المهمة التي يمكن للمعلم القيام بها عبر المحاضرات والندوات المجتمعية. يساعد في رفع الوعي العلمي لدى أفراد المجتمع وتعزيز التفكير العلمي. يعتبر امتداداً لدور المعلم التربوي إلى نطاق أوسع في المجتمع.",
      "wrong3": "تنمية الوعي البيئي يمكن أن يتم من خلال أنشطة مجتمعية مثل حملات النظافة والتشجير والتوعية البيئية. يشكل جزءاً من مسؤولية المعلم تجاه قضايا المجتمع البيئية. يعكس دور المعلم في المساهمة في حل المشكلات المجتمعية الملموسة."
    }
  },
  {
    "id": 23,
    "q": "قال المتنبي:...............يملأُ الْأَفْعَالَ رَأَيَا وَحِكمَةً ونادرة أحيان.................. وَيَغضَبُ الكلمتان اللتان تكملان البيت الشعري السابق",
    "options": ["فتا، يرضا", "فتا، يرضى", "فتى، يرضا", "فتى يرضى"],
    "answer": 3,
    "explanations": {
      "correct": "الكلمتان الصحيحتان هما (فتى، يرضى) لأن البيت الشعري يحتاج لكلمة (فتى) بالياء المنقوطة للمثنى المنصوب، و(يرضى) بالياء المنقوطة لأنها فعل مضارع معتل الآخر. الإعراب الصحيح يتطلب هذه الصيغ وفق قواعد اللغة العربية والإعراب. هاتان الكلمتان تتناسبان مع وزن البيت الشعري وقافيته.",
      "wrong1": "كلمة (فتا) غير صحيحة لأن المثنى المنصوب ينتهي بياء مشددة في حالة النصب. الصواب هو (فتى) بالياء المنقوطة وفق قواعد إعراب المثنى. هذه الصيغة تخالف القواعد النحوية المعتمدة في اللغة العربية الفصحى.",
      "wrong2": "تركيب (فتا، يرضى) خاطئ لأن الجزء الأول (فتا) غير صحيح إملائياً ونحوياً. المثنى المنصوب يجب أن ينتهي بياء مشددة مفتوحة ما قبلها. هذا الخيار يجمع بين صيغة خاطئة وأخرى صحيحة مما يجعله غير متجانس.",
      "wrong3": "كلمة (يرضا) غير صحيحة لأن الفعل المضارع المعتل الآخر بالألف يرفع بضمة مقدرة وينصب ويجزم بحذف الألف. الصواب هو (يرضى) بالياء عند الرفع والنصب والجزم. هذه الصيغة تخالف القواعد الصرفية للأفعال المعتلة."
    }
  },
  {
    "id": 24,
    "q": "كل مما يلي من خصائص الكتابة الوظيفية ما عدا:",
    "options": ["سهولة العبارة", "الاستشهاد بالحقائق", "الاعتماد على الخيال", "اختفاء شخصية الكاتب"],
    "answer": 2,
    "explanations": {
      "correct": "الاعتماد على الخيال ليس من خصائص الكتابة الوظيفية لأنها تعتمد على الحقائق والمعلومات الدقيقة والموضوعية. الكتابة الوظيفية تهدف لإيصال معلومات محددة واضحة دون إضافات أدبية أو تخيلية. تعتمد على المنطق والواقعية والموضوعية في عرض الأفكار والمعلومات.",
      "wrong1": "سهولة العبارة من خصائص الكتابة الوظيفية لأنها تهدف للوضوح والإيضاح وعدم التعقيد. تستخدم لغة مباشرة وبسيطة تصل للقارئ دون غموض أو التباس. تبتعد عن التعقيد اللفظي والتركيبي لتؤدي وظيفتها بشكل فعال.",
      "wrong2": "الاستشهاد بالحقائق من أساسيات الكتابة الوظيفية لأنها تعتمد على المعلومات الموثوقة والدقيقة. تقدم أدلة وبراهين واقعية تدعم الأفكار المطروحة. تعتمد على المصادر الموثوقة والبيانات الملموسة في بناء المحتوى.",
      "wrong3": "اختفاء شخصية الكاتب من سمات الكتابة الوظيفية لأنها تركز على الموضوع وليس على مشاعر الكاتب أو آرائه الشخصية. تقدم المعلومات بشكل محايد وموضوعي بعيداً عن الانحياز الشخصي. تهدف للحيادية والموضوعية في معالجة القضايا المطروحة."
    }
  },
  {
    "id": 25,
    "q": "تنمية مهارات الطالب في إدارة الوقت تتم من خلال:",
    "options": ["تدريبه على وضع خطة زمنية لتنفيذ الأنشطة", "إكسابه المهارات المعرفية المتعلقة بأهمية الوقت", "مساعدته على إنهاء النشاط في الوقت المحدد", "منحه الحرية في تحديد الوقت لتنفيذ الأنشطة"],
    "answer": 0,
    "explanations": {
      "correct": "تدريبه على وضع خطة زمنية لتنفيذ الأنشطة هو الأسلوب الأمثل لأنه ينمي مهارة التخطيط والتنظيم الذاتي. يتعلم الطالب من خلاله تحديد الأولويات وتوزيع الوقت بشكل متوازن بين المهام المختلفة. يساعد في تطوير الوعي الزمني والقدرة على إدارة الموارد الزمنية بشكل فعال.",
      "wrong1": "إكساب المهارات المعرفية حول أهمية الوقت ضروري لكنه لا يكفي دون تطبيق عملي. المعرفة النظرية وحدها لا تنمي المهارات العملية في إدارة الوقت. يحتاج الطالب للتطبيق العملي لتحويل المعرفة إلى سلوك فعلي.",
      "wrong2": "مساعدته على إنهاء النشاط في الوقت المحدد يركز على النتيجة النهائية وليس على عملية التعلم. لا ينمي مهارات التخطيط والتنظيم الذاتي لدى الطالب. يجعل الطالب зависиاً على المساعدة الخارجية بدلاً من تطوير استقلاليته.",
      "wrong3": "منح الحرية الكاملة في تحديد الوقت دون توجيه قد يؤدي إلى الفوضى وعدم التنظيم. الطالب يحتاج للإرشاد والتدرج في تحمل مسؤولية إدارة وقته. الحرية المطلقة دون تأهيل مسبق قد تعيق تطوير مهارات الإدارة الفعالة للوقت."
    }
  },
  {
    "id": 26,
    "q": "قام أحد الطلاب بالاستهزاء بإجابة أحد زملائه فالإجراء الأنسب تربويا الذي يفترض أن يمارسه المعلم :",
    "options": ["تأديبه أمام زملائه", "تحويل السؤال اليه مباشرة", "إيقافه وطلب الاعتذار منه لزميله فورا", "استدعاؤه على انفراد بعد الحصة وتوضيح خطأه"],
    "answer": 3,
    "explanations": {
      "correct": "استدعاء الطالب على انفراد بعد الحصة وتوضيح خطأه هو الإجراء التربوي الأمثل لأنه يحافظ على كرامة الطالب. يتيح فرصة للحوار الهادئ والتفاهم بعيداً عن ضغط الجمهور. يمكن المعلم من شرح الآثار السلبية للاستهزاء وتنمية مشاعر التعاطف والاحترام المتبادل.",
      "wrong1": "تأديب الطالب أمام زملائه يسبب الإحراج والعدوانية وقد يزيد المشكلة بدلاً من حلها. يتعارض مع مبادئ التربية الإيجابية التي تحترم كرامة المتعلم. قد يؤدي إلى فقدان ثقة الطالب بنفسه وبالمعلم وبالمدرسة.",
      "wrong2": "تحويل السؤال إليه مباشرة قد يزيد الموقف توتراً ويشعره بالهجوم أمام الآخرين. لا يعالج المشكلة الجذرية للسلوك غير اللائق. قد يدفع الطالب للدفاع عن نفسه بطريقة سلبية تزيد من تعقيد الموقف.",
      "wrong3": "إيقافه وطلب الاعتذار فوراً يجبره على اعتذار غير صادق وقد لا يفهم الخطأ الحقيقي. الاعتذار تحت الضغط لا يحقق الغرض التربوي المنشود. لا يعطي فرصة للتفكير والاستبصار وتعديل السلوك بشكل حقيقي."
    }
  },
  {
    "id": 27,
    "q": "المدرسة قدمت اختباراً موحداً، تفاوت تقدير المعلمين يدل على افتقار الاختبار إلى:",
    "options": ["الصدق", "الثبات", "الشمولية", "الموضوعية"],
    "answer": 1,
    "explanations": {
      "correct": "تفاوت التقدير بين المعلمين يدل على افتقار الاختبار للثبات لأنه يقيس عدم الاتساق في النتائج. الثبات يعني أن الاختبار يعطي نتائج متقاربة عند تطبيقه مرات متعددة أو من قبل مصححين مختلفين. عدم الثبات يشير إلى وجود عوامل عشوائية تؤثر على الدرجات وتقلل من مصداقية الاختبار.",
      "wrong1": "الصدق يعني قياس الاختبار لما صمم لقياسه وليس له علاقة مباشرة بتفاوت التقدير. يمكن أن يكون الاختبار صادقاً لكن غير ثابت إذا كانت نتائجه غير متسقة. الصدق يتعلق بمدى تمثيل الاختبار للمحتوى والمهارات المستهدفة.",
      "wrong2": "الشمولية تعني تغطية الاختبار لجميع أجزاء المحتوى التعليمي المطلوب. لا ترتبط مباشرة بمسألة تفاوت التقدير بين المصححين. الاختبار الشامل قد يكون ثابتاً أو غير ثابت اعتماداً على عوامل أخرى.",
      "wrong3": "الموضوعية تعني خلو الاختبار من التأثر بالآراء الشخصية للمصحح. تفاوت التقدير يدل على عدم الموضوعية لكن السبب الجذري هو عدم الثبات. الموضوعية نتيجة للثبات وليس العكس، فالاختبار الثابت يكون موضوعياً بالضرورة."
    }
  },
  {
    "id": 28,
    "q": "قبل البدء بتنفيذ المشروعات البحثية ، تزود المعلمة أمنه طالباتها بسلم تقدير يوضح مستويات الأداء المختلفة وما يقابلها من درجات (معايير التصحيح) ويتوقع لهذه الممارسة أن تؤدي إلى :",
    "options": ["ارتفاع نسبة جودة المشروعات ودرجة تقديمها بالمعايير الموضوعه", "زيادة مقدار الوقت اللازم لإنجاز مشروعات تستجيب للمعايير", "انخفاض مصداقية التصحيح بسبب المعرفة المسبقة بالمعايير", "شعور الطالبات بالاحباط نتيجة ارتفاع مستوى معايير التصحيح"],
    "answer": 0,
    "explanations": {
      "correct": "تزويد الطالبات بسلم التقدير مسبقاً يرفع جودة المشروعات لأنهن يعرفن التوقعات والمعايير بوضوح. يساعد في توجيه الجهود نحو المستويات المطلوبة وتحسين الأداء. يعزز الشفافية والعدالة في التقييم ويساعد الطالبات على التخطيط الفعال لعملهم.",
      "wrong1": "زيادة الوقت اللازم قد تحدث لكنها ليست النتيجة الأساسية المتوقعة من هذه الممارسة. الوقت الإضافي يستثمر في تحسين الجودة وتحقيق المعايير المطلوبة. لا يعتبر زيادة الوقت نتيجة سلبية بل استثمار في التعلم الجيد.",
      "wrong2": "المعرفة المسبقة بالمعايير تزيد مصداقية التصحيح وليس العكس لأنها تضمن الشفافية. الطالبات يعلمن مسبقاً كيف سيتم تقييمهن مما يزيد ثقتهن في العدالة. المصداقية تتعزز عندما تكون معايير التقييم واضحة ومعلنة للجميع.",
      "wrong3": "الشعور بالإحباط غير متوقع إذا كانت المعايير واقعية ومناسبة لمستوى الطالبات. الوضوح المسبق يقلل القلق ويزيد الدافعية للوصول للمستويات المطلوبة. الإحباط يحدث عندما تكون التوقعات غير واضحة وليس عندما تكون محددة ومعروفة."
    }
  },
  {
    "id": 29,
    "q": "من السمات الشخصية لجذب انتباه المستمعين:",
    "options": ["المحافظة على وتيرة صوت واحدة", "التواصل البصري مع المستمعين", "محاولة الخروج عن الموضوع", "استخدام الكلمات الغريبة"],
    "answer": 1,
    "explanations": {
      "correct": "التواصل البصري مع المستمعين من أهم السمات الشخصية لجذب الانتباه لأنه يخلق تفاعلاً مباشراً ويشعر المستمعين بأهميتهم. يعزز الثقة بين المتحدث والجمهور ويساعد في قراءة ردود أفعالهم. يمنح المتحدث فرصة لملاحظة مستوى اهتمام المستمعين وتعديل أسلوبه accordingly.",
      "wrong1": "المحافظة على وتيرة صوت واحدة تسبب الملل وتفقد العرض حيويته وتأثيره. تنوع نبرة الصوت وسرعته ودرجته يساعد في جذب الانتباه وتوضيح الأفكار. الصوت الرتيب يفقد الجمهور اهتمامه ولا يبرز النقاط المهمة في العرض.",
      "wrong2": "الخروج عن الموضوع يشوش الجمهور ويضعف الرسالة الرئيسية ويقلل من مصداقية المتحدث. الالتزام بالموضوع مع التنوع في العرض هو الأسلوب الأمثل لجذب الانتباه. الخروج عن الموضوع قد يظهر المتحدث كمتهور وغير منظم.",
      "wrong3": "استخدام الكلمات الغريبة يصعب الفهم على الجمهور وقد يسبب الإحباط والانفصال عن الموضوع. اللغة الواضحة البسيطة أكثر فعالية في إيصال الرسالة وجذب الانتباه. الكلمات المعقدة قد تظهر المتحدث كمتباهٍ ولكنها تفقد الجمهور اهتمامه."
    }
  },
  {
    "id": 30,
    "q": "في إحدى حلقات النقاش مع معلمي تخصصك في المدرسة ، أدرتم جلسة للعصف الذهني وذلك لاقتراح أسلوب يدعم تحقيق الطلاب للتوقعات العالية منهم ، كل مما يأتي يستخدم لإيصال الطلاب لتحقيق ذلك عدا:",
    "options": ["مقارنة الأداء مع الأقران", "استخدام تكليفات متنوعة", "تقديم التغذية الراجعة", "التعرف على اوجه التميز لدى الطلاب"],
    "answer": 0,
    "explanations": {
      "correct": "مقارنة الأداء مع الأقران لا تدعم تحقيق التوقعات العالية بل قد تسبب الإحباط والمنافسة السلبية. التركيز على المقارنة الخارجية يضعف الدافعية الذاتية ويعزز الشعور بعدم الكفاءة. بدلاً من ذلك، يجب التركيز على التقدم الشخصي لكل طالب مقارنة بأدائه السابق.",
      "wrong1": "استخدام تكليفات متنوعة يدعم تحقيق التوقعات العالية من خلال تلبية احتياجات التعلم المختلفة. يساعد الطلاب على إظهار قدراتهم بطرق متعددة تناسب أنماط تعلمهم. التنوع في التكليفات يشجع الإبداع والتفكير العميق ويحفز الاهتمام.",
      "wrong2": "تقديم التغذية الراجعة البناءة أساسي لتحقيق التوقعات العالية لأنه يوجه الطلاب نحو التحسين. يساعدهم على فهم نقاط القوة والضعف وكيفية التطوير. التغذية الراجعة الفورية والمحددة تزيد من دافعية الطلاب للوصول لأعلى المستويات.",
      "wrong3": "التعرف على أوجه التميز لدى الطلاب يساعد في بناء الثقة وتوجيهها نحو تحقيق التوقعات العالية. يمكن المعلم من تصميم experiences تعليمية تنمي نقاط القوة الفردية. يعزز الشعور بالكفاءة والقدرة على الإنجاز المتميز."
    }
  },
  {
    "id": 31,
    "q": "أي عمليات التعلم ذو المعنى يستهدفها المعلم عند طلب تحديد نقاط التشابه والاختلاف?",
    "options": ["الدعم والتسكيل", "التوفيق التكاملي", "التمايز التقدمي", "التنظيم المتسلسل"],
    "answer": 1,
    "explanations": {
      "correct": "التوفيق التكاملي هو العملية التي يستهدفها المعلم عند طلب تحديد نقاط التشابه والاختلاف لأنها تركز على ربط المفاهيم الجديدة بالمعرفة السابقة. تساعد هذه العملية في بناء شبكات معرفية مترابطة تمكن الطالب من فهم العلاقات بين المفاهيم المختلفة. تعزز التعلم ذو المعنى من خلال إيجاد روابط منطقية بين الأفكار وتنظيمها في إطار متماسك.",
      "wrong1": "الدعم والتسكيل يهدف إلى تقديم المساعدة المؤقتة للطالب أثناء التعلم ولكن لا يركز تحديداً على عمليات المقارنة والتمييز. يعتبر أسلوباً لدعم التعلم وليس عملية معرفية مباشرة للمقارنة. يركز على التدرج في سحب الدعم وليس على تحليل أوجه التشابه والاختلاف.",
      "wrong2": "التمايز التقدمي يركز على تكييف التعليم ليلائم الفروق الفردية بين الطلاب وليس على عمليات المقارنة المعرفية. يعتبر استراتيجية تدريسية وليس عملية تعلم معرفية داخلية. يهتم بتقديم محتوى تعليمي متنوع وليس بتحليل العلاقات بين المفاهيم.",
      "wrong3": "التنظيم المتسلسل يهتم بترتيب المحتوى التعليمي بشكل منطقي متدرج وليس بعمليات المقارنة والتمييز. يعتبر مبدأ من مبادئ تنظيم المناهج وليس عملية معرفية للمقارنة. يركز على التسلسل الهرمي للمفاهيم وليس على تحليل أوجه التشابه والاختلاف بينها."
    }
  },
  {
    "id": 32,
    "q": "كلمة 'غير أن' تدل على:",
    "options": ["الاستدراك", "الاستثناء", "التذكير", "التعليل"],
    "answer": 0,
    "explanations": {
      "correct": "كلمة 'غير أن' تدل على الاستدراك لأنها تستخدم للربط بين جملتين حيث تنسخ الثانية معنى الأولى أو تقيده. تعمل على تصحيح فكرة سابقة أو توضيحها بإضافة معلومات جديدة تخالف المتوقع. تساعد في إضفاء الدقة على المعنى وتوضيح العلاقة المنطقية بين الأفكار المتعاقبة.",
      "wrong1": "الاستثناء يختلف عن الاستدراك لأنه يعني إخراج ما بعد أداة الاستثناء من حكم ما قبلها. أدوات الاستثناء مثل 'إلا' و'غير' و'سوى' تختلف في دلالتها عن 'غير أن'. الاستثناء يتعلق بالإخراج من العموم وليس بتصحيح الأفكار أو تقييدها.",
      "wrong2": "التذكير يعني توجيه الانتباه إلى معلومة سابقة معروفة وليس له علاقة بالاستدراك. أدوات التذكير مثل 'ألا تذكر' و'تذكّر أن' تختلف عن 'غير أن' في الوظيفة والدلالة. التذكير يركز على استحضار المعلومات السابقة وليس على تصحيحها أو تقييدها.",
      "wrong3": "التعليل يهدف إلى بيان السبب والعلة وليس إلى الاستدراك أو التصحيح. أدوات التعليل مثل 'لأن' و'بسبب' و'نظراً ل' تختلف عن 'غير أن' في الدلالة والوظيفة. التعليل يوضح الأسباب بينما الاستدراك يصحح الأفكار أو يقيدها."
    }
  },
  {
    "id": 33,
    "q": "أحمد وبدر سئلا عن اللغة العربية، فأجاب أحمد هي أكثر اللغات من حيث المفردات وأجاب بدر: هي أكثر اللغات انتشارا في العالم ...",
    "options": ["كلاهما محايدان", "كلاهما متحيزان", "أحمد محايد، بدر : متحيز", "أحمد متحيز ، بدر محايد"],
    "answer": 3,
    "explanations": {
      "correct": "أحمد متحيز لأنه قدم حقيقة غير دقيقة (اللغة العربية ليست الأكثر من حيث المفردات بشكل قاطع) بينما بدر محايد لأنه قدم حقيقة قابلة للتحقق إحصائياً. تحيز أحمد نابع من تقديم رأي شخصي على أنه حقيقة مطلقة دون أدلة كافية. إجابة بدر تعتمد على بيانات واقعية يمكن التحقق منها حول انتشار اللغات في العالم.",
      "wrong1": "ليس كلاهما محايدان لأن أحمد قدم إجابة تعكس تحيزاً واضحاً دون أساس علمي مؤكد. المحايدة تتطلب الموضوعية والاعتماد على الحقائق الثابتة وليس الآراء الشخصية. إجابة أحمد تفتقر إلى الدقة العلمية المطلوبة في التقييم المحايد.",
      "wrong2": "ليس كلاهما متحيزان لأن إجابة بدر تعتمد على معطيات إحصائية يمكن التحقق منها موضوعياً. التحيز يعني تبني موقف مسبق دون اعتبار للحقائق الموضوعية. بدر قدم معلومة قابلة للقياس والتحقق بشكل موضوعي.",
      "wrong3": "العكس غير صحيح لأن أحمد هو المتحيز وليس المحايد، بينما بدر هو المحايد وليس المتحيز. تقييم انتشار اللغات يعتمد على إحصائيات موضوعية بينما تعداد المفردات مسألة أكثر تعقيداً. دقة المعلومات وقابليتها للتحقق هي المعيار في التمييز بين المحايدة والتحيز."
    }
  },
  {
  "id": 34,
  "q": "قال الوالد لابنه ___ ما أجملك ___ ما علامات الترقيم المناسبة؟",
  "options": ["، -", "، - ؟", ": - .", ": - !"],
  "answer": 3,
  "explanations": {
    "correct": "الاختيار الصحيح هو (: - !) لأن النقطتين الرأسيتين (:) تأتيان بعد فعل القول للدلالة على بداية كلام مباشر، بينما علامة التعجب (!) تُستخدم في نهاية الجملة لأنها تعبر عن الانفعال والإعجاب في عبارة (ما أجملك).",
    "wrong1": "الفاصلة (،) بعد فعل القول غير مناسبة لأنها لا تُستخدم لبداية الكلام المباشر، كما أن الشرطة أو النقطة لا تعبر عن الانفعال المناسب للجملة.",
    "wrong2": "وضع الفاصلة (،) بعد قول الوالد خطأ نحوي، كما أن علامة الاستفهام (؟) في النهاية لا تناسب الجملة لأنها تعجبية وليست سؤالاً.",
    "wrong3": "النقطتان الرأسيتان صحيحتان بعد فعل القول، لكن استخدام النقطة (.) في نهاية الجملة لا يعبر عن الانفعال أو الإعجاب الموجود في الجملة، لذا فهي غير مناسبة."
}
  },
  {
    "id": 35,
    "q": "كل الكلمات مترادفة ما عدا:",
    "options": ["شامخ وحافل", "سامق وعالي", "روابط ووشائج", "شظف وضيق"],
    "answer": 3,
    "explanations": {
      "correct": "كلمتي 'شظف وضيق' ليستا مترادفتين لأن 'شظف' تعني الشدة والقسوة في العيش بينما 'ضيق' تعني عدم السعة. العلاقة بينهما علاقة تضاد وليس ترادف. الشظف يدل على قسوة الظروف بينما الضيق يدل على عدم الاتساع المكاني أو المعنوي.",
      "wrong1": "كلمتي 'شامخ وحافل' مترادفتان لأن كلتيهما تدل على العلو والارتفاع والامتلاء. الشامخ يعني المرتفع العالي، والحافل يعني الممتلئ والغزير. الترادف بينهما واضح في الدلالة على العظمة والامتلاء.",
      "wrong2": "كلمتي 'سامق وعالي' مترادفتان لأن كلتيهما تدل على الارتفاع والعلو. السامق يعني الشاهق المرتفع، والعالي يعني ما ارتفع عن المستوى. الترادف بينهما قوي في الإشارة إلى معنى الارتفاع والعلو.",
      "wrong3": "كلمتي 'روابط ووشائج' مترادفتان لأن كلتيهما تدل على العلاقات والصلات. الروابط تعني الصلات والعلاقات، والوشائج تعني الأواصر والصلات. الترادف بينهما واضح في الدلالة على العلاقات والصلات."
    }
  },
  {
  "id": 36,
  "q": "يستخدم المتعلم أسلوب حل المشكلات للوصول إلى هدف معين، عندما يكون ذلك الهدف غير متاح أمامه. الضمير (الهاء) في كلمة 'أمامه' يعود على:",
  "options": ["الهدف", "المتعلم", "الوصول", "متاح"],
  "answer": 1,
  "explanations": {
    "correct": "الضمير (الهاء) في 'أمامه' يعود على المتعلم؛ لأن كلمة 'أمام' تُستخدم للدلالة على موقع شيء بالنسبة لشخص، لا بالنسبة لشيء آخر. فلا نقول: 'الهدف غير متاح أمام الهدف' أو 'أمام الوصول'. المعنى المقصود هو أن الهدف غير متاح أمام المتعلم، أي لا يراه أو لا يستطيع الوصول إليه مباشرة. لذلك فالضمير يعود على المتعلم، وهو المرجع الأنسب لغوياً وسياقياً.",
    "wrong1": "لا يصح أن يعود الضمير على 'الهدف'؛ لأن تركيب 'الهدف غير متاح أمام الهدف' غير منطقي لغوياً. كما أن كلمة 'أمام' لا تُستخدم عادة مع الأشياء الجامدة كمرجع للضمير، بل مع الأشخاص.",
    "wrong2": "الوصول عملية وليس شيئاً مادياً يمكن أن يكون أمام شخص أو شيء، وبالتالي لا يمكن للضمير أن يعود عليه في هذا السياق.",
    "wrong3": "'متاح' صفة وليس اسماً، ولا يصح أن يعود عليه الضمير. كما أنه تابع للهدف، ولا يُشكل مرجعاً للضمير في الجملة."
    }
  },
  {
    "id": 37,
    "q": "جميع الكلمات مصادر عدا:",
    "options": ["وقوف", "ابتهال", "تناصح", "استثار"],
    "answer": 3,
    "explanations": {
      "correct": "كلمة 'استثار' ليست مصدراً بل هي فعل ماض من الفعل يستثير. المصدر من هذا الفعل هو 'استثارة' على وزن استفعال. لا يمكن اعتبار 'استثار' مصدراً لأنه يحمل زمن الماضي وليس الحدث المجرد.",
      "wrong1": "كلمة 'وقوف' مصدر من الفعل وقف يقف على وزن فعول. تمثل الحدث المجرد للوقوف دون زمن محدد. تتبع القواعد الصرفية للمصادر في اللغة العربية.",
      "wrong2": "كلمة 'ابتهال' مصدر من الفعل ابتهل يبتهل على وزن افتعال. تدل على الحدث المجرد للابتهال والدعاء. تعتبر مصدراً قياسياً وفق أوزان المصادر في العربية.",
      "wrong3": "كلمة 'تناصح' مصدر من الفعل تناصح يتناصح على وزن تفاعل. تمثل الحدث المشترك للتناصح بين الطرفين. تتبع القواعد الصرفية للمصادر المتفعلة في اللغة."
    }
  },
  {
    "id": 38,
    "q": "الفعل يقارن ينتمي إلى:",
    "options": ["التحليل", "التطبيق", "التقويم", "التركيب"],
    "answer": 0,
    "explanations": {
      "correct": "الفعل 'يقارن' ينتمي إلى مستوى التحليل في تصنيف بلوم لأنه يتضمن تفكيك المعلومات إلى أجزاء وإيجاد العلاقات بينها. المقارنة تتطلب تحليل العناصر وفحص أوجه التشابه والاختلاف. تعتبر من المهارات التحليلية العليا التي تتطلب فهماً عميقاً للعلاقات.",
      "wrong1": "التطبيق يعني استخدام المعرفة في مواقف جديدة وليس المقارنة بين العناصر. يتضمن تنفيذ وإجراء عمليات محددة وليس تحليل العلاقات. يركز على الاستخدام العملي للمعرفة وليس على التحليل المقارن.",
      "wrong2": "التقويم يعني إصدار أحكام قيمية بناء على معايير محددة وليس مجرد المقارنة. يتطلب حكماً على الجودة والقيمة وليس فقط المقارنة الوصفية. يعتبر مستوى أعلى من التحليل في تصنيف بلوم.",
      "wrong3": "التركيب يعني تجميع الأجزاء لتكوين كل جديد ومبتكر وليس المقارنة بين عناصر موجودة. يتضمن الإبداع وتوليد أفكار جديدة وليس تحليل العلاقات بين العناصر. يعتبر مستوى إبداعياً يتجاوز التحليل والمقارنة."
    }
  },
  {
    "id": 39,
    "q": "أراد معلم إثارة التفكير بحيث يتعرف الطلاب على المفهوم ثم الأمثلة، الأسلوب التدريسي:",
    "options": ["الحوارية", "القياسية", "الاكتشاف", "حل المشكلات"],
    "answer": 2,
    "explanations": {
      "correct": "أسلوب الاكتشاف يناسب هذا الهدف لأنه يبدأ بالمفاهيم العامة ثم يتجه نحو الأمثلة والتطبيقات. يشجع الطلاب على التفكير النشط واستخلاص المعرفة بأنفسهم. ينمي مهارات الاستقصاء والبحث والتفكير العلمي المنظم.",
      "wrong1": "الأسلوب الحواري يركز على تبادل الآراء والأفكار بين المعلم والطلاب وليس بالضرورة على التسلسل من المفهوم إلى الأمثلة. يعتمد على النقاش والتفاعل اللفظي أكثر من التركيز على البنية المفاهيمية. قد لا يضمن الانتظام المنطقي في تقديم المفاهيم ثم الأمثلة.",
      "wrong2": "الأسلوب القياسي يعتمد على الانتقال من الأمثلة إلى القواعد وليس العكس كما في السؤال. يبدأ بالتطبيقات والأمثلة ثم يستنتج منها المفاهيم العامة. يعاكس التسلسل المطلوب في السؤال الذي يبدأ بالمفاهيم ثم الأمثلة.",
      "wrong3": "أسلوب حل المشكلات يركز على معالجة موقف problematic محدد وليس على الانتقال من المفاهيم إلى الأمثلة. يبدأ بمشكلة محددة ثم يبحث عن حلها باستخدام المعرفة. لا يتوافق مع التسلسل المطلوب من العام إلى الخاص."
    }
  },
  {
    "id": 40,
    "q": "إذا أراد المعلم تقويم امتلاك الطلاب لمهارات التلاوة والتجويد في القرآن الكريم، الأداة الأكثر دقة هي:",
    "options": ["سلم التقدير", "الاختبار الكتابي", "السجل القصصي", "سجل وصف التعلم للطالب"],
    "answer": 3,
    "explanations": {
      "correct": "سجل وصف التعلم للطالب هو الأداة الأكثر دقة لأنه يوثق تطور المهارات الأدائية عبر الوقت. يسجل ملاحظات مفصلة عن مستوى إتقان التلاوة والتجويد بشكل تراكمي. يمكنه توثيق الجوانب المختلفة للأداء الصوتي والنطق والالتزام بقواعد التجويد.",
      "wrong1": "سلم التقدير مفيد لكنه قد لا يلتقط الدقة الكاملة في مهارات التلاوة والتجويد. يعطي تقديرات عامة ولكن قد يفقد التفاصيل الدقيقة في الأداء. لا يوفر التغذية الراجعة التفصيلية التي يحتاجها تطوير مهارات التلاوة.",
      "wrong2": "الاختبار الكتابي غير مناسب لتقويم المهارات الأدائية مثل التلاوة والتجويد. لا يمكنه قياس الجوانب العملية للأداء الصوتي والنطق السليم. يركز على المعرفة النظرية وليس على التطبيق العملي للمهارات.",
      "wrong3": "السجل القصصي يركز على وصف المواقف والسلوكيات وليس على تقويم المهارات الأدائية الدقيقة. قد يكون مفيداً للجوانب السلوكية ولكن ليس لمهارات محددة مثل التجويد. لا يقدم تقييماً منهجياً لمستويات إتقان المهارات."
    }
  },
  {
    "id": 41,
    "q": "لكي يحافظ المعلم على مستوى مرتفع من الدافعية لدى الطلاب الذين يتعرضون لبعض خبرات الإخفاق ، وبالإستناد إلى النظريات المعرفية في الدافعية يفترض أن يقوم بعمل :",
    "options": ["عزو الفشل إلى الجهد المبذول", "تعزيز أي تقدم يحققه الطالب", "توفير بيئة صفية آمنة خالية من النقد", "تشجيع الطالب على تكرار المحاولات"],
    "answer": 0,
    "explanations": {
      "correct": "عزو الفشل إلى الجهد المبذول هو الأسلوب الأمثل وفق النظريات المعرفية لأنه يشجع الطالب على تحمل المسؤولية وإدراك أن النجاح مرتبط بالجهد. هذا النهج ينمي لدى الطالب الإحساس بالسيطرة على نتائج تعلمه وقدرته على التحسن من خلال بذل المزيد من الجهد. يعزز هذا الأسلوب الدافعية الداخلية ويقلل من الشعور بالعجز المكتسب لدى الطلاب.",
      "wrong1": "تعزيز أي تقدم يحققه الطالب مهم لكنه لا يعالج الجذور المعرفية للدافعية وفق النظريات المعرفية. التعزيز وحده لا يساعد الطالب على فهم أسباب الإخفاق وكيفية تجاوزه. يركز على المكافأة الخارجية أكثر من بناء المفاهيم المعرفية الصحيحة حول التعلم.",
      "wrong2": "توفير بيئة صفية آمنة ضروري لكنه لا يكفي لمعالجة قضايا الدافعية المتعلقة بالإخفاق. البيئة الآمنة تمثل شرطاً أساسياً لكنها لا تعلم الطالب كيفية تفسير الفشل والتعامل معه. لا تساعد الطالب على تطوير استراتيجيات المواجهة المعرفية المناسبة.",
      "wrong3": "تشجيع الطالب على تكرار المحاولات مفيد لكنه يظل سطحياً إذا لم يرافقه فهم للأسباب الحقيقية للإخفاق. التكرار دون فهم قد يؤدي إلى الإحباط إذا لم يصاحبه توجيه نحو تحسين الاستراتيجيات. لا يعالج المعتقدات الخاطئة لدى الطالب حول قدراته وأسباب فشله."
    }
  },
  {
    "id": 42,
    "q": "للفروق الفردية أثر في التعلم، أكبر مدى للفروق يظهر في أي الصفات?",
    "options": ["الجسمية", "الشخصية", "المعرفية", "العقلية"],
    "answer": 2,
    "explanations": {
      "correct": "الصفات المعرفية تظهر فيها أكبر مدى للفروق الفردية لأنها تتأثر بالعديد من العوامل البيئية والوراثية والتعليمية. تشمل الصفات المعرفية أنماط التعلم وسرعة الاستيعاب والقدرة على التحليل والتركيب التي تختلف بشكل كبير بين الأفراد. تظهر الأبحاث أن الفروق في القدرات المعرفية قد تصل إلى ستة مستويات صفية في الفصل الواحد.",
      "wrong1": "الصفات الجسمية رغم اختلافها إلا أن مدى الفروق فيها أقل من الصفات المعرفية. الفروق في الطول والوزن والقدرات الحسية تكون ضمن نطاق محدود نسبياً. لا تؤثر الصفات الجسمية بشكل مباشر وكبير على عملية التعلم كما تؤثر الصفات المعرفية.",
      "wrong2": "الصفات الشخصية مهمة لكن مدى الفروق فيها أقل من الصفات المعرفية في تأثيرها على التعلم. السمات الشخصية كالانطواء والانبساط تؤثر على أسلوب التعلم وليس على القدرة المعرفية الأساسية. يمكن تعويض بعض الفروق الشخصية بأساليب تدريس مناسبة.",
      "wrong3": "الصفات العقلية جزء من الصفات المعرفية لكنها لا تمثل المدى الكامل للفروق. القدرات العقلية الأساسية تختلف ولكن الفروق في المعرفة والمهارات المكتسبة أكبر. الصفات المعرفية تشمل الجانبين الفطري والمكتسب مما يوسع مدى الفروق."
    }
  },
  {
    "id": 43,
    "q": "يؤكد المشرف التربوي للأستاذ خالد على أهمية تزويد الطلاب بتغذية راجعة حول مستوى تقدمهم في إتقان المهارات والمفاهيم أثناء تعلم الوحدة الدراسية أي أنواع التقويم الأتية يساعد على تقديم التغذية الراجعة المطلوبة ?",
    "options": ["التشخيصي", "التكويني", "النهائي", "القبلي"],
    "answer": 1,
    "explanations": {
      "correct": "التقويم التكويني هو الأنسب لتقديم التغذية الراجعة أثناء عملية التعلم لأنه يركز على متابعة تقدم الطلاب وتحسين التعلم. يتم تطبيقه بشكل مستمر خلال الدرس لتحديد نقاط القوة والضعف والعمل على تحسينها. يوفر معلومات فورية تمكن المعلم والطالب من تعديل الاستراتيجيات وتحسين الأداء.",
      "wrong1": "التقويم التشخيصي يهدف إلى تحديد المستوى الأولي للطلاب قبل البدء في عملية التعلم. يستخدم للكشف عن المعرفة السابقة والمهارات الأساسية لدى الطلاب. لا يوفر تغذية راجعة مستمرة أثناء عملية التعلم بل يسبقها.",
      "wrong2": "التقويم النهائي يطبق في نهاية الوحدة أو الفصل الدراسي لتقييم التحصيل النهائي. يركز على قياس النتائج النهائية وليس على تحسين عملية التعلم أثناء حدوثها. يأتي بعد انتهاء عملية التعلم لذا لا يمكن استخدامه لتعديل المسار.",
      "wrong3": "التقويم القبلي يسبق بداية التدريس بهدف تحديد الاستعدادات والمستويات الأولية. يساعد في تخطيط التدريس ولكن لا يقدم تغذية راجعة أثناء سير عملية التعلم. يعتبر تمهيداً للتعلم وليس أداة لتحسينه أثناء حدوثه."
    }
  },
  {
    "id": 44,
    "q": "بعد مراجعة المعلم لما قدمه والتفكر فيه، نوع التقويم:",
    "options": ["ذاتي", "تشخيصي", "تكويني", "ختامي"],
    "answer": 0,
    "explanations": {
      "correct": "التقويم الذاتي هو المناسب هنا لأنه يعتمد على مراجعة المعلم لأدائه وتفكيره في ما قدمه. يتضمن تحليل الشخص لأدائه وتفكيره في ممارساته التعليمية بهدف التحسين. يساعد المعلم على تطوير نفسه من خلال التفكير الناقد في أساليبه ونتائجها.",
      "wrong1": "التقويم التشخيصي يهدف لتحديد المستويات الأولية للطلاب قبل البدء في التدريس. لا يركز على تقييم المعلم لأدائه بل على تقييم الطلاب. يستخدم للكشف عن الصعوبات التعليمية المحتملة لدى المتعلمين.",
      "wrong2": "التقويم التكويني يهدف إلى تحسين عملية التعلم أثناء حدوثها من خلال التغذية الراجعة. يركز على تقييم تقدم الطلاب وليس على تقييم المعلم لذاته. يتم تطبيقه خلال العملية التعليمية وليس بعد انتهائها.",
      "wrong3": "التقويم الختامي يطبق في نهاية المقرر أو البرنامج لتقييم التحصيل النهائي. يركز على قياس النتائج النهائية للتعلم وليس على تقييم أداء المعلم. يعتبر تقويماً خارجياً وليس ذاتياً."
    }
  },
  {
    "id": 45,
    "q": "أي من التطبيقات الآتية يمكن للمعلم استخدامه للتواصل الإيجابي المنتظم مع أولياء أمور الطلاب ، وإطلاعهم على مدى تقدم أبنائهم دون الحاجة إلى إستدعاء أولياء الأمور للحضور ?",
    "options": ["Google Classroom", "School Circle", "Class Dojo", "Remind"],
    "answer": 3,
    "explanations": {
      "correct": "تطبيق Remind هو الأنسب للتواصل المنتظم مع أولياء الأمور لأنه مصمم خصيصاً للرسائل النصية والتواصل الفوري. يسمح بإرسال تحديثات منتظمة عن تقدم الطلاب وإنجازاتهم ومشاركة الصور والمستندات. يوفر خصوصية وأماناً في التواصل مع الحفاظ على الحدود المهنية المناسبة.",
      "wrong1": "Google Classroom مصمم primarily لإدارة الفصل الدراسي والتفاعل مع الطلاب. يوفر أدوات للتعلم لكنه ليس متخصصاً في التواصل مع أولياء الأمور. يحتاج أولياء الأمور إلى حسابات Google وقد لا يكون مناسباً للتواصل اليومي.",
      "wrong2": "School Circle قد يكون مفيداً لكنه ليس شائعاً أو متخصصاً في التواصل مع أولياء الأمور مثل Remind. قد لا يوفر نفس المستوى من الخصوصية وسهولة الاستخدام. يحتاج إلى بنية تحتية أكثر تعقيداً للتطبيق.",
      "wrong3": "Class Dojo مفيد لإدارة السلوك الصفي لكنه قد لا يكون الأنسب للتواصل المنتظم حول التقدم الأكاديمي. يركز أكثر على إدارة السلوك والمكافآت وليس على التواصل الشامل مع أولياء الأمور. قد لا يغطي جميع جوانب التقدم التعليمي المطلوب."
    }
  },
  {
    "id": 46,
    "q": "مؤشراً على أن معلم الرياضيات ينمي مهارات التفكير الإبداعي:",
    "options": ["يشكل اتجاهات إيجابية نحو الرياضيات", "يحقق متطلبات النجاح", "يفهم الطلاب المسائل", "يقدم الطلاب طرق مختلفة للحل"],
    "answer": 3,
    "explanations": {
      "correct": "تقديم الطلاب لطرق مختلفة للحل هو المؤشر الأقوى على تنمية التفكير الإبداعي لأنه يدل على المرونة والطلاقة في التفكير. يشير إلى قدرة الطلاب على النظر للمشكلات من زوايا متعددة وإيجاد حلول مبتكرة. يعكس تنمية مهارات التفكير التباعدي والقدرة على توليد بدائل متعددة.",
      "wrong1": "تشكيل اتجاهات إيجابية نحو الرياضيات مهم لكنه لا يعكس بالضرورة تنمية التفكير الإبداعي. قد يكون الطلاب إيجابيين نحو المادة لكنهم لا يمتلكون مهارات التفكير الإبداعي. يعتبر شرطاً مساعداً وليس مؤشراً مباشراً على الإبداع.",
      "wrong2": "تحقيق متطلبات النجاح يركز على الجانب الأكاديمي التقليدي وليس على الإبداع. النجاح في الاختبارات لا يعني بالضرورة امتلاك مهارات التفكير الإبداعي. قد يحقق الطلاب النجاح من خلال الحفظ والتكرار وليس من خلال التفكير المبتكر.",
      "wrong3": "فهم الطلاب للمسائل مهم لكنه يمثل المستوى الأساسي من التفكير وليس الإبداعي. الفهم ضروري لكنه لا يكفي لتطوير التفكير الإبداعي الذي يتطلب تجاوز الفهم إلى الابتكار. يعتبر أساساً للتفكير الإبداعي وليس تجسيداً له."
    }
  },
  {
    "id": 47,
    "q": "يبدأ المعلم (خالد) دروسه بتهيئة يشجع فيها طلابه على تكوين روابط بين مفاهيم الدروس ويجزئ المعلم (زيد) المادة التعليمية إلى وحدات متدرجة ويركز المعلم (عمر) على الملاحظة في دروسه لتحقيق الأهداف المرغوبة، أما المعلم (محمد) فيركز على تقويم الطلاب لادائهم بانفسهم بعد الانتهاء من المهمات التعليمية. المعلم الذي يطبق مبادي المدخل الاجتماعي في تدريسه هو :",
    "options": ["زيد", "عمر", "خالد", "محمد"],
    "answer": 2,
    "explanations": {
      "correct": "المعلم خالد هو الذي يطبق مبادئ المدخل الاجتماعي لأنه يشجع على تكوين روابط بين المفاهيم مما يتوافق مع نظرية فيجوتسكي. المدخل الاجتماعي يؤكد على أهمية التفاعل الاجتماعي وبناء المعرفة من خلال المشاركة. تكوين الروابط بين المفاهيم يتطلب حواراً ونقاشاً مما يعزز البناء الاجتماعي للمعرفة.",
      "wrong1": "المعلم زيد يطبق مبادئ التنظيم المنطقي للمحتوى وليس المدخل الاجتماعي. تجزئة المادة إلى وحدات متدرجة يركز على البنية المنطقية وليس على التفاعل الاجتماعي. يعكس النظرة السلوكية أو المعرفية أكثر من الاجتماعية.",
      "wrong2": "المعلم عمر يركز على الملاحظة التي قد تكون فردية ولا تتطلب بالضرورة تفاعلاً اجتماعياً. الملاحظة يمكن أن تكون نشاطاً فردياً لا يعكس البناء الاجتماعي للمعرفة. لا يشترط أن تتضمن المشاركة والتفاعل مع الآخرين.",
      "wrong3": "المعلم محمد يركز على التقويم الذاتي الذي يعزز الاستقلالية الفردية وليس التفاعل الاجتماعي. التقويم الذاتي نشاط فردي يتناسب مع النظريات البنائية الفردية. لا يتطلب التفاعل الاجتماعي أو البناء الجماعي للمعرفة."
    }
  },
  {
    "id": 48,
    "q": "كتبت الهمزات كتابة صحيحة في:",
    "options": [
      "هدفك يوصلك لما تريد فأسع وراءه للقيام بالأشياء التي تهمك",
      "لا تكن طاءشا في إختياراتك، وضع لك أهدافا ممتلئة بالنجاح",
      "أفضل طريقة لإزالة السلبية هو أن تحدد أهدافك وتراقب نتائجها",
      "ركز على أهدافك بعيدا عن إرضائي الناس والإستجابة لرغباتهم"
    ],
    "answer": 0,
    "explanations": {
      "correct": "الجملة الأولى كتبت الهمزات بشكل صحيح حيث كتبت همزة القطع في 'هدفك' و'أشياء' بشكل صحيح. همزة الوصل في 'اسع' كتبت دون همزة في أول الكلمة وفق القواعد. جميع الهمزات متوسطة ومتطرفة مكتوبة وفق قواعد الرسم الإملائي الصحيحة.",
      "wrong1": "الجملة الثانية تحتوي على أخطاء في كتابة الهمزات حيث كلمة 'طاءشا' الصواب 'طائشاً'. كما أن كلمة 'إختياراتك' الصواب 'اختياراتك' بهمزة وصل. هناك أخطاء في كتابة الهمزات المتوسطة والمتطرفة.",
      "wrong2": "الجملة الثالثة تحتوي على أخطاء إملائية في كتابة بعض الهمزات. كلمة 'إزالة' الصواب 'إزالة' أو 'ازالة' حسب القواعد الحديثة. هناك عدم دقة في تطبيق قواعد كتابة الهمزات في مواقع مختلفة.",
      "wrong3": "الجملة الرابعة بها أخطاء في كتابة الهمزات خاصة في كلمة 'إرضائي'. كما أن كلمة 'الإستجابة' الصواب 'الاستجابة' بهمزة وصل. تظهر أخطاء في تمييز همزة القطع من همزة الوصل."
    }
  },
  {
  "id": 49,
  "q": "كتبت الضاد والظاء بشكل صحيح في:",
  "options": [
    "خير الوعظ ما كان ظاهره العتاب",
    "في الظلام تضيق الرؤية وتتسع الأفكار",
    "أضعف الناس من أفشى سره وأضاع أمره",
    "التصرف في أثناء الغضب كالإبحار في خضم العاصفة"
  ],
  "answer": 1,
  "explanations": {
    "correct": "الجملة الثانية هي الوحيدة التي كُتبت فيها الضاد والظاء بشكل صحيح؛ فـ(الظلام) بالظاء الصحيحة، و(تضيق) بالضاد. جميع الكلمات موافقة للقواعد الإملائية.",
    "wrong1": "الجملة الأولى كانت مكتوبة خطأ بصيغة (ضاهره)، والصواب (ظاهره) بالظاء، لذا فهي لا تحقق شرط سلامة كتابة الضاد والظاء.",
    "wrong2": "الجملة الثالثة لا تضم حرف الظاء إطلاقًا، وكلمة (أضعف) صحيحة بالضاد، لكنها لا تحقق شرط وجود الضاد والظاء معًا مكتوبتين بشكل صحيح.",
    "wrong3": "الجملة الرابعة تحتوي على الضاد في كلمة (الغضب) بشكل صحيح، لكنها لا تحتوي على الظاء، ولا تحقق شرط السؤال الذي يطلب جملة تجمع الضاد والظاء وتكتبان فيها صحيحين."
    }
  },
  {
    "id": 50,
    "q": "الجملة الصحيحة إملائياً:",
    "options": ["كن دومن لطيفن", "كن دومن لطيفا", "كن دوما لطيفا", "كن دوما لطيفن"],
    "answer": 2,
    "explanations": {
      "correct": "الجملة 'كن دوماً لطيفاً' هي الصحيحة إملائياً حيث كتبت 'دوماً' بتنوين النصب الصحيح. كلمة 'لطيفاً' كتبت بتنوين النصب المناسب مع الألف. التعبير سليم إملائياً ويتوافق مع قواعد اللغة العربية الفصحى.",
      "wrong1": "الجملة 'كن دومن لطيفن' خاطئة لأن 'دومن' و'لطيفن' كتبتا بشكل غير صحيح. التنوين يجب أن يكتب مع الألف في حالة النصب. هناك أخطاء في كتابة علامات الإعراب والتنوين.",
      "wrong2": "الجملة 'كن دومن لطيفا' خاطئة لأن 'دومن' كتبت بشكل غير صحيح. الصواب 'دوماً' بتنوين النصب مع الألف. خطأ في كتابة التنوين في الكلمة الأولى مع صحة الثانية.",
      "wrong3": "الجملة 'كن دوما لطيفن' خاطئة لأن 'لطيفن' كتبت بشكل غير صحيح. الصواب 'لطيفاً' بتنوين النصب مع الألف. خطأ في كتابة التنوين في الكلمة الثانية مع صحة الأولى."
    }
  },
  {
    "id": 51,
    "q": "هذه الدرجة ...",
    "options": ["ملغاة", "ملغية", "لاغية", "ملتغاة"],
    "answer": 2,
    "explanations": {
      "correct": "كلمة 'لاغية' هي الصحيحة في هذا السياق لأنها ت形容 الإبطال والإلغاء في المصطلحات الإدارية والقانونية. تأتي من الفعل 'ألغى' الذي يعني أبطل أو أفسخ، وتستخدم لوصف ما تم إبطاله أو إسقاطه. في السياق التعليمي، 'الدرجة اللاغية' تعني الدرجة الملغاة أو المبطلة رسمياً.",
      "wrong1": "كلمة 'ملغاة' رغم أنها تحمل معنى الإلغاء إلا أنها ليست الاصطلاح الشائع في هذا السياق. تستخدم في سياقات أخرى ولكنها أقل شيوعاً في التعبير عن إلغاء الدرجات. الصيغة 'لاغية' هي الأكثر قبولاً في المصطلح الإداري التعليمي.",
      "wrong2": "كلمة 'ملغية' صيغة غير صحيحة من الناحية النحوية والصرفية. لا تتوافق مع قواعد اشتقاق الصفات من الأفعال في اللغة العربية. تعتبر خطأ شائعاً ولكنها غير مقبولة في الكتابة الرسمية.",
      "wrong3": "كلمة 'ملتغاة' صيغة غير موجودة في اللغة العربية ولا تتوافق مع أي من قواعد الاشتقاق. تعتبر خطأ إملائياً ونحوياً واضحاً. لا يمكن استخدامها في أي سياق رسمي أو أدبي."
    }
  },
  {
    "id": 52,
    "q": "لاحظت معلمة الصف الخامس أن إحدى الطالبات تتحاشى القراءة وإذا قرأت لا تقرأ بطلاقة ، وتستخدم أصابعها لتتبع الكلمات كما تخلط بين الكلمات المتشابهة الحروف شخصت المعلمة حالة الطالبة بأنها :",
    "options": ["بطء التعلم", "عوق إدراكي", "تأخر دراسي", "صعوبات تعلم"],
    "answer": 3,
    "explanations": {
      "correct": "الحالة تصنف كصعوبات تعلم لأن الأعراض تشمل صعوبات في القراءة والطلاقة وتمييز الحروف المتشابهة. صعوبات التعلم تعني وجود اضطراب في العمليات النفسية الأساسية المشاركة في الفهم أو استخدام اللغة. تظهر بشكل واضح في الصعوبات القرائية مع الحفاظ على المستوى الطبيعي للذكاء.",
      "wrong1": "بطء التعلم يختلف عن صعوبات التعلم حيث يشير إلى انخفاض عام في القدرات المعرفية. الطلاب بطيئو التعلم يكون أداؤهم منخفضاً في جميع المجالات وليس في مجالات محددة. الحالة المذكورة تركز على صعوبات نوعية في القراءة فقط.",
      "wrong2": "العوق الإدراكي يشير إلى إعاقات عقلية أكثر شمولية تؤثر على مختلف جوانب الحياة. يتضمن عادة قيوداً كبيرة في الأداء الوظيفي اليومي. الأعراض المذكورة لا تشير إلى عوق إدراكي شامل.",
      "wrong3": "التأخر الدراسي يعني تدني التحصيل العام دون وجود اضطرابات محددة في العمليات المعرفية. قد يكون بسبب عوامل بيئية أو ظروف اجتماعية. الحالة المذكورة تظهر صعوبات نوعية تشير إلى اضطراب في المعالجة اللغوية."
    }
  },
  {
    "id": 53,
    "q": "سبب تدني مستوى طلاب صعوبات التعلم:",
    "options": ["انخفاض الذكاء", "اضطراب العمليات الذهنية", "عدم وجود دافعية", "عدم القدرة على المشاركة"],
    "answer": 1,
    "explanations": {
      "correct": "السبب الرئيسي هو اضطراب العمليات الذهنية التي تؤثر على معالجة المعلومات. يشمل ذلك صعوبات في الذاكرة، الانتباه، الإدراك، والتفكير. هذه الاضطرابات تؤثر على كيفية تلقي المعلومات ومعالجتها وتخزينها واسترجاعها.",
      "wrong1": "انخفاض الذكاء ليس سمة لصعوبات التعلم، فكثير من ذوي صعوبات التعلم لديهم ذكاء طبيعي أو فوق الطبيعي. الفرق بين صعوبات التعلم والتخلف العقلي هو أن الأول يكون مع ذكاء طبيعي. الذكاء المنخفض يشير إلى فئات أخرى من الإعاقة.",
      "wrong2": "عدم وجود الدافعية قد يكون نتيجة لصعوبات التعلم وليس سبباً لها. الإحباط المتكرر من الفشل في التعلم قد يؤدي إلى انخفاض الدافعية. الدافعية تعتبر عاملاً ثانوياً وليس جذرياً في صعوبات التعلم.",
      "wrong3": "عدم القدرة على المشاركة قد يكون أحد المظاهر ولكن ليس السبب الجذري. يعود إلى الصعوبات الأساسية في المعالجة الذهنية التي تؤثر على المشاركة الفعالة. المشاركة تتأثر بالصعوبات وليست مسبباً لها."
    }
  },
  {
    "id": 54,
    "q": "سعر جوال 7000 ريال أصبح 3700 بعد 3 سنوات، الخصم السنوي:",
    "options": ["1100", "1300", "1500", "2100"],
    "answer": 0,
    "explanations": {
      "correct": "الخصم السنوي هو 1100 ريال، حيث أن إجمالي الخصم لمدة 3 سنوات هو 7000 - 3700 = 3300 ريال. بقسمة إجمالي الخصم على عدد السنوات: 3300 ÷ 3 = 1100 ريال سنوياً. هذا الحساب يفترض أن الخصم ثابت ومتساوي كل سنة.",
      "wrong1": "1300 ريال غير صحيح لأن 1300 × 3 = 3900، وإذا طرحناها من 7000 يصبح 3100 وليس 3700. الحساب لا يتطابق مع البيانات المعطاة في السؤال. الناتج النهائي يختلف عن السعر المذكور بعد الخصم.",
      "wrong2": "1500 ريال غير صحيح لأن 1500 × 3 = 4500، و7000 - 4500 = 2500 وليس 3700. الناتج النهائي أقل بكثير من السعر المطلوب. العملية الحسابية لا تعطي النتيجة الصحيحة.",
      "wrong3": "2100 ريال غير صحيح لأن 2100 × 3 = 6300، و7000 - 6300 = 700 وليس 3700. الفرق كبير جداً بين الناتج والقيمة المطلوبة. الحساب بعيد تماماً عن الإجابة الصحيحة."
    }
  },
  {
    "id": 55,
    "q": "أنواع القراءة من حيث الأداء:",
    "options": ["جهرية-صامتة", "سمعية-بصرية", "مرئية-مسموعة", "سريعة-باطنة"],
    "answer": 0,
    "explanations": {
      "correct": "التصنيف الصحيح لأنواع القراءة من حيث الأداء هو الجهرية والصامتة. القراءة الجهرية تتضمن النطق بالكلمات مسموعاً بينما الصامتة تكون دون صوت. هذا التصنيف يعتمد على طريقة أداء عملية القراءة وليس على قنوات الإدخال.",
      "wrong1": "السمعية-البصرية تصنيف لقنوات الإدراك وليس لأنواع القراءة من حيث الأداء. يشير إلى طريقة تلقي المعلومات وليس إلى أداء القراءة. يتعلق بحواس الإدراب وليس بطريقة الأداء.",
      "wrong2": "المرئية-المسموعة تصنيف مشابه للسمعية-البصرية ويركز على قنوات الإدخال. لا يعكس التمييز بين القراءة الجهرية والصامتة. ليس التصنيف المعتمد في الأدبيات التربوية.",
      "wrong3": "السريعة-الباطنة ليس تصنيفاً معتمداً لأنواع القراءة. القراءة الباطنة ليست مصطلحاً تربوياً معترفاً به. لا يمثل التقسيم الرئيسي المعتمد في تصنيف أنواع القراءة."
    }
  },
  {
    "id": 56,
    "q": "جدار طوله 6 م وعرضه 3، سعر المتر 20 ريال، تكلفة الطلاء:",
    "options": ["340", "400", "280", "360"],
    "answer": 3,
    "explanations": {
      "correct": "تكلفة الطلاء هي 360 ريال، حيث أن مساحة الجدار = الطول × العرض = 6 × 3 = 18 متراً مربعاً. التكلفة = المساحة × سعر المتر = 18 × 20 = 360 ريال. هذا الحساب يفترض أن الجدار مستطيل الشكل ويتم طلاء وجه واحد فقط.",
      "wrong1": "340 ريال غير صحيح لأنه لا يتوافق مع عملية الضرب 18 × 20. قد يكون نتيجة خطأ في حساب المساحة أو سعر المتر. لا يمثل ناتج العملية الحسابية الصحيحة.",
      "wrong2": "400 ريال قد يكون نتيجة حساب محيط الجدار بدلاً من المساحة. محيط الجدار = 2 × (6 + 3) = 18 متراً، و18 × 20 = 360 وليس 400. الحساب غير دقيق ولا يتطابق مع المعطيات.",
      "wrong3": "280 ريال غير صحيح وقد يكون نتيجة خطأ في ضرب 14 × 20 بدلاً من 18 × 20. أو قد يكون ناتجاً عن حساب غير دقيق للمساحة. لا يمثل الإجابة الصحيحة بناءً على المعطيات."
    }
  },
  {
  "id": 57,
  "q": "الدخول على موقع إلكتروني وتغيير تصميمه أو حذفه أو إتلافه يسمى:",
  "options": [
    "جريمة معلوماتية",
    "سرقة إلكترونية",
    "تخريب رقمي",
    "إتلاف معلوماتي"
  ],
  "answer": 0,
  "explanations": {
    "correct": "يُعد الدخول غير المشروع إلى موقع إلكتروني والقيام بتغيير تصميمه أو حذف محتواه أو إتلافه جريمة معلوماتية، لأنها تشمل أي اعتداء أو تعديل غير مصرح به يتم على الأنظمة أو المواقع أو البيانات الرقمية. ويدخل التخريب الرقمي ضمن هذا النوع من الجرائم.",
    "wrong1": "السرقة الإلكترونية تركز على الاستيلاء على البيانات أو الأموال ولا تتضمن بالضرورة التعديل أو الإتلاف.",
    "wrong2": "التخريب الرقمي يصف الفعل نفسه (تشويه أو تغيير الموقع)، لكنه ليس الاسم القانوني الأشمل للجريمة، بل يُعتبر جزءًا من الجريمة المعلوماتية.",
    "wrong3": "إتلاف معلوماتي مصطلح غير شائع وغير مستخدم بشكل رسمي في التصنيفات القانونية للجرائم المعلوماتية."
    }
  },
  {
    "id": 58,
    "q": "صفوة الأفكار في التقرير تكون في:",
    "options": ["المقدمة", "التحليل", "التمهيد", "الختام"],
    "answer": 3,
    "explanations": {
      "correct": "الختام هو مكان عرض صفوة الأفكار والاستنتاجات الرئيسية في التقرير. يجمل النتائج والتوصيات المستخلصة من التحليل السابق. يعتبر ملخصاً مركزاً لأهم ما توصل إليه التقرير من أفكار واستنتاجات.",
      "wrong1": "المقدمة تقدم خلفية عن الموضوع وأهداف التقرير ولكنها لا تحتوي على صفوة الأفكار. تركز على التمهيد للموضوع وليس على الاستنتاجات. تعتبر مدخلاً وليس خلاصة للتقرير.",
      "wrong2": "التحليل يقدم التفاصيل والبيانات والمناقشات ولكن ليس بالضرورة الصفوة المركزة. يعرض المعلومات بشكل مفصل وغير مركز. يركز على عملية التحليل وليس على النتائج النهائية.",
      "wrong3": "التمهيد يشبه المقدمة في كونه تمهيدياً ولا يحتوي على الخلاصات النهائية. يهيء القارئ للموضوع ولكن لا يقدم الاستنتاجات. يعتبر جزءاً تحضيرياً وليس ختامياً."
    }
  },
  {
    "id": 59,
    "q": "فصل 20 طالب، الموهوبين 10%، انضم 4 طلاب واحد منهم موهوب، النسبة الجديدة:",
    "options": ["12.5%", "17.5%", "20%", "15%"],
    "answer": 0,
    "explanations": {
      "correct": "النسبة الجديدة هي 12.5%، حيث أن عدد الموهوبين الأصلي = 20 × 10% = 2 طالب. بعد انضمام 4 طلاب واحد منهم موهوب، يصبح عدد الموهوبين = 3 طلاب من إجمالي 24 طالباً. النسبة = (3 ÷ 24) × 100 = 12.5%.",
      "wrong1": "17.5% غير صحيح لأنه سيعني وجود 4.2 طالب موهوب وهو عدد غير منطقي. لا يتوافق مع العملية الحسابية الصحيحة. النسبة مبالغ فيها ولا تعكس البيانات الحقيقية.",
      "wrong2": "20% غير صحيح لأنه سيعني وجود 4.8 طالب موهوب وهو غير ممكن. يتعارض مع مبدأ أن عدد الطلاب يجب أن يكون صحيحاً. النسبة مرتفعة جداً compared إلى البيانات المعطاة.",
      "wrong3": "15% غير صحيح لأنه سيعني وجود 3.6 طالب موهوب وهو عدد كسري غير مقبول. لا يمثل نتيجة القسمة الصحيحة 3/24. النسبة لا تتطابق مع الحساب الرياضي الدقيق."
    }
  },
  {
  "id": 60,
  "q": "وُصِفْتَ بأنك خبير تربوي في بناء المناهج، وطُلِبَ منك اختيار التنظيم الذي يهتم بحاجات الطلاب أكثر من ميولهم واهتماماتهم، ويُتيح للمعلم الاستعانة بمتخصصين آخرين، كما يتعامل فيه المعلم مع عدد قليل من الطلاب. فأيٌّ من تنظيمات المناهج الآتية يُعدّ الأنسب؟",
  "options": ["المحوري", "المواد المنفصلة", "المواد المترابطة", "المجالات العلمية"],
  "answer": 0,
  "explanations": {
    "correct": "التنظيم المحوري هو الأنسب لأنه يركز على حاجات الطلاب الأساسية ويسمح بمرونة في التدريس. يتميز بصغر عدد الطلاب في المجموعة الواحدة مما يتيح اهتماماً فردياً أكبر، كما يسمح للمعلم بالاستعانة بمتخصصين آخرين لدعم التعلم.",
    "wrong1": "تنظيم المواد المنفصلة يركز على التخصص الدراسي وليس بالضرورة على حاجات الطلاب. يعتمد على الفصل بين المواد ولا يوفّر التكامل أو المرونة المطلوبة.",
    "wrong2": "تنظيم المواد المترابطة يهتم بربط المواد ببعضها، لكنه لا يركز بدرجة كافية على الحاجات الفردية للطلاب، كما لا يضمن وجود مجموعات صغيرة.",
    "wrong3": "تنظيم المجالات العلمية يعتمد على التصنيفات الأكاديمية للمعرفة أكثر من اهتمامه بالحاجات الفردية للطلاب، ولا يوفّر المرونة أو العمل ضمن مجموعات صغيرة."
    }
  },
  {
    "id": 61,
    "q": "الإسهام في تعزيز مكانة المعلم العلمية والاجتماعية يمثل:",
    "options": ["الحقوق الوظيفية", "متطلبات الممارسة المهنية", "أهداف سياسة التعليم", "أهداف ميثاق أخلاقيات المهنة"],
    "answer": 0,
    "explanations": {
      "correct": "الإسهام في تعزيز مكانة المعلم العلمية والاجتماعية يمثل أحد الحقوق الوظيفية الأساسية للمعلم. هذه الحقوق تضمن للمعلم مكانة اجتماعية مناسبة وتقديراً لجهوده العلمية والتربوية. تشمل الحقوق الوظيفية أيضاً توفير البيئة المناسبة للتطوير المهني المستمر والاعتراف بالإنجازات العلمية.",
      "wrong1": "متطلبات الممارسة المهنية تركز على الواجبات والمسؤوليات التي يجب على المعلم الالتزام بها. تشمل المهارات والمعارف التي يحتاجها لأداء عمله بشكل فعال. لا تعتبر تعزيز المكانة من المتطلبات بل من الحقوق المكتسبة.",
      "wrong2": "أهداف سياسة التعليم تشمل الغايات العامة للنظام التعليمي على المستوى الوطني. تهتم بتطوير التعليم ككل وليس بالحقوق الفردية للمعلمين. تعتبر أوسع نطاقاً من مجرد تعزيز مكانة المعلم.",
      "wrong3": "أهداف ميثاق أخلاقيات المهنة تركز على السلوكيات والقيم الأخلاقية الواجب توفرها في المعلم. تشمل المبادئ والقيم التي تنظم العلاقات المهنية داخل المجتمع التعليمي. لا تتعلق مباشرة بتعزيز المكانة العلمية والاجتماعية."
    }
  },
  {
    "id": 62,
    "q": "الحصة السادسة وأذن الظهر، المعلم يغرس قيم التدين:",
    "options": ["يردد الأذان مع الطلاب", "يذكر قصص قصيرة عن الأذان", "يوضح واجب المسلم مع الأذان", "يستمر في شرح الدرس"],
    "answer": 2,
    "explanations": {
      "correct": "توضيح واجب المسلم مع الأذان هو التصرف الأنسب لأنه يربط بين الموقف التعليمي والقيمة الدينية بشكل عملي. يساعد الطلاب على فهم التطبيق العملي للتعاليم الدينية في حياتهم اليومية. يعزز الوعي الديني والسلوك الإسلامي الصحيح في المواقف الحياتية المختلفة.",
      "wrong1": "ترديد الأذان مع الطلاب قد يكون مناسباً لكنه لا يغرس القيمة بشكل عميق. يركز على الجانب الشكلي أكثر من الجوهر التربوي للقيمة. لا يساعد الطلاب على فهم المعنى الحقيقي للأذان وواجباتهم تجاهه.",
      "wrong2": "ذكر قصص عن الأذان مفيد لكنه لا يعالج الموقف المباشر الذي يعيشه الطلاب. القصص تقدم معرفة نظرية لكنها لا تربطها بالسلوك العملي المطلوب. يعتبر أسلوباً غير مباشر قد لا يحقق الهدف التربوي المنشود.",
      "wrong3": "الاستمرار في شرح الدرس يتجاهل الفرصة التربوية المتاحة لغرس القيم. يفصل بين الجانب التعليمي والتربوي مما يضعف تكامل الشخصية. لا يستثمر الموقف الطبيعي لتعزيز القيم الدينية لدى الطلاب."
    }
  },
  {
    "id": 63,
    "q": "إذا ابتسم المعلم فور أداء الطالب، نوع التعزيز:",
    "options": ["أولي", "ثانوي", "معنوي", "مادي"],
    "answer": 2,
    "explanations": {
      "correct": "الابتسامة تعتبر تعزيزاً معنوياً لأنها تعبر عن الرضا والتشجيع المعنوي. التعزيز المعنوي يعتمد على الإشارات الاجتماعية والعاطفية التي تعزز السلوك الإيجابي. يعتبر من أنجع أنواع التعزيز لأنه يبني الثقة ويعزز الدافعية الداخلية.",
      "wrong1": "التعزيز الأولي يرتبط بالحاجات البيولوجية الأساسية كالطعام والشراب. الابتسامة لا تشبع حاجة بيولوجية مباشرة للطالب. يعتبر أبعد أنواع التعزيز عن الموقف المذكور.",
      "wrong2": "التعزيز الثانوي يشمل المعززات التي اكتسبت قيمتها من ارتباطها بالمعززات الأولية. الابتسامة تعزز مباشرة وليس من خلال ارتباطها بمعززات أخرى. لا تحتاج إلى تكوين ارتباطات مسبقة لكي تكون فعالة.",
      "wrong3": "التعزيز المادي يشمل المكافآت الملموسة كالهدايا والعلامات. الابتسامة لا تعتبر مكافأة مادية ملموسة. يعتمد على الأشياء المحسوسة وليس على الإشارات الاجتماعية."
    }
  },
  {
  "id": 64,
  "q": "الأستاذ أحمد زرع قيمة المواطنة السعودية في نفوس المتعلمين، ووضع الأهداف الآتية لهذه القيمة: (1) أن يشارك الطالب في ندوة عن جهود المملكة العربية السعودية في خدمة الحرمين (2) أن يتمثل القدوة الحسنة لأسرته في بناء الحس الوطني (3) أن يقدر الطالب دور المملكة العربية السعودية في خدمة المسجد الأقصى (4) أن يبدي الطالب اهتمامه لحديث معلمه عن جهود المملكة العربية السعودية في خدمة الحجاج. الترتيب المناسب للأهداف من الأدنى إلى الأعلى لتحقيق القيمة وفق تصنيف كراثول هو:",
  "options": ["٤١٣٢", "٤٢٣١", "١٣٢٤", "١٢٣٤"],
  "answer": 0,
  "explanations": {
    "correct": "الترتيب الصحيح (٤١٣٢) يتوافق تماماً مع البنية الوجدانية التي وضعها كراثول لتطور القيم داخل شخصية المتعلم. لفهم الترتيب بعمق، يجب أن نعرف أن اكتساب القيم لا يحدث دفعة واحدة، بل يمر خلال مراحل تبدأ من مجرد الانتباه للمعلومة، ثم التفاعل معها، ثم إعطائها أهمية داخلية، وأخيراً تحويلها إلى سلوك مستقر يقود حياة الفرد. أولاً: الهدف (4) «يبدي الطالب اهتمامه لحديث معلمه…» يمثل المستوى الأول (الاستقبال Receiving)، وهو المستوى الذي لا يُطالب فيه الطالب بأي فعل أو سلوك، بل يكفي أن يُظهر انتباهاً أو استعداداً لسماع المعلومة. في هذا المستوى يكون الطالب في مرحلة بداية العلاقة مع القيمة، ولا تزال القيمة خارج شخصيته ولم تؤثر في سلوكه بعد، بل كل ما حدث هو فتح قناة الانتباه فقط. ثانياً: الهدف (1) «يشارك الطالب في ندوة…» ينتمي إلى مستوى (الاستجابة Responding)، وفيه ينتقل الطالب من مجرد الاستماع إلى القيام بسلوك فعلي يدل على تفاعل مع القيمة. المشاركة في ندوة ليست مجرد اهتمام؛ بل هي فعل يتضمن رغبة في الاندماج معناً وسلوكاً، وهذا يدل على أن القيمة بدأت تتحرك من الخارج إلى الداخل بدرجة ما. ثالثاً: الهدف (3) «يقدر الطالب دور المملكة…» يعبر عن مستوى (التقدير Valuing)، وهو نقطة تحول مهمة؛ لأن الطالب هنا لا يقوم بسلوك خارجي فقط، بل أصبحت القيمة ذات معنى عنده، وأصبح ينظر إليها على أنها شيء يستحق التقدير والدفاع عنه. هنا تتشكل الاتجاهات الوجدانية ويبدأ الطالب في بناء موقف داخلي ثابت تجاه قيمة المواطنة. رابعاً: الهدف (2) «يتمثل القدوة الحسنة لأسرته…» يمثل أعلى المستويات وهو (التنظيم/التوصيف Characterization). في هذا المستوى تصبح القيمة جزءًا أصيلًا من شخصية الطالب ومن نظامه الداخلي الذي يحكم سلوكياته في حياته اليومية. عندما يصبح الطالب قدوة لأسرته فهذا لا يعني استجابة مؤقتة، بل يعني أن القيمة استقرت وأصبحت مبدأ يوجه السلوك في مواقف مختلفة ومتجددة. هذا السلوك المتكرر أمام الأسرة يدل على تجذّر القيمة حتى أصبحت عنصرًا من عناصر الهوية والسمات الشخصية. لذلك فإن التسلسل (4 → 1 → 3 → 2) يعكس بدقة مسار تشكّل القيم بحسب كراثول: يبدأ الانتباه، ثم المشاركة، ثم تبني القيمة وجدانياً، ثم تحويلها إلى سلوك دائم ومستقر في حياة المتعلم.",
    "wrong1": "الخيار (٤٢٣١) يبدأ بشكل صحيح ثم ينقلب رأساً على عقب لأنه يضع القدوة (2) في مستوى منخفض، بينما هذا الهدف يمثل أعلى مستويات التجذّر السلوكي.",
    "wrong2": "الخيار (١٣٢٤) يفترض أن المشاركة هي البداية، وهذا يتجاهل أن كل القيم تبدأ باستقبال بسيط قبل أي استجابة.",
    "wrong3": "الخيار (١٢٣٤) يعكس الترتيب الطبيعي، إذ يبدأ بسلوك نشط ويجعل الاهتمام يأتي كخطوة نهائية، وهذا مخالف تماماً لتسلسل كراثول العلمي."
  }
  },
  {
    "id": 65,
    "q": "عندما ينظم المعلم خبراته التعليمية بحيث لا تكون مكررة لما سبق تدريسه بل إرتقاء بمستواه من مرحلة لأخرى مفهوم :",
    "options": ["التتابع", "التكامل", "التقويم", "التوازن"],
    "answer": 0,
    "explanations": {
      "correct": "مفهوم التتابع يعني تنظيم الخبرات التعليمية بشكل متدرج ومتسلسل دون تكرار. يعتمد على مبدأ البناء التراكمي للمعرفة من السهل إلى الصعب. يضمن تطور التعلم بشكل منطقي ومنظم من مرحلة إلى أخرى أعلى.",
      "wrong1": "التكامل يعني ربط الخبرات التعليمية المختلفة معاً في وحدة مترابطة. يركز على العلاقات الأفقية بين المواد وليس التسلسل الرأسي. لا يعالج بشكل مباشر مسألة التدرج وعدم التكرار.",
      "wrong2": "التقويم يعني تقييم مدى تحقيق الأهداف التعليمية وتحسين العملية. يركز على القياس والتقييم وليس على تنظيم الخبرات. يعتبر عملية منفصلة عن تنظيم المحتوى التعليمي.",
      "wrong3": "التوازن يعني توزيع الخبرات التعليمية بشكل متوازن بين مختلف المجالات. يهتم بالتنوع والتوازن في المحتوى وليس بالتسلسل والتدرج. لا يتناول بشكل مباشر مسألة التتابع والارتقاء بالمستوى."
    }
  },
  {
    "id": 66,
    "q": "التعلم الذي يتيح استخدام الأجهزة الخلوية وملحقاتها في إطار بيئة تعليمية تعلمية تشاركية غير محكومة بزمان او مكان يطلق عليه",
    "options": ["الحوسبة السحابية", "الرحلات المعرفية", "التعليم المنتقل", "التعليم المتزامن"],
    "answer": 2,
    "explanations": {
      "correct": "التعليم المنتقل هو المصطلح المناسب لأنه يشير إلى استخدام الأجهزة المحمولة في التعلم في أي وقت ومكان. يتميز بالمرونة والحركة ويتيح فرص التعلم خارج نطاق الفصل التقليدي. يعتمد على التقنيات اللاسلكية والأجهزة المحمولة لتقديم المحتوى التعليمي.",
      "wrong1": "الحوسبة السحابية تركز على توفير الخدمات والتطبيقات عبر الإنترنت. لا تشترط استخدام الأجهزة المحمولة بشكل مباشر. تعتبر تقنية داعمة للتعليم المنتقل وليس مرادفاً له.",
      "wrong2": "الرحلات المعرفية هي استراتيجية تعليمية تستخدم الإنترنت للبحث والاستكشاف. لا ترتبط بشكل خاص بالأجهزة المحمولة وخصائص التنقل. تعتبر أسلوباً تدريسياً وليس نموذجاً للتعلم المتنقل.",
      "wrong3": "التعليم المتزامن يعني حدوث التعلم في وقت واحد بين المعلم والمتعلمين. يتعارض مع فكرة عدم التحكم بالزمان والمكان. يرتبط بالتفاعل اللحظي وليس بالمرونة والحركة."
    }
  },
  {
    "id": 67,
    "q": "إذا اراد المعلم أن يبني هدفاً سلوكياً جيداً، فإن أهم الشروط التي يجب مراعاتها أن يتناول الهدف:",
    "options": ["ناتج التعلم", "موضوع التعلم", "عملية التعلم", "نشاط التعلم"],
    "answer": 0,
    "explanations": {
      "correct": "الهدف السلوكي الجيد يجب أن يركز على ناتج التعلم الذي يمكن ملاحظته وقياسه. يشير إلى السلوك النهائي المتوقع من الطالب بعد عملية التعلم. يجب أن يكون محدداً وواضحاً وقابلاً للقياس والتقييم.",
      "wrong1": "موضوع التعلم يمثل المحتوى التعليمي وليس الهدف السلوكي. يركز على المادة التعليمية وليس على نتيجة التعلم. لا يعبر عن التغير المتوقع في سلوك الطالب.",
      "wrong2": "عملية التعلم تركز على الطرق والأساليب المستخدمة في التدريس. تهتم بكيفية التعلم وليس بما سيتعلمه الطالب. تعتبر وسيلة وليس غاية في صياغة الأهداف.",
      "wrong3": "نشاط التعلم يمثل المهام والإجراءات التي يقوم بها الطالب. يركز على الفعل وليس على النتيجة المتوقعة. قد لا يعكس التغير الحقيقي في المعرفة أو المهارة."
    }
  },
  {
    "id": 68,
    "q": "اختبارات نسبة الذكاء تعد:",
    "options": ["ذاتي المرجع", "معياري المرجع", "محكي المرجع", "مبنية على المنهج"],
    "answer": 1,
    "explanations": {
      "correct": "اختبارات الذكاء تعتبر معياريَّة المرجع لأنها تقارن أداء الفرد بأداء مجموعة معيارية. تعتمد على المقارنة الإحصائية مع عينة ممثلة للمجتمع. تهدف إلى تحديد موقع الفرد بالنسبة لأقرانه في نفس الفئة العمرية.",
      "wrong1": "الاختبارات ذاتية المرجع تقارن أداء الفرد بأدائه السابق. تركز على النمو الفردي وليس المقارنة مع الآخرين. لا تناسب طبيعة اختبارات الذكاء التي تهتم بالمقارنة الجماعية.",
      "wrong2": "الاختبارات محكية المرجع تقيس مدى إتقان الفرد لمجالات معرفية محددة. تعتمد على معايير absolute وليس على المقارنة النسبية. تختلف عن اختبارات الذكاء التي تعتمد على التوزيع الطبيعي.",
      "wrong3": "الاختبارات المبنية على المنهج تقيس تحقيق أهداف منهج specific. ترتبط بمحتوى تعليمي محدد وليس بقدرات عقلية عامة. لا تنطبق على اختبارات الذكاء التي تقيس قدرات متعددة المجالات."
    }
  },
  {
  "id": 69,
  "q": "قدّم المعلم لطلابه نشاطاً يشتمل على مجموعات من المثلثات مختلفة الزوايا، وطلب منهم قياس زوايا كل مثلث ثم إيجاد مجموعها وملاحظة النتائج، حتى توصّل الطلاب إلى حقيقة أن مجموع زوايا المثلث يساوي 180 درجة. بناءً على ذلك، فإن طريقة التدريس المطبقة هي:",
  "options": ["الاستنباط", "الاستقراء", "العرض العملي", "حل المشكلات"],
  "answer": 1,
  "explanations": {
    "correct": "الطريقة المستخدمة هي **الاستقراء**، لأنها تبدأ من أمثلة جزئية (مثلثات مختلفة الزوايا) وتنتهي بالتوصل إلى قاعدة عامة (مجموع زوايا المثلث = 180). في هذه الطريقة، يقوم الطلاب بالملاحظة، والقياس، وجمع النتائج، ثم الوصول إلى القاعدة بأنفسهم. وهذا يعزز مهارات التفكير العلمي، والاستكشاف، والاستنتاج.",
    "wrong1": "طريقة **الاستنباط** غير مناسبة هنا لأنها تبدأ عادة من قاعدة عامة قائمة مسبقاً، ثم تنتقل إلى تطبيقها على أمثلة خاصة. في النشاط المطروح، الطلاب لم يطبقوا قاعدة، بل اكتشفوها، وهذا يتعارض مع فكرة الاستنباط.",
    "wrong2": "طريقة **العرض العملي** تعتمد على أن يقوم المعلم بعرض الخطوات أو التجربة أمام الطلاب بشكل مباشر لتوضيح المفهوم، دون أن يتوصل الطلاب إلى القاعدة بأنفسهم. بينما النشاط المذكور يعتمد على اكتشاف الطلاب للنتيجة من خلال إجراءاتهم الذاتية، وليس مجرد مشاهدة عرض.",
    "wrong3": "طريقة **حل المشكلات** غير مناسبة هنا، لأنها تفترض وجود مشكلة أو موقف يتطلب إيجاد حل. النشاط المعطى ليس مشكلة بحاجة إلى حل، بل هو نشاط استقصائي يهدف لاكتشاف قاعدة رياضية، وهو أقرب إلى الاستقراء منه إلى حل المشكلات."
    }
  },
  {
    "id": 70,
    "q": "طريقة تهتم بكم الأفكار قبل نوعيتها:",
    "options": ["حل المشكلات", "العصف الذهني", "المشروعات", "المحاضرة"],
    "answer": 1,
    "explanations": {
      "correct": "العصف الذهني هو الطريقة التي تهتم بكم الأفكار قبل نوعيتها حيث تشجع على توليد أكبر عدد ممكن من الأفكار. تعتمد على مبدأ تأجيل النقد والتقييم حتى اكتمال مرحلة توليد الأفكار. تهدف إلى تحرير التفكير من القيود وزيادة الطلاقة الإبداعية.",
      "wrong1": "حل المشكلات يركز على جودة الحلول وليس كم الأفكار. يهتم بالتحليل المنطقي والوصول إلى الحل الأمثل. يعتمد على التقييم والنقد منذ البداية.",
      "wrong2": "المشروعات تهتم بالتخطيط والتنفيذ الشامل للمهمة. تركز على الجودة والإتقان في العمل النهائي. لا تعطي أولوية لكم الأفكار في المراحل الأولى.",
      "wrong3": "المحاضرة تعتمد على نقل المعلومات من المعلم إلى الطلاب. لا تشجع على توليد الأفكار بل على استقبالها. تهتم بدقة المعلومة وجودة العرض وليس بكم الأفكار."
    }
  },
  {
    "id": 71,
    "q": "الحقائق التعليمية تعد:",
    "options": ["تعليم تبادلي", "تعليم مباشر", "تفريد تعلم", "تعليم موجه"],
    "answer": 1,
    "explanations": {
      "correct": "الحقائق التعليمية تعد من التعليم المباشر لأنها تعتمد على نقل المعلومات بشكل مباشر من المعلم إلى الطالب. هذا النوع من التعليم يتضمن تقديم الحقائق والمعلومات الجاهزة التي لا تحتاج إلى اكتشاف أو استقصاء. يعتبر فعالاً في نقل المعرفة الأساسية والمعلومات الواقعية التي تشكل أساساً للتعلم اللاحق.",
      "wrong1": "التعليم التبادلي يركز على الحوار والمناقشة بين المعلم والطلاب وليس على نقل الحقائق مباشرة. يعتمد على تبادل الآراء والأفكار وتطوير مهارات التفكير الناقد. لا يناسب نقل الحقائق المجردة التي تحتاج إلى شرح مباشر وواضح.",
      "wrong2": "تفريد التعلم يعني تكييف التعليم ليلائم احتياجات كل طالب فردية. يركز على التمايز في المحتوى والطريقة حسب قدرات الطلاب. لا يتناسب مع نقل الحقائق التعليمية التي تكون عادة موحدة لجميع الطلاب.",
      "wrong3": "التعليم الموجه يعني توجيه الطلاب نحو اكتشاف المعرفة بأنفسهم. يعتمد على التوجيه والإرشاد أكثر من النقل المباشر للمعلومات. يتناقض مع طبيعة الحقائق التعليمية التي تحتاج إلى عرض مباشر وواضح."
    }
  },
  {
    "id": 72,
    "q": "من حقوق المعلم المدنية:",
    "options": ["الاطلاع على تقويم الأداء", "دراسة المناهج وتقويمها", "المشاركة في برامج النشاط", "حضور الاجتماعات المدرسية"],
    "answer": 0,
    "explanations": {
      "correct": "الاطلاع على تقويم الأداء من الحقوق المدنية الأساسية للمعلم لأنه يتعلق بحقه في معرفة تقييم أدائه المهني. يمكّن المعلم من التعرف على نقاط القوة والضعف في أدائه والعمل على تطويرها. يعتبر شكلاً من أشكال الشفافية والعدالة في التقييم المهني.",
      "wrong1": "دراسة المناهج وتقويمها يعتبر من واجبات المعلم المهنية وليس من حقوقه المدنية. يتعلق بمهامه الوظيفية في تحليل المحتوى التعليمي وتطويره. يعكس المسؤولية المهنية أكثر من كونه حقاً مدنياً.",
      "wrong2": "المشاركة في برامج النشاط تعتبر من الواجبات الوظيفية التي تساهم في تحقيق أهداف المدرسة. تدخل في نطاق المسؤوليات المهنية للمعلم تجاه طلابه ومدرسته. لا تصنف كحق مدني بل كالتزام مهني.",
      "wrong3": "حضور الاجتماعات المدرسية يعتبر من الواجبات الإدارية والتنظيمية للمعلم. يدخل في إطار الالتزامات الوظيفية والانضباط المهني. لا يعتبر حقاً مدنياً بل مسؤولية وظيفية."
    }
  },
  {
    "id": 73,
    "q": "معلم يخطط لدرس جديد والطلاب ليس لديهم معلومات سابقة عنه ماذا يستخدم مع الطلاب من أبعاد اوزيل",
    "options": ["المقارن", "الاستقبالي", "الكشفي", "الشارح"],
    "answer": 2,
    "explanations": {
      "correct": "البعد الكشفي هو الأنسب عندما لا يكون لدى الطلاب معلومات سابقة عن الموضوع. يعتمد على استكشاف الطلاب للموضوع من خلال الأسئلة والمناقشات الاستقصائية. يساعد في بناء المعرفة من خلال الاكتشاف الموجه والتدرج في تقديم المعلومات.",
      "wrong1": "البعد المقارن يستخدم عندما يكون لدى الطلاب معرفة سابقة يمكن مقارنتها بالمعرفة الجديدة. يتطلب وجود إطار مرجعي سابق للمقارنة. لا يناسب الحالة التي يفتقد فيها الطلاب للمعلومات الأساسية.",
      "wrong2": "البعد الاستقبالي يركز على استقبال المعلومات بشكل سلبي من المعلم. لا يشجع على التفاعل النشط والاكتشاف الشخصي. يتناقض مع فكرة البناء المعرفي عند عدم وجود خلفية سابقة.",
      "wrong3": "البعد الشارح يعتمد على الشرح المباشر من قبل المعلم دون مشاركة فعالة من الطلاب. قد لا يكون فعالاً عندما يفتقر الطلاب للإطار المرجعي الأساسي. لا ينمي مهارات الاستقصاء والتفكير النشط."
    }
  },
  {
    "id": 74,
    "q": "في حصة الرياضيات بالصف الثاني الإبتدائي أحضر المعلم عددا كبيرا من الأدوات ذات الأشكال الهندسية المختلفة ، وكلف الطلاب بتصنيفها إلى مجموعات وفقا لعدد أضلاع الشكل الموقف السابق يساعد الطلاب على تعلم ... .?",
    "options": ["المفاهيم", "الحقائق", "التعميمات", "القواعد"],
    "answer": 0,
    "explanations": {
      "correct": "الموقف يساعد الطلاب على تعلم المفاهيم لأنه يتضمن التصنيف بناء على خصائص مشتركة. يتعلم الطلاب من خلاله مفهوم الأشكال الهندسية وخصائصها الأساسية. ينمي القدرة على التمييز بين المفاهيم المختلفة وتصنيفها حسب معايير محددة.",
      "wrong1": "الحقائق تمثل معلومات ثابتة ومحددة لا تحتاج إلى تصنيف أو تحليل. الموقف لا يركز على حفظ معلومات بل على فهم العلاقات والخصائص. يتجاوز مستوى الحقائق إلى مستوى الفهم والتطبيق.",
      "wrong2": "التعميمات تمثل قواعد عامة مستخلصة من عدة حالات خاصة. الموقف الحالي يركز على التصنيف وليس على استخلاص القواعد العامة. يعتبر خطوة تمهيدية للوصول إلى التعميمات لاحقاً.",
      "wrong3": "القواعد تمثل إجراءات ثابتة ومحددة يجب اتباعها. النشاط لا يتضمن تطبيق قواعد بل اكتشاف خصائص وتصنيفها. يركز على البناء المفاهيمي أكثر من التطبيق الآلي للقواعد."
    }
  },
  {
    "id": 75,
    "q": "تربية المواطن المؤمن ليكون لبنة صالحة في بناء أمته ، وذلك عن طريق إعداده إعداداً سليماً وتزويده بالقدر المناسب من المعلومات الثقافية والخبرات المختلفة . أي المبادئ الآتية في سياسة التعليم في المملكة العربية السعودية يمثل النموذج السابق ?",
    "options": ["الأصالة والتجديد", "التربية المتكاملة", "التربية للحياة", "تكافؤ الفرص"],
    "answer": 1,
    "explanations": {
      "correct": "مبدأ التربية المتكاملة هو الأنسب لأنه يجمع بين الجوانب الإيمانية والثقافية والخبرات المختلفة. يتوافق مع الرؤية الشاملة لتنمية الشخصية المتكاملة للمواطن. يعكس التوازن بين الجوانب الروحية والعقلية والاجتماعية في العملية التربوية.",
      "wrong1": "مبدأ الأصالة والتجديد يركز على الموازنة بين التراث والحداثة في التعليم. لا يعالج بشكل مباشر فكرة التربية الشاملة للمواطن. يتعلق أكثر بالمحتوى التعليمي وليس بالمنهجية التربوية الشاملة.",
      "wrong2": "مبدأ التربية للحياة يهتم بتأهيل الطالب للحياة العملية والمهنية. يركز على الجوانب التطبيقية والمهارات الحياتية. لا يغطي الجوانب الإيمانية والروحية بشكل كافٍ.",
      "wrong3": "مبدأ تكافؤ الفرص يعني توفير فرص التعليم المتكافئة للجميع. يتعلق بالعدالة في توزيع الخدمات التعليمية. لا يعكس فكرة التربية المتكاملة والشاملة للمواطن."
    }
  },
  {
    "id": 76,
    "q": "نموذج تقني يوفر التقنيات التعليمية متاح في أي وقت وأجهزة مختلفة:",
    "options": ["الواقع المعزز", "الكتب التفاعلية", "المدونات التعليمية", "الحوسبة السحابية"],
    "answer": 3,
    "explanations": {
      "correct": "الحوسبة السحابية هي النموذج التقني الذي يوفر التقنيات التعليمية في أي وقت ومن خلال أجهزة مختلفة. تتيح الوصول إلى التطبيقات والبيانات عبر الإنترنت دون الحاجة لتثبيتها على أجهزة محددة. توفر مرونة كبيرة في التعلم وتسهل التعاون بين الطلاب والمعلمين.",
      "wrong1": "الواقع المعزز يضيف طبقات رقمية على الواقع الحقيقي لكنه لا يضمن accessibility على جميع الأجهزة. يتطلب تقنيات وأجهزة محددة للتشغيل. لا يوفر نفس مستوى المرونة والوصول الشامل.",
      "wrong2": "الكتب التفاعلية تعتمد على تنسيقات وأجهزة محددة قد لا تكون متاحة للجميع. تتطلب توافقاً في البرامج والأجهزة للاستفادة منها. لا تقدم نفس مستوى المرحلة والاستقلالية عن الأجهزة.",
      "wrong3": "المدونات التعليمية توفر محتوى تعليمياً ولكنها لا توفر بيئة تعلم متكاملة. تعتبر أداة واحدة وليس نموذجاً تقنياً شاملاً. تفتقر للعديد من الميزات التفاعلية والتعاونية المتوفرة في الحوسبة السحابية."
    }
  },
  {
    "id": 77,
    "q": "مجموعة القواعد والمعايير التي توجه الأفراد نحو منافع الحياة الحديثة والحماية من أخطارها تعرف ب:",
    "options": ["الضبط الرقمي", "التوجيه الرقمي", "الرقابة الرقمية", "المواطنة الرقمية"],
    "answer": 3,
    "explanations": {
      "correct": "المواطنة الرقمية تشمل مجموعة القواعد والمعايير التي تنظم سلوك الأفراد في العالم الرقمي. تهدف إلى توجيه المستخدمين نحو الاستفادة الآمنة والإيجابية من التقنيات الحديثة. تشمل الجوانب الأخلاقية والأمنية والقانونية في استخدام التقنية.",
      "wrong1": "الضبط الرقمي يركز على الجوانب التقنية والسيطرة على الأنظمة الرقمية. لا يغطي الجوانب التربوية والاجتماعية الشاملة. يعتبر جزءاً من إدارة الأنظمة وليس توجيه السلوك البشري.",
      "wrong2": "التوجيه الرقمي قد يشير إلى الإرشاد التقني ولكن ليس كمصطلح شامل ومعترف به. لا يغطي جميع جوانب السلوك الرقمي المسؤول. ليس المصطلح المتعارف عليه في الأدبيات التربوية.",
      "wrong3": "الرقابة الرقمية تركز على المراقبة والتحكم في المحتوى الرقمي. تهتم بالجوانب الأمنية والرقابية أكثر من الجوانب التربوية. لا تعكس فكرة التوجيه الإيجابي والاستخدام المسؤول."
    }
  },
  {
    "id": 78,
    "q": "لاحظ المعلم محمود ان الطالب عبد الرحمن من الصف الأول الإبتدائي يأتي كل فترة وعلى جسمه آثار كدمات ، وعند سؤاله يجيب الطالب متردداً : وقعت يا أستاذ !! الإجراء المناسب الذي يجب على المعلم محمود القيام به هو:",
    "options": ["تجاهل ذلك لأنه حدث خارج الفصل", "الإتصال فورا بوالد الطفل للاستفسار", "إبلاغ إدارة المدرسة والمرشد الطلابي", "التحقيق مع الطالب ليتعرف على سبب ذلك"],
    "answer": 2,
    "explanations": {
      "correct": "إبلاغ إدارة المدرسة والمرشد الطلابي هو الإجراء المناسب لأنه يضمن التعامل المهني مع الحالة. المرشد الطلابي متخصص في التعامل مع مثل هذه الحالات ويمكنه تقييم الموقف بشكل صحيح. يحافظ على السرية والاحترافية ويضمن حماية حقوق الطالب.",
      "wrong1": "تجاهل الموقف غير أخلاقي ويتعارض مع مسؤولية المعلم towards حماية الطلاب. قد يعرض الطالب لمخاطر أكبر إذا كان يتعرض للإيذاء. يتجاهل واجب الإبلاغ عن حالات الإساءة المحتملة.",
      "wrong2": "الاتصال المباشر بوالد الطفل قد يكون خطيراً إذا كان الأهل هم مصدر الإيذاء. قد يعرض الطالب لخطر أكبر أو يزيد من تعنيفه. يجب ترك التحقيق للمتخصصين في هذا المجال.",
      "wrong3": "التحقيق المباشر مع الطالب قد يسبب خوفاً أو إحراجاً له. المعلم ليس متخصصاً في التحقيق في حالات الإساءة. قد يؤدي إلى تشويه الأدلة أو إرباك الطالب."
    }
  },
  {
    "id": 79,
    "q": "صف تتباين فيه قدرات الطلاب، أنسب أسلوب تدريس:",
    "options": ["المناقشة", "المحاضرة", "تفريد التعليم", "التعلم التعاوني"],
    "answer": 3,
    "explanations": {
      "correct": "التعلم التعاوني هو الأنسب للصفوف متباينة القدرات لأنه يستفيد من تنوع القدرات والمواهب. يمكن الطلاب من التعلم من بعضهم البعض وتكميل نقاط القوة والضعف. ينمي مهارات العمل الجماعي والاحترام المتبادل بين الطلاب مختلفي القدرات.",
      "wrong1": "المناقشة قد تفيد الطلاب المتميزين أكثر من غيرهم في الصفوف متباينة القدرات. قد لا تناسب الطلاب ضعيفي المستوى الذين يجدون صعوبة في المشاركة. لا توفر الدعم الفردي الكافي للطلاب المختلفي الاحتياجات.",
      "wrong2": "المحاضرة تعامل جميع الطلاب بنفس المستوى ولا تراعي الفروق الفردية. تقدم المحتوى بنفس الطريقة والسرعة للجميع. لا تتيح فرصاً كافية للطلاب ضعيفي المستوى للتعلم بالسرعة المناسبة لهم.",
      "wrong3": "تفريد التعليم قد يكون فعالاً لكنه يتطلب موارد ووقتاً كبيراً من المعلم. يصعب تطبيقه في الصفوف العادية ذات الأعداد الكبيرة. التعلم التعاوني أكثر واقعية ويحقق فوائد اجتماعية إضافية."
    }
  },
  {
    "id": 80,
    "q": "دور المتعلم في المدرسة السلوكية :",
    "options": [
      "مشاركة زملائه في إنجاز مهام التعلم المطلوبة",
      "تهيئة بيئة التعلم ، وانتقاء الأنشطة المناسبة لها",
      "تنظيم الممارسات العملية واستدعاء الاستجابات المناسبة",
      "الاستجابة للمؤثرات وتطبيق ما يتعلمه في مواقف جديدة"
    ],
    "answer": 3,
    "explanations": {
      "correct": "في المدرسة السلوكية، دور المتعلم هو الاستجابة للمؤثرات وتطبيق ما يتعلمه في مواقف جديدة. يركز هذا النهج على السلوك الظاهر والقابل للملاحظة والقياس. يعتمد على مبدأ التعزيز والعقاب في تشكيل سلوك المتعلم.",
      "wrong1": "مشاركة الزملاء في إنجاز المهام يتناسب أكثر مع النظريات الاجتماعية في التعلم. يركز على التفاعل الاجتماعي والتعاون بين الأقران. لا يعكس النظرة السلوكية التي تركز على الفرد واستجاباته.",
      "wrong2": "تهيئة بيئة التعلم وانتقاء الأنشطة من أدوار المعلم في النظريات البنائية. يعطي المتعلم دوراً نشطاً في بناء بيئة تعلمه. يتعارض مع النظرة السلوكية التي ترى المعلم كمصدر للمؤثرات.",
      "wrong3": "تنظيم الممارسات العملية واستدعاء الاستجابات يتناسب مع النظريات المعرفية. يركز على العمليات العقلية الداخلية والتنظيم الذاتي. لا يعكس النظرة السلوكية التي تهتم بالاستجابات الظاهرة فقط."
    }
  },
  {
    "id": 81,
    "q": "التوجه الحديث لتكييف المحتوى مع الفروق الفردية:",
    "options": ["التعلم النشط", "التعليم البنائي", "التعليم المتمايز", "التعليم الإلكتروني"],
    "answer": 2,
    "explanations": {
      "correct": "التعليم المتمايز هو التوجه الحديث الذي يركز على تكييف المحتوى والطريقة والتقييم ليتناسب مع الفروق الفردية بين الطلاب. يقوم هذا النهج على تصميم تجارب تعليمية متنوعة تلبي احتياجات المتعلمين المختلفين في نفس الصف الدراسي. يعتبر استجابة عملية للتنوع الكبير في قدرات الطلاب وأنماط تعلمهم وخلفياتهم الثقافية.",
      "wrong1": "التعلم النشط يركز على إشراك الطلاب في العملية التعليمية ولكن لا يتضمن بالضرورة تكييف المحتوى مع الفروق الفردية. يمكن تطبيقه بطرق موحدة دون مراعاة الاختلافات بين الطلاب. يعتبر استراتيجية تدريسية وليس نهجاً شاملاً للتكيف مع الفروق الفردية.",
      "wrong2": "التعليم البنائي يؤكد على بناء المعرفة من قبل المتعلم ولكن لا يركز بشكل خاص على تمايز المحتوى. يعطي أهمية للخبرات السابقة ولكن ليس بالضرورة من خلال تكييف منهجي للمحتوى. يركز على عملية التعلم أكثر من تركيزه على تمايز المحتوى التعليمي.",
      "wrong3": "التعليم الإلكتروني يوفر أدوات تقنية ولكن لا يضمن تكييف المحتوى مع الفروق الفردية تلقائياً. يمكن استخدامه لدعم التعليم المتمايز ولكن ليس مرادفاً له. يعتبر وسيلة وليس غاية في تكييف المحتوى مع احتياجات الطلاب."
    }
  },
  {
    "id": 82,
    "q": "من صور التفاعل الإيجابي الذي يقوم بها المعلم مع أولياء أمور الطلاب استخدام تقنيات التواصل لإطلاعهم على:",
    "options": ["أهداف المقررات الدراسية", "أهداف المعرفة ذات الأولوية", "خططه التدريسية وتعلم الطلاب", "تنظيم العمل التعليمي والإرشادي"],
    "answer": 2,
    "explanations": {
      "correct": "إطلاع أولياء الأمور على الخطط التدريسية وتعلم الطلاب يمثل تفاعلاً إيجابياً لأنه يشركهم في العملية التعليمية بشكل مباشر. يساعد هذا التواصل على بناء شراكة حقيقية بين البيت والمدرسة لدعم تعلم الطلاب. يمكن الأولياء من متابعة تطور أبنائهم وتقديم الدعم المناسب في الوقت المناسب.",
      "wrong1": "أهداف المقررات الدراسية مهمة لكن إطلاع أولياء الأمور عليها فقط لا يكفي لبناء تفاعل إيجابي مستمر. يعتبر معلومات عامة قد لا تثير اهتمام جميع أولياء الأمور بنفس الدرجة. لا يوفر صورة متكاملة عن تقدم الطالب الفعلي في التعلم.",
      "wrong2": "أهداف المعرفة ذات الأولوية تمثل جزءاً من المنهج ولكن إطلاع أولياء الأمور عليها فقط قد يكون محدود الفائدة. لا يعكس الجانب التطبيقي والتقدم الفعلي للطالب. قد يصبح التواصل نظرياً وغير مرتبط بالواقع اليومي للطالب.",
      "wrong3": "تنظيم العمل التعليمي والإرشادي يمثل معلومات إدارية وتنظيمية أكثر منها تعليمية. قد لا يهم جميع أولياء الأمور بنفس الدرجة خاصة إذا لم يرتبط بأداء أبنائهم المباشر. لا يوضح التقدم الفعلي للطلاب ولا يوفر مؤشرات محددة لأدائهم."
    }
  },
  {
    "id": 83,
    "q": "الإجراء التقويمي المناسب لوصف سلوك الطالب في بيئات التعلم هو :",
    "options": ["الملاحظة الصفية", "المقابلة الشخصية", "الاختبار الموضوعي", "تحليل السمات الشخصية"],
    "answer": 0,
    "explanations": {
      "correct": "الملاحظة الصفية هي الإجراء التقويمي الأنسب لوصف سلوك الطالب لأنها تتيح رصد السلوك في سياقه الطبيعي. تمكن المعلم من ملاحظة التفاعلات اليومية والاستجابات في المواقف التعليمية الحقيقية. توفر بيانات غنية ومتنوعة عن سلوك الطالب في مختلف الظروف والمواقف الصفية.",
      "wrong1": "المقابلة الشخصية مفيدة لكنها تعتمد على التقرير الذاتي للطالب وقد لا تعكس السلوك الفعلي. تتأثر بالقدرة التعبيرية للطالب ورغبته في الكشف عن سلوكه الحقيقي. لا توفر فرصة لملاحظة السلوك في سياقه الطبيعي.",
      "wrong2": "الاختبار الموضوعي يقيس التحصيل المعرفي وليس السلوك بشكل مباشر. يركز على المعرفة والمهارات الأكاديمية أكثر من السلوكيات اليومية. لا يمكنه التقاط التفاعلات الاجتماعية والسلوكيات في المواقف الطبيعية.",
      "wrong3": "تحليل السمات الشخصية يعتمد على استبانات وتقارير قد لا تعكس السلوك الفعلي في الصف. يتطلب وقتاً طويلاً وقد لا يكون عملياً للملاحظة اليومية. يركز على السمات العامة وليس على السلوكيات المحددة في بيئة التعلم."
    }
  },
  {
    "id": 84,
    "q": "أراد معلم استخدام استراتيجية تدريسية من بين استراتيجيات متعددة، فأي المعايير الآتية يجب عليه مراعاتها?",
    "options": ["تبني استراتيجية تبرز استقلالية الطلاب", "انتقاء استراتيجية تتطلب فصولا مكتملة التجهيزات", "اختيار استراتيجية ترتبط بخصائص الطلاب وحاجاتهم", "التركيز على استراتيجية شائعة يستخدمها الزملاء بكثرة"],
    "answer": 2,
    "explanations": {
      "correct": "اختيار استراتيجية ترتبط بخصائص الطلاب وحاجاتهم هو المعيار الأساسي الذي يجب مراعاته. يضمن هذا المعيار أن تكون الاستراتيجية مناسبة لمستوى الطلاب وقدراتهم وأنماط تعلمهم. يسهم في تحقيق أقصى استفادة من عملية التعلم ويزيد من فعالية التدريس.",
      "wrong1": "تبني استراتيجية تبرز استقلالية الطلاب مهم لكنه ليس المعيار الأساسي لاختيار الاستراتيجية. بعض الاستراتيجيات قد تبرز الاستقلالية ولكنها لا تناسب جميع المواقف التعليمية. يجب أن يكون التركيز على ملاءمة الاستراتيجية للغرض التعليمي وليس على خاصية واحدة فقط.",
      "wrong2": "انتقاء استراتيجية تتطلب فصولاً مكتملة التجهيزات قد لا يكون عملياً في جميع الظروف. التجهيزات تمثل عاملاً مساعداً وليس معياراً أساسياً لاختيار الاستراتيجية. قد يحرم هذا المعيار المعلم من استخدام استراتيجيات فعالة بسبب محدودية الإمكانات.",
      "wrong3": "التركيز على استراتيجية شائعة يستخدمها الزملاء ليس معياراً صحيحاً لاختيار الاستراتيجية. الشعبية لا تضمن الفعالية مع جميع المجموعات الطلابية. يجب أن يعتمد الاختيار على تحليل احتياجات الطلاب وليس على تقليد الآخرين."
    }
  },
  {
  "id": 85,
  "q": "استخدم المعلم استراتيجية تعلم نشط حديثة وهي:",
  "options": ["بيسك", "فراير", "H4", "كاروسل"],
  "answer": 2,
  "explanations": {
    "correct": "استراتيجية H4 تعد إحدى استراتيجيات التعلم النشط الحديثة التي تركز على جعل المتعلم محور العملية التعليمية من خلال أربع خطوات متتابعة: Hear وHunt وHuddle وHighlight. تجمع هذه الاستراتيجية بين التهيئة السمعية، والبحث الاستقصائي، والنقاش التعاوني، ثم عرض النتائج. وتساعد هذه الخطوات المتسلسلة على تعزيز الفهم العميق، وتنمية مهارات التواصل، ورفع مستوى المشاركة الفاعلة داخل الصف.",
    "wrong1": "بيسك (PECS) هو نظام تواصل معتمد على الصور ويُستخدم بشكل رئيسي مع الطلاب ذوي اضطراب طيف التوحد بهدف دعم التواصل الوظيفي. وعلى الرغم من فعاليته في تطوير مهارات التعبير، إلا أنه لا يُعد استراتيجية تعلم نشط صفية. فهو يركز على إنشاء قنوات تواصل بديلة أكثر من تركيزه على بناء مواقف تعلم تفاعلية قائمة على الاستقصاء أو العمل الجماعي.",
    "wrong2": "نموذج فراير (Frayer Model) هو أداة لتنظيم المفاهيم وتوضيحها من خلال التعريف والخصائص والأمثلة وغير الأمثلة. ورغم أنه يدعم الفهم العميق للمصطلحات، إلا أنه ليس استراتيجية تعلم نشط متكاملة، بل يعد وسيلة تنظيم معرفي. لا يشمل النموذج خطوات بحث أو تفاعل جماعي ديناميكي، مما يجعله مختلفًا عن الاستراتيجيات الحديثة القائمة على الحركة والتعاون والاستقصاء.",
    "wrong3": "استراتيجية كاروسل (Carousel) تُعد من استراتيجيات التعلم النشط الشائعة، حيث ينتقل الطلاب بين محطات تعلم مختلفة لإنجاز مهام متنوعة. لكنها ليست الاستراتيجية المقصودة في هذا السؤال لأن خطواتها وآلياتها تختلف تمامًا عن نموذج H4 الذي يعتمد على الاستماع والبحث والنقاش ثم العرض. وعلى الرغم من حداثتها وشيوعها، إلا أن إجابة السؤال تتطلب تحديد الاستراتيجية ذات الهيكلة الرباعية H4."
    }
  },
  {
    "id": 86,
    "q": "منحنى التدريس هو :",
    "options": ["استراتيجية التدريس", "طريقة التدريس", "أسلوب التدريس", "مدخل التدريس"],
    "answer": 3,
    "explanations": {
      "correct": "منحنى التدريس يعد مدخلاً للتدريس لأنه يمثل إطاراً نظرياً شاملاً يوجه العملية التعليمية. يتضمن نظرية متكاملة عن كيفية حدوث التعلم وأفضل السبل لتحقيقه. يشكل الأساس الفلسفي والتربوي الذي تبنى عليه الاستراتيجيات والطرق والأساليب التدريسية.",
      "wrong1": "استراتيجية التدريس تمثل خططاً وتصميمات تنفيذية محددة داخل مدخل التدريس. تعتبر أداة تطبيقية وليست الإطار النطري الشامل. تندرج تحت مدخل التدريس وليس العكس.",
      "wrong2": "طريقة التدريس تشير إلى الإجراءات والتقنيات المحددة المستخدمة في تنفيذ الدرس. تمثل المستوى التطبيقي الأكثر تحديداً من مدخل التدريس. تعتبر جزءاً من المدخل وليس المدخل نفسه.",
      "wrong3": "أسلوب التدريس يعكس الطريقة الشخصية للمعلم في التفاعل مع الطلاب وتنفيذ التدريس. يتعلق بالخصائص الفردية للمعلم وليس بالإطار النظري الشامل. يعتبر مكملاً لمدخل التدريس وليس مرادفاً له."
    }
  
            }, 
            // يمكن إضافة المزيد من الأسئلة هنا
        ];

        let currentQuestionIndex = 0;
        let userAnswers = Array(questions.length).fill(null);
        let timeLeft = 45 * 60; // 45 دقيقة
        let timerInterval;
        let markedQuestions = [];
        let answerLocked = Array(questions.length).fill(false); // مصفوفة لتتبع حالة القفل لكل سؤال

        // تبديل الوضع الليلي
        document.getElementById('themeBtn').addEventListener('click', function() {
            document.body.classList.toggle('dark-theme');
            const icon = this.querySelector('i');
            if (document.body.classList.contains('dark-theme')) {
                icon.classList.remove('fa-moon');
                icon.classList.add('fa-sun');
                localStorage.setItem('darkMode', 'enabled');
            } else {
                icon.classList.remove('fa-sun');
                icon.classList.add('fa-moon');
                localStorage.setItem('darkMode', 'disabled');
            }
        });

        // التحقق من تفضيل الوضع الداكن المخزن
        function checkDarkModePreference() {
            const darkMode = localStorage.getItem('darkMode');
            const icon = document.querySelector('#themeBtn i');
            
            if (darkMode === 'enabled') {
                document.body.classList.add('dark-theme');
                icon.classList.remove('fa-moon');
                icon.classList.add('fa-sun');
            } else {
                document.body.classList.remove('dark-theme');
                icon.classList.remove('fa-sun');
                icon.classList.add('fa-moon');
            }
        }

        // المؤقت
        function startTimer() {
            timerInterval = setInterval(() => {
                timeLeft--;
                updateTimerDisplay();
                
                if (timeLeft <= 0) {
                    clearInterval(timerInterval);
                    finishQuiz();
                }
            }, 1000);
        }

        function updateTimerDisplay() {
            const minutes = Math.floor(timeLeft / 60);
            const seconds = timeLeft % 60;
            const timeDisplay = document.getElementById('time-display');
            timeDisplay.textContent = `${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
            
            if (timeLeft < 300) { // 5 دقائق
                timeDisplay.classList.add('timer-warning');
            } else {
                timeDisplay.classList.remove('timer-warning');
            }
        }

        // عرض قائمة الأسئلة
        function showQuestionsList() {
            const grid = document.getElementById('questions-grid');
            grid.innerHTML = '';
            
            questions.forEach((_, index) => {
                const btn = document.createElement('div');
                btn.className = `question-status-grid ${index === currentQuestionIndex ? 'current' : ''} ${userAnswers[index] !== null ? 'answered' : ''} ${markedQuestions.includes(index) ? 'flagged' : ''}`;
                btn.innerHTML = `<span>${index + 1}</span>`;
                btn.onclick = () => {
                    currentQuestionIndex = index;
                    loadQuiz();
                    hideQuestionsList();
                };
                grid.appendChild(btn);
            });
            
            document.getElementById('questions-list').style.display = 'block';
        }

        function hideQuestionsList() {
            document.getElementById('questions-list').style.display = 'none';
        }

        // وضع علامة للمراجعة
        function toggleMarkForReview() {
            const index = markedQuestions.indexOf(currentQuestionIndex);
            const btn = document.getElementById('mark-review-btn');
            
            if (index === -1) {
                markedQuestions.push(currentQuestionIndex);
                btn.innerHTML = '<i class="fas fa-flag"></i> إزالة العلامة';
                btn.style.background = 'var(--tertiary)';
            } else {
                markedQuestions.splice(index, 1);
                btn.innerHTML = '<i class="fas fa-flag"></i> وضع علامة للمراجعة';
                btn.style.background = 'var(--secondary)';
            }
            
            if (document.getElementById('questions-list').style.display === 'block') {
                showQuestionsList();
            }
        }

        // تحميل الاختبار
        function loadQuiz() {
            const quizDiv = document.getElementById("quiz");
            quizDiv.innerHTML = "";

            const question = questions[currentQuestionIndex];
            const isLocked = answerLocked[currentQuestionIndex];
            
            let html = `
                <div class="question-box fade-in">
                    <div class="question-number">
                        <i class="fas fa-question-circle"></i>
                        السؤال ${currentQuestionIndex + 1} من ${questions.length}
                        ${isLocked ? '<span style="color: var(--accent); margin-right: 10px;"><i class="fas fa-lock"></i> مقفل</span>' : ''}
                    </div>
                    <div class="question-text">${question.q}</div>
                    <div class="options">
            `;
            
            question.options.forEach((opt, i) => {
                const isChecked = userAnswers[currentQuestionIndex] === i;
                const isDisabled = isLocked;
                let labelClass = '';
                
                if (isLocked) {
                    labelClass = 'locked';
                    if (isChecked) {
                        labelClass += userAnswers[currentQuestionIndex] === question.answer ? ' correct-answer' : ' wrong-answer';
                    } else if (i === question.answer) {
                        labelClass += ' correct-answer';
                    }
                } else if (isChecked) {
                    labelClass = 'selected';
                }
                
                html += `
                    <label class="${labelClass}">
                        <input type="radio" name="q${currentQuestionIndex}" value="${i}" ${isChecked ? 'checked' : ''} ${isDisabled ? 'disabled' : ''} onchange="selectAnswer(${i})">
                        ${opt}
                        ${isLocked && i === question.answer ? ' <i class="fas fa-check" style="color: var(--secondary); margin-right: 5px;"></i>' : ''}
                    </label>
                `;
            });
            
            html += `
                    </div>
                    <div id="explanation" class="explanation"></div>
                </div>
                <div class="navigation">
                    <button class="btn btn-secondary" onclick="previousQuestion()" ${currentQuestionIndex === 0 ? 'disabled' : ''}>
                        <i class="fas fa-arrow-right"></i>
                        السابق
                    </button>
                    <button class="btn btn-primary" onclick="nextQuestion()" ${currentQuestionIndex === questions.length - 1 ? 'disabled' : ''}>
                        التالي
                        <i class="fas fa-arrow-left"></i>
                    </button>
                </div>
            `;
            
            quizDiv.innerHTML = html;
            
            // تحديث شريط التقدم
            document.getElementById('progress').style.width = `${((currentQuestionIndex + 1) / questions.length) * 100}%`;
            
            // تحديث معلومات الاختبار
            document.getElementById('quiz-info').innerHTML = `السؤال ${currentQuestionIndex + 1} من ${questions.length}`;
            
            // تحديث زر وضع العلامة
            const markBtn = document.getElementById('mark-review-btn');
            if (markedQuestions.includes(currentQuestionIndex)) {
                markBtn.innerHTML = '<i class="fas fa-flag"></i> إزالة العلامة';
                markBtn.style.background = 'var(--tertiary)';
            } else {
                markBtn.innerHTML = '<i class="fas fa-flag"></i> وضع علامة للمراجعة';
                markBtn.style.background = 'var(--secondary)';
            }
            
            // عرض الشرح إذا كان المستخدم قد أجاب على السؤال
            if (userAnswers[currentQuestionIndex] !== null) {
                showExplanation();
            }
        }

        // اختيار إجابة
        function selectAnswer(answerIndex) {
            userAnswers[currentQuestionIndex] = answerIndex;
            answerLocked[currentQuestionIndex] = true; // قفل الإجابة
            showExplanation();
            loadQuiz(); // إعادة تحميل لعرض التغييرات
        }

        // عرض الشرح
        function showExplanation() {
            const question = questions[currentQuestionIndex];
            const explanationDiv = document.getElementById("explanation");
            const userAnswer = userAnswers[currentQuestionIndex];
            
            if (userAnswer !== null) {
                explanationDiv.style.display = "block";
                
                let resultHTML = "";
                
                if (userAnswer === question.answer) {
                    resultHTML = `<p class="correct"><i class="fas fa-check-circle"></i> إجابة صحيحة</p>`;
                } else {
                    resultHTML = `
                        <p class="wrong"><i class="fas fa-times-circle"></i> إجابة خاطئة — الإجابة الصحيحة: <span class="correct">${question.options[question.answer]}</span></p>
                    `;
                }
                
                // إضافة الشروح الملونة
                resultHTML += `
                    <div class="explanation-line explanation-correct"><strong>التفسير الصحيح:</strong> ${question.explanations.correct}</div>
                `;
                
                if (question.explanations.wrong1) {
                    resultHTML += `<div class="explanation-line explanation-wrong-1">${question.explanations.wrong1}</div>`;
                }
                
                if (question.explanations.wrong2) {
                    resultHTML += `<div class="explanation-line explanation-wrong-2">${question.explanations.wrong2}</div>`;
                }
                
                if (question.explanations.wrong3) {
                    resultHTML += `<div class="explanation-line explanation-wrong-3">${question.explanations.wrong3}</div>`;
                }
                
                explanationDiv.innerHTML = resultHTML;
            }
        }

        // الانتقال إلى السؤال التالي
        function nextQuestion() {
            if (currentQuestionIndex < questions.length - 1) {
                currentQuestionIndex++;
                loadQuiz();
            }
        }

        // الانتقال إلى السؤال السابق
        function previousQuestion() {
            if (currentQuestionIndex > 0) {
                currentQuestionIndex--;
                loadQuiz();
            }
        }

        // عرض الدرجات الحالية دون إنهاء الاختبار
        function showCurrentScore() {
            let totalCorrect = 0;
            userAnswers.forEach((answer, index) => {
                if (answer === questions[index].answer) {
                    totalCorrect++;
                }
            });

            const total = questions.length;
            const percentage = ((totalCorrect / total) * 100).toFixed(2);

            document.getElementById("current-score").style.display = "block";
            document.getElementById("current-correct").innerHTML = `الإجابات الصحيحة: ${totalCorrect} من ${total}`;
            document.getElementById("current-percentage").innerHTML = `النسبة المئوية الحالية: ${percentage}%`;
        }

        // حساب الدرجات النهائية
        function finishQuiz() {
            clearInterval(timerInterval);
            
            let totalCorrect = 0;
            userAnswers.forEach((answer, index) => {
                if (answer === questions[index].answer) {
                    totalCorrect++;
                }
            });

            const total = questions.length;
            const percentage = ((totalCorrect / total) * 100).toFixed(2);

            let evaluation = "";
            let evaluationIcon = "";
            if (percentage >= 90) {
                evaluation = "ممتاز";
                evaluationIcon = "🌟";
            } else if (percentage >= 80) {
                evaluation = "جيد جداً";
                evaluationIcon = "🔵";
            } else if (percentage >= 70) {
                evaluation = "جيد";
                evaluationIcon = "🟢";
            } else {
                evaluation = "يحتاج تحسين";
                evaluationIcon = "⚠️";
            }

            document.getElementById("result-box").style.display = "block";
            document.getElementById("result").innerHTML = `${evaluationIcon} النتيجة: ${totalCorrect} من ${total}`;
            document.getElementById("percentage").innerHTML = `النسبة المئوية: ${percentage}%`;
            document.getElementById("evaluation").innerHTML = `التقييم: ${evaluation}`;
            
            // إخفاء الاختبار
            document.getElementById("quiz").style.display = "none";
            document.querySelector(".controls").style.display = "none";
            document.getElementById('questions-list').style.display = 'none';
        }

        // بدء التحميل الأولي
        window.onload = function() {
            checkDarkModePreference();
            loadQuiz();
            startTimer();
        }
    </script>
</body>
</html>
