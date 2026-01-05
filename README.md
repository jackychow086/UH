<UH>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UH | 氫能航空動力專家</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@300;400;700&display=swap');
        body { font-family: 'Noto Sans TC', sans-serif; background-color: #f8fafc; color: #1e293b; scroll-behavior: smooth; margin: 0; padding: 0; }
        .hero-bg { background: linear-gradient(135deg, #0f172a 0%, #1e40af 100%); position: relative; overflow: hidden; }
        .data-card { background: white; border-radius: 16px; border: 1px solid #e2e8f0; transition: all 0.3s ease; }
        .data-card:hover { transform: translateY(-5px); box-shadow: 0 15px 30px -10px rgba(0,0,0,0.1); border-color: #3b82f6; }
        .reveal { opacity: 0; transform: translateY(30px); transition: all 0.8s ease-out; }
        .reveal.active { opacity: 1; transform: translateY(0); }
        .highlight { color: #3b82f6; font-weight: bold; }
    </style>
</head>
<body>

    <nav class="bg-white/80 backdrop-blur-md border-b sticky top-0 z-50 px-8 py-4">
        <div class="max-w-7xl mx-auto flex justify-between items-center">
            <span class="text-xl font-bold tracking-tight text-slate-800">UH <span class="text-blue-600">Aviation</span></span>
            <div class="space-x-8 text-sm font-medium">
                <a href="#vision" class="hover:text-blue-600">核心願景</a>
                <a href="#tech" class="hover:text-blue-600">技術實力</a>
                <a href="#market" class="hover:text-blue-600">市場路徑</a>
            </div>
        </div>
    </nav>

    <header id="vision" class="hero-bg text-white py-24 px-6 text-center">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-5xl md:text-6xl font-bold mb-8 leading-tight">
                引領下一代 <span class="text-blue-400">液態氫</span> <br>eVTOL 動力革命
            </h1>
            <p class="text-xl text-blue-100 mb-12 font-light">
                UH 致力於為 eVTOL 提供液態氫（LH2）儲存與燃料電池動力系統。
            </p>
            <div class="flex flex-wrap justify-center gap-6">
                <div class="bg-white/10 px-6 py-3 rounded-full border border-white/20">TRL 6-7 技術驗證</div>
                <div class="bg-white/10 px-6 py-3 rounded-full border border-white/20">專注高增長市場</div>
            </div>
        </div>
    </header>

    <section class="py-20 px-6 max-w-4xl mx-auto text-center reveal">
        <h2 class="text-3xl font-bold mb-6">為什麼是現在？為什麼是液態氫？</h2>
        <p class="text-lg text-slate-600 leading-relaxed">
            對於實際航程需求，電池過重，氣態氫體積則過於龐大。<br>
            對於 eVTOL，僅需數十公斤液態氫 (LH2) 即可達成所需的續航時間與任務目標。
        </p>
    </section>

    <section id="tech" class="py-16 px-6 max-w-7xl mx-auto grid md:grid-cols-3 gap-8">
        <div class="data-card p-8 reveal">
            <div class="text-blue-600 text-3xl mb-6"><i class="fas fa-microchip"></i></div>
            <h3 class="text-xl font-bold mb-4">1. 已驗證動力系統</h3>
            <p class="text-slate-500 text-sm mb-6">曾成功在測試平台上飛行測試 1MW 氫電動力系統。</p>
            <button onclick="toggleInfo('tech1')" class="text-blue-600 text-sm font-bold hover:underline">查看詳情</button>
            <div id="tech1" class="hidden mt-4 text-xs bg-slate-50 p-4 rounded-lg">技術包含模塊化 LH2 儲存與經過驗證的真空絕緣技術。</div>
        </div>

        <div class="data-card p-8 reveal">
            <div class="text-emerald-600 text-3xl mb-6"><i class="fas fa-chart-line"></i></div>
            <h3 class="text-xl font-bold mb-4">2. 鎖定領先市場</h3>
            <p class="text-slate-500 text-sm mb-6">中國是全球 eVTOL 領先市場，已有商業營運案例。</p>
            <button onclick="toggleInfo('tech2')" class="text-blue-600 text-sm font-bold hover:underline">市場數據</button>
            <div id="tech2" class="hidden mt-4 text-xs bg-slate-50 p-4 rounded-lg">2035 年全球市場規模預計將突破 400 億美元。</div>
        </div>

        <div class="data-card p-8 reveal">
            <div class="text-orange-600 text-3xl mb-6"><i class="fas fa-boxes"></i></div>
            <h3 class="text-xl font-bold mb-4">3. 商業模式</h3>
            <p class="text-slate-500 text-sm mb-6">提供航空系統套件，包含儲存模組與燃料電池動力系統。</p>
            <button onclick="toggleInfo('tech3')" class="text-blue-600 text-sm font-bold hover:underline">執行計畫</button>
            <div id="tech3" class="hidden mt-4 text-xs bg-slate-50 p-4 rounded-lg">第一階段重組團隊；第二階段透過中國供應鏈實現產業化量產。</div>
        </div>
    </section>

    <section id="market" class="py-24 text-center px-6 reveal">
        <h2 class="text-3xl font-bold mb-8">準備好見證航空能源的未來了嗎？</h2>
        <button onclick="openModal()" class="bg-blue-600 hover:bg-blue-700 text-white text-lg px-12 py-4 rounded-full font-bold shadow-lg transition">我懂了</button>
    </section>

    <div id="modal" class="fixed inset-0 bg-slate-900/80 hidden items-center justify-center z-[100] p-4 backdrop-blur-sm">
        <div class="bg-white p-8 rounded-3xl max-w-lg w-full text-center border border-blue-500">
            <h4 class="text-2xl font-bold mb-4 text-blue-600">UH 核心策略</h4>
            <p class="text-slate-600 mb-8 text-left text-sm leading-relaxed">
                1. 專注於高增長的 eVTOL 市場，優先對接急需航程解決方案的廠商。<br>
                2. 利用中國成熟的液態氫儲罐製造與供應鏈能力進行量產。<br>
                3. 以已驗證的 TRL 6-7 技術作為核心競爭優勢。
            </p>
            <button onclick="closeModal()" class="w-full py-4 bg-slate-900 text-white rounded-xl font-bold">開啟合作討論</button>
        </div>
    </div>

    <script>
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => { if (entry.isIntersecting) entry.target.classList.add('active'); });
        }, { threshold: 0.1 });
        document.querySelectorAll('.reveal').forEach(el => observer.observe(el));
        function toggleInfo(id) { document.getElementById(id).classList.toggle('hidden'); }
        function openModal() { document.getElementById('modal').style.display = 'flex'; }
        function closeModal() { document.getElementById('modal').style.display = 'none'; }
    </script>
</body>
</html>
