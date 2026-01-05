[!DOCTYPE html.txt](https://github.com/user-attachments/files/24428762/DOCTYPE.html.txt)
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UH 2.0 | 氫能航空投資數據分析</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Noto+Sans+TC:wght@300;400;700&display=swap');
        
        body {
            font-family: 'Inter', 'Noto Sans TC', sans-serif;
            background-color: #f8fafc;
            color: #1e293b;
        }

        .hero-section {
            background: linear-gradient(135deg, #0f172a 0%, #1e40af 100%);
            color: white;
            padding: 80px 20px;
        }

        .data-card {
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1);
            transition: all 0.3s ease;
            border: 1px solid #e2e8f0;
        }

        .data-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1);
            border-color: #3b82f6;
        }

        .tag {
            background: #e0f2fe;
            color: #0369a1;
            padding: 2px 10px;
            border-radius: 9999px;
            font-size: 0.75rem;
            font-weight: 600;
        }

        .status-pulse {
            width: 8px;
            height: 8px;
            background: #10b981;
            border-radius: 50%;
            display: inline-block;
            margin-right: 8px;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(16, 185, 129, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 6px rgba(16, 185, 129, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(16, 185, 129, 0); }
        }

        .reveal { opacity: 0; transform: translateY(20px); transition: all 0.6s ease-out; }
        .reveal.active { opacity: 1; transform: translateY(0); }
    </style>
</head>
<body>

    <nav class="bg-white border-b border-slate-200 py-4 px-8 sticky top-0 z-50">
        <div class="max-w-7xl mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-4">
                <span class="text-2xl font-bold text-blue-600">IT 桔子 <span class="text-slate-400 font-light">| 項目詳解</span></span>
                <div class="hidden md:flex space-x-6 text-sm font-medium text-slate-600 ml-10">
                    <a href="#" class="hover:text-blue-600">首頁</a>
                    <a href="#" class="text-blue-600">投融資事件</a>
                    <a href="#" class="hover:text-blue-600">公司庫</a>
                </div>
            </div>
            <button class="bg-blue-600 text-white px-4 py-2 rounded text-sm font-bold">登入/註冊</button>
        </div>
    </nav>

    <header class="hero-section text-center">
        <div class="max-w-4xl mx-auto">
            <div class="inline-flex items-center bg-white/10 rounded-full px-4 py-1 mb-6">
                <span class="status-pulse"></span>
                <span class="text-sm font-medium">融資中：Universal Hydrogen 2.0 (UH 2.0)</span>
            </div>
            <h1 class="text-4xl md:text-6xl font-bold mb-6">液態氫航空系統：<br>重新定義 eVTOL 的航程極限</h1>
            <p class="text-blue-100 text-lg md:text-xl mb-10 max-w-2xl mx-auto font-light">
                我們提供 LH2 儲存與燃料電池動力系統，專為電動垂直起降飛行器（eVTOL）打造。
            </p>
            <div class="flex justify-center space-x-4">
                <div class="bg-white/20 p-4 rounded-xl backdrop-blur-md">
                    <div class="text-3xl font-bold">130k €</div>
                    <div class="text-xs text-blue-200">月度預算 (Phase 1)</div>
                </div>
                <div class="bg-white/20 p-4 rounded-xl backdrop-blur-md">
                    <div class="text-3xl font-bold">10+ 人</div>
                    <div class="text-xs text-blue-200">法國圖盧茲核心團隊</div>
                </div>
            </div>
        </div>
    </header>

    <main class="max-w-7xl mx-auto py-16 px-6">
        
        <div class="grid md:grid-cols-3 gap-8 mb-16">
            <div class="data-card p-8 reveal">
                <div class="flex justify-between items-start mb-6">
                    <div class="bg-blue-100 p-3 rounded-lg text-blue-600 text-2xl"><i class="fas fa-bolt"></i></div>
                    <span class="tag">能源密度優勢</span>
                </div>
                <h3 class="text-xl font-bold mb-3">為何選擇液態氫 (LH2)?</h3>
                <p class="text-slate-500 text-sm leading-relaxed">
                    電池太重，氣態氫體積太大 [cite: 7]。對 eVTOL 而言，僅需數十公斤 LH2 即可實現所需的任務續航 [cite: 8]。
                </p>
            </div>

            <div class="data-card p-8 reveal">
                <div class="flex justify-between items-start mb-6">
                    <div class="bg-emerald-100 p-3 rounded-lg text-emerald-600 text-2xl"><i class="fas fa-plane-departure"></i></div>
                    <span class="tag">已驗證 TRL 6-7</span>
                </div>
                <h3 class="text-xl font-bold mb-3">實證數據 (Proof of Work)</h3>
                <p class="text-slate-500 text-sm leading-relaxed">
                    曾在 Dash 8-300 改裝機上成功飛行測試 1 MW 氫電動力系統 [cite: 15, 17]，並驗證了模塊化低蒸發 LH2 儲存技術 [cite: 18]。
                </p>
            </div>

            <div class="data-card p-8 reveal">
                <div class="flex justify-between items-start mb-6">
                    <div class="bg-orange-100 p-3 rounded-lg text-orange-600 text-2xl"><i class="fas fa-industry"></i></div>
                    <span class="tag">中國供應鏈整合</span>
                </div>
                <h3 class="text-xl font-bold mb-3">產業化路徑</h3>
                <p class="text-slate-500 text-sm leading-relaxed">
                    將產品文檔轉移至中國進行量產 [cite: 35]。中國具備成熟的 LH2 低溫製造能力與靈活的燃料電池供應鏈 [cite: 36]。
                </p>
            </div>
        </div>

        <div class="bg-white rounded-2xl border border-slate-200 p-8 mb-16 reveal">
            <h2 class="text-2xl font-bold mb-8 flex items-center">
                <i class="fas fa-info-circle text-blue-600 mr-3"></i> 項目核心邏輯剖析
            </h2>
            <div class="space-y-4">
                <button onclick="toggleAccordion('acc1')" class="w-full text-left p-4 bg-slate-50 hover:bg-slate-100 rounded-xl transition flex justify-between items-center">
                    <span class="font-semibold text-slate-700">1. 過去失敗的教訓是什麼？(UH 1.0 vs 2.0)</span>
                    <i class="fas fa-chevron-down text-slate-400"></i>
                </button>
                <div id="acc1" class="hidden p-6 text-slate-600 text-sm border-l-4 border-blue-500">
                    過度擴張：舊計畫在缺乏資金的情況下挑戰大型客機（56-72 座）適航認證 [cite: 22]。<br>
                    <strong class="text-blue-600">UH 2.0 策略：</strong> 專注於高增長的 eVTOL 市場，且在獲得領頭客戶前絕不啟動漫長的認證路徑 [cite: 26, 44]。
                </div>

                <button onclick="toggleAccordion('acc2')" class="w-full text-left p-4 bg-slate-50 hover:bg-slate-100 rounded-xl transition flex justify-between items-center">
                    <span class="font-semibold text-slate-700">2. 中國市場的具體表現如何？</span>
                    <i class="fas fa-chevron-down text-slate-400"></i>
                </button>
                <div id="acc2" class="hidden p-6 text-slate-600 text-sm border-l-4 border-blue-500">
                    中國是 eVTOL 領導者，已有億航（EHang）獲得商業營運證書 [cite: 52]。<br>
                    以「京鴻」DF600 為例：1.2 噸起飛重量，單次加氫航程可達 800-1,000 公里 [cite: 57, 60]。
                </div>
            </div>
        </div>

        <div class="bg-blue-50 border-2 border-dashed border-blue-200 p-8 rounded-3xl mb-16 reveal">
            <div class="flex items-center space-x-4 mb-4">
                <div class="w-12 h-12 rounded-full bg-blue-500 flex items-center justify-center text-white"><i class="fas fa-lightbulb"></i></div>
                <h4 class="text-lg font-bold text-blue-800">平台建立者的小提醒</h4>
            </div>
            <p class="text-blue-700 leading-relaxed italic">
                「在向大中華區投資人展示時，別只強調技術指標。要強調我們在法國圖盧茲的團隊能如何對接中國的 OEM 廠商（如小鵬匯天、沃飛長空等）。投資人更在乎你的技術能不能在中國這片土地上『飛起來』並『省下錢』。」
            </p>
        </div>

        <div class="text-center py-12 reveal">
            <h2 class="text-3xl font-bold mb-6">掌握氫能航空的下一波紅利</h2>
            <p class="text-slate-500 mb-8 italic">2035 年全球市場規模預計將突破 400 億美元 [cite: 53]。</p>
            <button onclick="showFinalTip()" class="bg-blue-600 hover:bg-blue-700 text-white px-12 py-4 rounded-full font-bold shadow-xl transform transition hover:scale-105 active:scale-95">
                點擊獲取核心投資策略
            </button>
        </div>
    </main>

    <div id="modal" class="fixed inset-0 bg-black/60 hidden items-center justify-center z-[100] p-6 backdrop-blur-sm">
        <div class="bg-white p-10 rounded-3xl max-w-md w-full text-center">
            <div class="text-6xl mb-6">🚀</div>
            <h4 class="text-2xl font-bold mb-4">我懂了：核心商業模型</h4>
            <div class="text-left text-slate-600 mb-8 space-y-3">
                <p>1. <strong>Phase 1:</strong> 在圖盧茲重組核心團隊，準備工業化文檔 [cite: 28, 31]。</p>
                <p>2. <strong>Phase 2:</strong> 鎖定 1-2 個中國 eVTOL 平台，提供原型模組與集成支持 [cite: 48, 49]。</p>
                <p>3. <strong>核心目標:</strong> 成為 eVTOL 廠商的「一級供應商 (Tier 1)」，銷售儲罐、動力系統與售後服務 [cite: 38, 42]。</p>
            </div>
            <button onclick="closeModal()" class="w-full py-4 bg-slate-900 text-white rounded-2xl font-bold">開啟融資對接</button>
        </div>
    </div>

    <script>
        // 滾動顯示
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) entry.target.classList.add('active');
            });
        }, { threshold: 0.1 });
        document.querySelectorAll('.reveal').forEach(el => observer.observe(el));

        // 手風琴效果
        function toggleAccordion(id) {
            const el = document.getElementById(id);
            el.classList.toggle('hidden');
        }

        // 彈窗
        function showFinalTip() { document.getElementById('modal').style.display = 'flex'; }
        function closeModal() { document.getElementById('modal').style.display = 'none'; }
    </script>
</body>
</html>
