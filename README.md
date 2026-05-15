<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>王熙然 · 家长会要点 & 育儿指南</title>
    <style>
        :root {
            --primary: #4f46e5;
            --primary-light: #818cf8;
            --chinese: #ef4444;
            --math: #3b82f6;
            --sports: #10b981;
            --habit: #8b5cf6;
            --growth: #f59e0b;
            --family: #14b8a6;
            --bg: #f8fafc;
            --card-bg: #ffffff;
            --text: #1e293b;
            --text-secondary: #64748b;
            --border: #e2e8f0;
            --shadow: 0 4px 6px -1px rgba(0,0,0,0.1), 0 2px 4px -2px rgba(0,0,0,0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            font-family: 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', -apple-system, sans-serif;
            background: var(--bg);
            min-height: 100vh;
            color: var(--text);
            line-height: 1.6;
            -webkit-text-size-adjust: 100%;
        }

        /* 头部 */
        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 32px 20px;
            text-align: center;
        }

        .header h1 {
            font-size: 24px;
            font-weight: 800;
            margin-bottom: 6px;
        }

        .header .subtitle {
            font-size: 14px;
            opacity: 0.9;
            margin-bottom: 8px;
        }

        .header .date-badge {
            display: inline-block;
            background: rgba(255,255,255,0.2);
            padding: 4px 14px;
            border-radius: 20px;
            font-size: 12px;
        }

        /* 导航 */
        .nav-tabs {
            display: flex;
            gap: 8px;
            padding: 16px;
            background: white;
            position: sticky;
            top: 0;
            z-index: 50;
            box-shadow: var(--shadow);
        }

        .nav-tab {
            flex: 1;
            padding: 10px;
            border-radius: 10px;
            text-align: center;
            font-size: 14px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.2s;
            border: 2px solid var(--border);
            color: var(--text-secondary);
            background: white;
        }

        .nav-tab.active {
            background: var(--primary);
            color: white;
            border-color: var(--primary);
            box-shadow: 0 4px 12px rgba(79,70,229,0.3);
        }

        .nav-tab .emoji {
            display: block;
            font-size: 20px;
            margin-bottom: 2px;
        }

        /* 内容区 */
        .content-section {
            display: none;
            padding: 0 16px 100px;
        }

        .content-section.active {
            display: block;
            animation: fadeIn 0.3s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(8px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* 卡片 */
        .card {
            background: var(--card-bg);
            border-radius: 16px;
            margin-bottom: 16px;
            box-shadow: var(--shadow);
            overflow: hidden;
            border: 1px solid var(--border);
        }

        .card-header {
            padding: 16px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            cursor: pointer;
            user-select: none;
            transition: background 0.2s;
        }

        .card-header:hover {
            background: #f8fafc;
        }

        .card-header-left {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .card-icon {
            width: 40px;
            height: 40px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 22px;
        }

        .card-title {
            font-size: 17px;
            font-weight: 700;
        }

        .card-badge {
            font-size: 11px;
            padding: 3px 10px;
            border-radius: 20px;
            font-weight: 600;
        }

        .card-toggle {
            font-size: 18px;
            color: var(--text-secondary);
            transition: transform 0.3s;
        }

        .card.expanded .card-toggle {
            transform: rotate(180deg);
        }

        .card-body {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease, padding 0.4s ease;
        }

        .card.expanded .card-body {
            max-height: 3000px;
            padding: 0 16px 16px;
        }

        /* 列表项 */
        .item {
            padding: 10px 0;
            border-bottom: 1px dashed var(--border);
            display: flex;
            gap: 10px;
            align-items: flex-start;
        }

        .item:last-child {
            border-bottom: none;
        }

        .item-dot {
            width: 6px;
            height: 6px;
            border-radius: 50%;
            margin-top: 8px;
            flex-shrink: 0;
        }

        .item-content {
            flex: 1;
            font-size: 14px;
            line-height: 1.7;
            color: var(--text);
        }

        /* 重点框 */
        .highlight-box {
            border-radius: 10px;
            padding: 12px 14px;
            margin: 10px 0;
            font-size: 14px;
            line-height: 1.6;
        }

        .highlight-box.red {
            background: #fef2f2;
            border-left: 3px solid var(--chinese);
            color: #991b1b;
        }

        .highlight-box.yellow {
            background: #fefce8;
            border-left: 3px solid #eab308;
            color: #854d0e;
        }

        .highlight-box.blue {
            background: #eff6ff;
            border-left: 3px solid var(--math);
            color: #1e40af;
        }

        .highlight-box.green {
            background: #f0fdf4;
            border-left: 3px solid var(--sports);
            color: #166534;
        }

        /* 标签 */
        .tag {
            display: inline-block;
            padding: 2px 8px;
            border-radius: 6px;
            font-size: 11px;
            font-weight: 600;
            margin-right: 4px;
        }

        .tag-red { background: #fee2e2; color: #991b1b; }
        .tag-yellow { background: #fef9c3; color: #854d0e; }
        .tag-blue { background: #dbeafe; color: #1e40af; }
        .tag-green { background: #dcfce7; color: #166534; }

        /* 步骤 */
        .steps {
            background: #f8fafc;
            border-radius: 10px;
            padding: 12px;
            margin: 8px 0;
        }

        .step {
            display: flex;
            gap: 10px;
            margin-bottom: 8px;
            align-items: flex-start;
        }

        .step:last-child {
            margin-bottom: 0;
        }

        .step-num {
            width: 22px;
            height: 22px;
            border-radius: 50%;
            background: var(--primary);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 11px;
            font-weight: 700;
            flex-shrink: 0;
        }

        .step-text {
            font-size: 13px;
            line-height: 1.6;
            padding-top: 2px;
        }

        /* 小标题 */
        .sub-title {
            font-size: 13px;
            font-weight: 700;
            color: var(--text);
            margin: 14px 0 8px;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        /* 年级按钮 */
        .grade-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin: 12px 0;
        }

        .grade-btn {
            display: inline-block;
            padding: 6px 12px;
            background: #fee2e2;
            color: #991b1b;
            border-radius: 8px;
            font-size: 12px;
            font-weight: 600;
            cursor: pointer;
            border: none;
        }

        /* 底部按钮 */
        .footer-actions {
            display: flex;
            gap: 10px;
            margin-top: 20px;
            padding: 0 16px;
        }

        .btn {
            flex: 1;
            padding: 14px;
            border-radius: 12px;
            border: none;
            font-size: 14px;
            font-weight: 600;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 6px;
            transition: all 0.2s;
        }

        .btn-primary {
            background: var(--primary);
            color: white;
            box-shadow: 0 4px 12px rgba(79,70,229,0.3);
        }

        .btn-primary:active {
            transform: scale(0.98);
        }

        .btn-secondary {
            background: white;
            color: var(--text);
            border: 2px solid var(--border);
        }

        /* Toast */
        .toast {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: rgba(0,0,0,0.8);
            color: white;
            padding: 14px 28px;
            border-radius: 12px;
            font-size: 14px;
            z-index: 1000;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.3s;
        }

        .toast.show {
            opacity: 1;
        }

        /* 图片弹窗 */
        .image-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.92);
            z-index: 1000;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            padding: 20px;
        }

        .image-modal.active {
            display: flex;
        }

        .image-modal img {
            max-width: 100%;
            max-height: 80vh;
            width: auto;
            height: auto;
            object-fit: contain;
            border-radius: 8px;
        }

        .image-modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255,255,255,0.2);
            color: white;
            border: none;
            font-size: 20px;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .image-modal-title {
            color: white;
            font-size: 13px;
            margin-bottom: 10px;
            opacity: 0.7;
        }

        /* 侧边导航 */
        .sidebar-nav {
            position: fixed;
            right: 16px;
            bottom: 100px;
            z-index: 100;
            display: flex;
            flex-direction: column;
            align-items: flex-end;
            gap: 8px;
        }

        .menu-fab {
            width: 52px;
            height: 52px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            font-size: 20px;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(102,126,234,0.4);
            display: flex;
            align-items: center;
            justify-content: center;
            transition: transform 0.3s;
        }

        .menu-fab.active {
            transform: rotate(45deg);
        }

        .menu-items {
            display: none;
            flex-direction: column;
            gap: 6px;
            margin-bottom: 8px;
        }

        .menu-items.show {
            display: flex;
            animation: popUp 0.3s ease;
        }

        @keyframes popUp {
            from { opacity: 0; transform: scale(0.8) translateY(10px); }
            to { opacity: 1; transform: scale(1) translateY(0); }
        }

        .menu-item {
            background: white;
            padding: 8px 14px;
            border-radius: 20px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.15);
            font-size: 13px;
            font-weight: 600;
            color: var(--text);
            white-space: nowrap;
            border: none;
            cursor: pointer;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        /* 主题色 */
        .theme-chinese .card-header { border-left: 4px solid var(--chinese); }
        .theme-chinese .card-icon { background: #fee2e2; }
        .theme-chinese .item-dot { background: var(--chinese); }

        .theme-math .card-header { border-left: 4px solid var(--math); }
        .theme-math .card-icon { background: #dbeafe; }
        .theme-math .item-dot { background: var(--math); }

        .theme-sports .card-header { border-left: 4px solid var(--sports); }
        .theme-sports .card-icon { background: #dcfce7; }
        .theme-sports .item-dot { background: var(--sports); }

        .theme-habit .card-header { border-left: 4px solid var(--habit); }
        .theme-habit .card-icon { background: #ede9fe; }
        .theme-habit .item-dot { background: var(--habit); }

        .theme-growth .card-header { border-left: 4px solid var(--growth); }
        .theme-growth .card-icon { background: #fef3c7; }
        .theme-growth .item-dot { background: var(--growth); }

        .theme-family .card-header { border-left: 4px solid var(--family); }
        .theme-family .card-icon { background: #ccfbf1; }
        .theme-family .item-dot { background: var(--family); }

        /* 响应式 */
        @media (max-width: 480px) {
            .header h1 { font-size: 20px; }
            .header { padding: 24px 16px; }
            .nav-tab { font-size: 12px; padding: 8px 4px; }
            .card-title { font-size: 15px; }
            .item-content { font-size: 13px; }
            .sidebar-nav { right: 12px; bottom: 80px; }
            .menu-fab { width: 48px; height: 48px; }
        }

        /* 防止溢出 */
        html, body { overflow-x: hidden; }
        img { max-width: 100%; height: auto; }
    </style>
<base target="_blank">
</head>
<body>

    <!-- 头部 -->
    <div class="header">
        <h1>📋 王熙然 · 家长会要点</h1>
        <div class="subtitle">一年级下学期 · 家校共育指南</div>
        <div class="date-badge">📅 2026年5月 更新 · 创建于 2025年10月育儿课</div>
    </div>

    <!-- 导航 -->
    <div class="nav-tabs">
        <div class="nav-tab active" onclick="switchTab('subjects')">
            <span class="emoji">📚</span>
            学科要点
        </div>
        <div class="nav-tab" onclick="switchTab('parenting')">
            <span class="emoji">🏠</span>
            育儿指南
        </div>
        <div class="nav-tab" onclick="switchTab('all')">
            <span class="emoji">📋</span>
            全部内容
        </div>
    </div>

    <!-- 学科要点 -->
    <div id="subjects" class="content-section active">

        <!-- 语文 -->
        <div class="card theme-chinese expanded" id="card-chinese">
            <div class="card-header" onclick="toggleCard('card-chinese')">
                <div class="card-header-left">
                    <div class="card-icon">📖</div>
                    <div class="card-title">语文</div>
                </div>
                <div style="display:flex;align-items:center;gap:8px;">
                    <span class="card-badge" style="background:#fee2e2;color:#991b1b;">重点</span>
                    <span class="card-toggle">▼</span>
                </div>
            </div>
            <div class="card-body">


                    <div class="highlight-box">
                        <strong>🌟 王熙然表现优秀：</strong>早读认真奖、眼保健操认真奖、护脊操认真奖、午餐打扫认真奖
                    </div>

                    <div class="sub-title">📌 识字 & 写字</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <span class="tag tag-green">表扬</span> 课作本认真独立完成
                        </div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <span class="tag tag-green">表扬</span> 写字AB本结构掌握好，认真独立完成
                        </div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <span class="tag tag-green">表扬</span> 听写优秀
                        </div>
                    </div>

                    <div class="sub-title">📌 阅读理解（四步法）</div>
                    <div class="steps">
                        <div class="step">
                            <div class="step-num">1</div>
                            <div class="step-text"><strong>指读全文</strong> — 用手指着逐字阅读</div>
                        </div>
                        <div class="step">
                            <div class="step-num">2</div>
                            <div class="step-text"><strong>寻找答案</strong> — 在文中标记线索位置</div>
                        </div>
                        <div class="step">
                            <div class="step-num">3</div>
                            <div class="step-text"><strong>组织语言</strong> — 用自己的话写出答案</div>
                        </div>
                        <div class="step">
                            <div class="step-num">4</div>
                            <div class="step-text"><strong>检查答案</strong> — 是否通顺、准确</div>
                        </div>
                    </div>

                    <div class="sub-title">📌 写作培养</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">句式练习、仿写训练</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">看图写话：注意<strong>环境描写</strong>、<strong>细节观察</strong>，思考图画意思</div>
                    </div>

                    <div class="sub-title">📌 听讲与发言</div>
                    <div class="highlight-box green">
                        👍 王熙然积极发言、认真听讲，继续保持！
                    </div>

                    <div class="sub-title">📌 科创活动</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <span class="tag tag-yellow">推荐参加</span> <strong>AI配音师</strong> — 无人数限制，建议大家参加
                        </div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <span class="tag tag-blue">有难度</span> 天文竞赛（限制人数）
                        </div>
                    </div>

                    <div class="sub-title">📌 运动会</div>
                    <div class="highlight-box blue">
                        🏆 今年班级总分第一名！
                    </div>

                
            </div>
        </div>

        <!-- 数学 -->
        <div class="card theme-math" id="card-math">
            <div class="card-header" onclick="toggleCard('card-math')">
                <div class="card-header-left">
                    <div class="card-icon">🔢</div>
                    <div class="card-title">数学</div>
                </div>
                <div style="display:flex;align-items:center;gap:8px;">
                    <span class="card-badge" style="background:#dbeafe;color:#1e40af;">重点</span>
                    <span class="card-toggle">▼</span>
                </div>
            </div>
            <div class="card-body">


                    <div class="highlight-box">
                        <strong>⚠️ 当前挑战：</strong>题干变长，需要加强阅读理解能力；应用题涉及人民币购物等生活场景
                    </div>

                    <div class="sub-title">📌 学习重点</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>理解</strong> — 语文基础影响数学题理解</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>应用</strong> — 人民币购物等生活场景题</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>阅读</strong> — 题干变长，学会<strong>找关键词</strong></div>
                    </div>

                    <div class="sub-title">📌 读题规范（三步法）</div>
                    <div class="steps">
                        <div class="step">
                            <div class="step-num">1</div>
                            <div class="step-text"><strong>指读</strong> — 手指指着题目逐字读</div>
                        </div>
                        <div class="step">
                            <div class="step-num">2</div>
                            <div class="step-text"><strong>圈关键词</strong> — 圈出数字、单位、关键条件</div>
                        </div>
                        <div class="step">
                            <div class="step-num">3</div>
                            <div class="step-text"><strong>速读检查</strong> — 快速再读一遍确认</div>
                        </div>
                    </div>

                    <div class="sub-title">📌 做题习惯</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">按顺序做题，<strong>不会的做标记</strong>，做完再回头</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">做完<strong>及时检查</strong>，培养自己找错的能力</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">练坐姿，鼓励课上积极发言</div>
                    </div>

                    <div class="sub-title">📌 书写 & 收纳</div>
                    <div class="highlight-box green">
                        <span class="tag tag-green">表扬</span> 王熙然书写获得表扬！
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">文件袋管理：要交的、未订正的放文件袋；已订正的放家里</div>
                    </div>

                    <div class="sub-title">📌 口算 & 错题</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">坚持口算练习，提升计算能力</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>错题整理</strong> — 建立错题本，定期复习</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">培养<strong>独立思考</strong>，作业检查时先让孩子自己找错</div>
                    </div>

                    <div class="sub-title">📌 推荐资源</div>
                    <div class="highlight-box blue">
                        📱 <strong><a href="https://www.zxx.edu.cn/" target="_blank" style="color:#2b6cb0;text-decoration:underline;">国家中小学智慧教育平台</a></strong> — 官方免费学习资源，点击直达 ↗
                    </div>

                
            </div>
        </div>

        <!-- 体育 -->
        <div class="card theme-sports" id="card-sports">
            <div class="card-header" onclick="toggleCard('card-sports')">
                <div class="card-header-left">
                    <div class="card-icon">🏃</div>
                    <div class="card-title">体育</div>
                </div>
                <div style="display:flex;align-items:center;gap:8px;">
                    <span class="card-badge" style="background:#fee2e2;color:#991b1b;">重要</span>
                    <span class="card-toggle">▼</span>
                </div>
            </div>
            <div class="card-body">


                    <div class="highlight-box">
                        <strong>🚨 健康预警：</strong>三年级以前是控制体重的关键期，肥胖和脊柱侧弯要及早干预！
                    </div>

                    <div class="sub-title">📌 体能测试项目（杭州市小学女生标准）</div>
                    <div style="display:flex;flex-wrap:wrap;gap:8px;margin:12px 0;">
                        <a href="一年级.jpg" onclick="openImageModal(this.href);return false;" style="text-decoration:none;">
                            <span style="display:inline-block;padding:6px 14px;background:#fed7d7;color:#c53030;border-radius:10px;font-size:13px;font-weight:600;">🖼️ 一年级标准</span>
                        </a>
                        <a href="二年级.jpg" onclick="openImageModal(this.href);return false;" style="text-decoration:none;">
                            <span style="display:inline-block;padding:6px 14px;background:#fed7d7;color:#c53030;border-radius:10px;font-size:13px;font-weight:600;">🖼️ 二年级标准</span>
                        </a>
                        <a href="三年级.jpg" onclick="openImageModal(this.href);return false;" style="text-decoration:none;">
                            <span style="display:inline-block;padding:6px 14px;background:#fed7d7;color:#c53030;border-radius:10px;font-size:13px;font-weight:600;">🖼️ 三年级标准</span>
                        </a>
                        <a href="四年级.jpg" onclick="openImageModal(this.href);return false;" style="text-decoration:none;">
                            <span style="display:inline-block;padding:6px 14px;background:#fed7d7;color:#c53030;border-radius:10px;font-size:13px;font-weight:600;">🖼️ 四年级标准</span>
                        </a>
                        <a href="五年级.jpg" onclick="openImageModal(this.href);return false;" style="text-decoration:none;">
                            <span style="display:inline-block;padding:6px 14px;background:#fed7d7;color:#c53030;border-radius:10px;font-size:13px;font-weight:600;">🖼️ 五年级标准</span>
                        </a>
                        <a href="六年级.jpg" onclick="openImageModal(this.href);return false;" style="text-decoration:none;">
                            <span style="display:inline-block;padding:6px 14px;background:#fed7d7;color:#c53030;border-radius:10px;font-size:13px;font-weight:600;">🖼️ 六年级标准</span>
                        </a>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <strong>1分钟跳绳</strong> <span class="tag tag-yellow">及格/满分</span><br>
                            <span style="color:#c53030;font-weight:600;">143个 / 157个</span>
                        </div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <strong>坐位体前屈</strong> <span class="tag tag-yellow">及格/满分</span><br>
                            <span style="color:#c53030;font-weight:600;">16cm / 18.6cm</span>
                        </div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <strong>50米跑</strong> <span class="tag tag-yellow">及格/满分</span><br>
                            <span style="color:#c53030;font-weight:600;">11.2秒 / 11.0秒</span>
                        </div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">
                            <strong>肺活量</strong> <span class="tag tag-yellow">及格/满分</span><br>
                            <span style="color:#c53030;font-weight:600;">1200ml / 1400ml</span>
                        </div>
                    </div>

                    <div class="sub-title">📌 锻炼项目（趣味比赛形式）</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>30分钟趣味比赛</strong> — 跳绳轮流跳、坐位体前屈轮流尝试、50米跑轮流跑、肺活量轮流吹，然后大家比一比</div>
                    </div>

                    <div class="sub-title">📌 健康关注</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><span class="tag tag-red">重点关注</span> <strong>超重问题</strong> — 三年级前把肥胖扼杀在摇篮里</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><span class="tag tag-red">重点关注</span> <strong>脊柱侧弯</strong> — 注意坐姿和体态</div>
                    </div>

                    <div class="sub-title">📌 心理品质培养</div>
                    <div class="highlight-box green">
                        💪 培养<strong>抗挫折能力</strong>、<strong>抗压能力</strong>和<strong>坚持精神</strong>
                    </div>

                    <div class="sub-title">📌 家庭配合</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">每天保证运动时间，<strong>跳绳要考试</strong>（目标157个满分），需坚持练习</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">注意孩子坐姿、站姿，预防脊柱侧弯</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">控制体重，合理饮食+运动</div>
                    </div>

                
            </div>
        </div>

    </div>

    <!-- 育儿指南 -->
    <div id="parenting" class="content-section">

        <!-- 习惯培养 -->
        <div class="card theme-habit expanded" id="card-habit">
            <div class="card-header" onclick="toggleCard('card-habit')">
                <div class="card-header-left">
                    <div class="card-icon">🎯</div>
                    <div class="card-title">习惯培养</div>
                </div>
                <div style="display:flex;align-items:center;gap:8px;">
                    <span class="card-badge" style="background:#ede9fe;color:#6b21a8;">核心</span>
                    <span class="card-toggle">▼</span>
                </div>
            </div>
            <div class="card-body">


                    <div class="sub-title">📌 自理能力</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>自己整理书包</strong> 🎒 — 家长不要包办</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>自己穿衣吃饭收拾</strong> — 自我服务能力</div>
                    </div>

                    <div class="sub-title">📌 时间观念</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">做事不拖拉，吃饭控制在 <strong>20-30分钟</strong></div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">放钟表计时 ⏰，让小朋友看懂时间</div>
                    </div>
                    <div class="highlight-box yellow">
                        <strong>⚠️ 切忌催促：</strong>不要说"快点""还有几分钟"，让小朋友自己感受时间
                    </div>

                    <div class="sub-title">📌 专注力保护</div>
                    <div class="highlight-box red">
                        <strong>👓 专注做事时不要打扰！</strong><br>
                        尤其老人避免问："饿不饿？渴不渴？吃不吃水果？"
                    </div>

                    <div class="sub-title">📌 阅读培养</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>每天阅读20分钟</strong> 📚 — 非常重要！</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>家长带指读</strong> 👀 — 带动小朋友注意力，而不是家长读孩子听</div>
                    </div>
                    <div class="highlight-box blue">
                        如果小朋友已经自己阅读，<strong>不要在旁边盯着</strong>，给孩子独立空间
                    </div>

                    <div class="sub-title">📌 运动 & 作息</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>每天运动</strong> 🏃 — 喜欢的运动都可以，跳绳要考试</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>按时睡觉 🛏 · 按时起床 ☀</strong> — 规律作息</div>
                    </div>

                    <div class="sub-title">📌 家务劳动</div>
                    <div class="highlight-box green">
                        <strong>🧹 非常建议让小朋友承担一项固定家务！</strong><br>
                        例如：分碗筷 🍚、倒垃圾 🚮<br>
                        培养自理能力、服务意识、责任心
                    </div>

                
            </div>
        </div>

        <!-- 能力培养 -->
        <div class="card theme-growth" id="card-growth">
            <div class="card-header" onclick="toggleCard('card-growth')">
                <div class="card-header-left">
                    <div class="card-icon">🌱</div>
                    <div class="card-title">能力培养</div>
                </div>
                <div style="display:flex;align-items:center;gap:8px;">
                    <span class="card-badge" style="background:#ede9fe;color:#6b21a8;">核心</span>
                    <span class="card-toggle">▼</span>
                </div>
            </div>
            <div class="card-body">


                    <div class="sub-title">📌 表达能力</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content">在外玩时 🧑‍🤝‍🧑，<strong>家长离远一点</strong>，让小朋友自己独立交往</div>
                    </div>

                    <div class="sub-title">📌 情绪控制</div>
                    <div class="highlight-box red">
                        <strong>😠 发脾气时：</strong>家长不要被拿捏，<strong>不要让小朋友得逞</strong>。坚持原则，不被情绪绑架。
                    </div>

                    <div class="sub-title">📌 自我保护</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>相信孩子，放手尝试</strong> — 教正确的做法，而不是一味禁止</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>应急处理，指导演练</strong> — 例如：困在电梯、建筑安全通道、汽车应急门、落水急救</div>
                    </div>

                    <div class="sub-title">📌 正确自我定位</div>
                    <div class="highlight-box blue">
                        <strong>家长：</strong>注重习惯培养，<strong>而非盯着成绩</strong>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>学习是我的事情</strong>，我会变得越来越好 — 自我认可</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>能输能赢</strong>，不要盯着别人 — 看自己，有自己的擅长和缺点</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>承认别人的优秀</strong>，看清自己的不足，积极改进，勇敢接受</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>悲悯情怀</strong> — 善待他人、善待动物、感恩长辈</div>
                    </div>

                
            </div>
        </div>

        <!-- 家庭关系 -->
        <div class="card theme-family" id="card-family">
            <div class="card-header" onclick="toggleCard('card-family')">
                <div class="card-header-left">
                    <div class="card-icon">💑</div>
                    <div class="card-title">家庭关系</div>
                </div>
                <div style="display:flex;align-items:center;gap:8px;">
                    <span class="card-badge" style="background:#dcfce7;color:#166534;">重要</span>
                    <span class="card-toggle">▼</span>
                </div>
            </div>
            <div class="card-body">


                    <div class="highlight-box">
                        <strong>💑 夫妻关系好，亲子关系才会好</strong><br>
                        孩子有眼睛 👀 会学习模仿父母的相处方式
                    </div>

                    <div class="sub-title">📌 日常经营</div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>常陪伴，每天沟通</strong> — 储蓄感情，为青春期做准备</div>
                    </div>
                    <div class="item">
                        <div class="item-dot"></div>
                        <div class="item-content"><strong>不骄纵，眼中有人</strong> — 遵守规则，尊重他人</div>
                    </div>

                
            </div>
        </div>

    </div>

    <!-- 全部内容 -->
    <div id="all" class="content-section">
        <div style="text-align:center;color:var(--text-secondary);margin-bottom:16px;font-size:13px;">
            以下为全部内容汇总，可点击卡片展开查看
        </div>
        <div id="all-content-area"></div>
    </div>

    <!-- 底部按钮 -->
    <div class="footer-actions">
        <button class="btn btn-primary" onclick="copyAll()">
            📋 复制全部要点
        </button>
        <button class="btn btn-secondary" id="expandAllBtn" onclick="toggleExpandAll()">
            🔽 展开全部
        </button>
    </div>

    <!-- 侧边浮动导航 -->
    <div class="sidebar-nav">
        <div class="menu-items" id="menuItems">
            <button class="menu-item" onclick="jumpToSection('subjects', 'card-chinese')">📖 语文</button>
            <button class="menu-item" onclick="jumpToSection('subjects', 'card-math')">🔢 数学</button>
            <button class="menu-item" onclick="jumpToSection('subjects', 'card-sports')">🏃 体育</button>
            <button class="menu-item" onclick="jumpToSection('parenting', 'card-habit')">🎯 习惯</button>
            <button class="menu-item" onclick="jumpToSection('parenting', 'card-growth')">🌱 能力</button>
            <button class="menu-item" onclick="jumpToSection('parenting', 'card-family')">💑 家庭</button>
        </div>
        <button class="menu-fab" id="menuFab" onclick="toggleMenu()">☰</button>
    </div>

    <!-- Toast -->
    <div class="toast" id="toast"></div>

    <!-- 图片弹窗 -->
    <div class="image-modal" id="imageModal" onclick="closeImageModal(event)">
        <button class="image-modal-close" onclick="closeImageModal(event)">✕</button>
        <div class="image-modal-title">点击任意位置关闭</div>
        <img src="" alt="体测标准" id="imageModalImg">
    </div>

    <script>
        // 悬浮菜单切换
        function toggleMenu() {
            const items = document.getElementById('menuItems');
            const fab = document.getElementById('menuFab');
            items.classList.toggle('show');
            fab.classList.toggle('active');
        }

        // 图片弹窗功能
        function openImageModal(src) {
            const modal = document.getElementById('imageModal');
            const img = document.getElementById('imageModalImg');
            img.src = src;
            modal.classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        function closeImageModal(event) {
            if (event.target.id === 'imageModal' || event.target.classList.contains('image-modal-close')) {
                const modal = document.getElementById('imageModal');
                modal.classList.remove('active');
                document.body.style.overflow = '';
            }
        }

        // 防止滚动监听覆盖点击高亮的标志
        let isClickJumping = false;
        let clickJumpTimer = null;

        // 跳转到指定板块并展开卡片
        function jumpToSection(tabId, cardId) {
            // 重置展开/收起按钮状态
            const btn = document.getElementById('expandAllBtn');
            if (btn) {
                btn.innerHTML = '🔽 展开全部';
                isAllExpanded = false;
            }

            // 设置标志，防止滚动监听覆盖点击高亮
            isClickJumping = true;
            clearTimeout(clickJumpTimer);

            // 切换标签页
            document.querySelectorAll('.nav-tab').forEach(t => t.classList.remove('active'));
            document.querySelectorAll('.nav-tab').forEach(t => {
                if (t.getAttribute('onclick') && t.getAttribute('onclick').includes("'" + tabId + "'")) {
                    t.classList.add('active');
                }
            });

            // 显示对应内容区
            document.querySelectorAll('.content-section').forEach(s => s.classList.remove('active'));
            document.getElementById(tabId).classList.add('active');

            // 如果是"全部"标签，需要重建内容
            if (tabId === 'all') {
                const area = document.getElementById('all-content-area');
                area.innerHTML = '';
                document.querySelectorAll('#subjects .card, #parenting .card').forEach(card => {
                    const clone = card.cloneNode(true);
                    clone.id = clone.id + '-all';
                    clone.classList.remove('expanded');
                    area.appendChild(clone);
                });
            }

            // 高亮当前侧边栏项（立即执行，不等待滚动）
            highlightSidebarItem(cardId);

            // 展开目标卡片并滚动
            setTimeout(() => {
                const targetCard = document.getElementById(cardId);
                if (targetCard) {
                    targetCard.classList.add('expanded');
                    targetCard.scrollIntoView({ behavior: 'smooth', block: 'center' });
                }
            }, 100);

            // 1.5秒后恢复滚动监听
            clickJumpTimer = setTimeout(() => {
                isClickJumping = false;
            }, 1500);
        }

        // 高亮侧边栏指定项
        function highlightSidebarItem(cardId) {
            document.querySelectorAll('.sidebar-item').forEach(item => item.classList.remove('active'));
            const map = {
                'card-chinese': 'chinese',
                'card-math': 'math', 
                'card-sports': 'sports',
                'card-habit': 'habit',
                'card-growth': 'growth',
                'card-family': 'family'
            };
            const activeClass = map[cardId];
            if (activeClass) {
                document.querySelectorAll('.sidebar-item.' + activeClass).forEach(item => item.classList.add('active'));
            }
        }

        // 收起/展开侧边栏
        function toggleSidebar() {
            const sidebar = document.getElementById('sidebarNav');
            const container = document.querySelector('.container');

            // 检测是否为手机端（通过窗口宽度）
            if (window.innerWidth <= 768) {
                // 手机端：切换 mobile-collapsed 类
                sidebar.classList.toggle('mobile-collapsed');
                container.classList.toggle('mobile-nav-collapsed');
            } else {
                // 桌面端：切换 collapsed/expanded
                sidebar.classList.toggle('collapsed');
                sidebar.classList.toggle('expanded');
            }
        }

        // 滚动时更新侧边栏高亮
        function updateActiveOnScroll() {
            // 如果正在执行点击跳转，不更新高亮
            if (isClickJumping) return;

            // 获取当前激活的标签页
            const activeSection = document.querySelector('.content-section.active');
            if (!activeSection) return;

            const sectionId = activeSection.id;

            // 根据当前标签页确定要查找的卡片
            let cardsToCheck = [];
            if (sectionId === 'subjects') {
                cardsToCheck = ['card-chinese', 'card-math', 'card-sports'];
            } else if (sectionId === 'parenting') {
                cardsToCheck = ['card-habit', 'card-growth', 'card-family'];
            } else if (sectionId === 'all') {
                cardsToCheck = ['card-chinese-all', 'card-math-all', 'card-sports-all', 'card-habit-all', 'card-growth-all', 'card-family-all'];
            }

            const map = {
                'card-chinese': 'chinese',
                'card-math': 'math',
                'card-sports': 'sports',
                'card-chinese-all': 'chinese',
                'card-math-all': 'math',
                'card-sports-all': 'sports',
                'card-habit': 'habit',
                'card-growth': 'growth',
                'card-family': 'family',
                'card-habit-all': 'habit',
                'card-growth-all': 'growth',
                'card-family-all': 'family'
            };

            let current = null;
            let maxVisibleTop = -Infinity;

            for (const cardId of cardsToCheck) {
                const card = document.getElementById(cardId);
                if (card) {
                    const rect = card.getBoundingClientRect();
                    // 卡片必须在视口内（顶部在屏幕下方一半位置以上，底部在屏幕上方以上）
                    if (rect.top < window.innerHeight * 0.6 && rect.bottom > 0) {
                        // 选择最靠近视口顶部的卡片（top值最大的）
                        if (rect.top > maxVisibleTop) {
                            maxVisibleTop = rect.top;
                            current = cardId;
                        }
                    }
                }
            }

            if (current) {
                document.querySelectorAll('.sidebar-item').forEach(item => item.classList.remove('active'));
                const activeClass = map[current];
                if (activeClass) {
                    document.querySelectorAll('.sidebar-item.' + activeClass).forEach(item => item.classList.add('active'));
                }
            }
        }

        window.addEventListener('scroll', updateActiveOnScroll);

        // 切换标签
        function switchTab(tabId) {
            document.querySelectorAll('.nav-tab').forEach(t => t.classList.remove('active'));
            event.target.closest('.nav-tab').classList.add('active');

            document.querySelectorAll('.content-section').forEach(s => s.classList.remove('active'));
            document.getElementById(tabId).classList.add('active');

            // 切换标签时重置展开/收起按钮状态
            const btn = document.getElementById('expandAllBtn');
            if (btn) {
                btn.innerHTML = '🔽 展开全部';
                isAllExpanded = false;
            }

            // 如果是全部标签，复制内容并重新绑定事件
            if (tabId === 'all') {
                const area = document.getElementById('all-content-area');
                area.innerHTML = '';
                document.querySelectorAll('#subjects .card, #parenting .card').forEach((card, index) => {
                    const clone = card.cloneNode(true);
                    const newId = card.id + '-all';
                    clone.id = newId;
                    clone.classList.remove('expanded');

                    // 重新绑定卡片点击事件
                    const header = clone.querySelector('.card-header');
                    if (header) {
                        header.onclick = function() {
                            toggleCard(newId);
                        };
                    }

                    area.appendChild(clone);
                });
            }
        }

        // 折叠/展开卡片
        function toggleCard(cardId) {
            const card = document.getElementById(cardId);
            card.classList.toggle('expanded');
        }

        // 展开/收起全部切换
        let isAllExpanded = false;

        function toggleExpandAll() {
            const btn = document.getElementById('expandAllBtn');
            const activeCards = document.querySelectorAll('.content-section.active .card');

            if (!isAllExpanded) {
                // 展开全部
                activeCards.forEach(card => {
                    card.classList.add('expanded');
                });
                btn.innerHTML = '🔼 收起全部';
                isAllExpanded = true;
                showToast('已展开全部内容');
            } else {
                // 收起全部
                activeCards.forEach(card => {
                    card.classList.remove('expanded');
                });
                btn.innerHTML = '🔽 展开全部';
                isAllExpanded = false;
                showToast('已收起全部内容');
            }
        }

        // 兼容旧函数名
        function expandAll() {
            toggleExpandAll();
        }

        // 复制全部
        function copyAll() {
            let text = '📋 王熙然家长会要点\n';
            text += '==================\n\n';

            // 语文
            text += '📖 【语文】\n';
            text += '✅ 王熙然表现：早读认真奖、眼保健操认真奖、护脊操认真奖、午餐打扫认真奖\n';
            text += '📝 识字写字：课作本、写字AB本认真独立完成，听写优秀\n';
            text += '📖 阅读理解四步法：①指读全文 → ②寻找答案标记线索 → ③组织语言写答案 → ④检查通顺准确\n';
            text += '✍️ 写作：句式、仿写、看图写话（环境、细节）\n';
            text += '👍 听讲发言：积极发言、认真听讲\n';
            text += '🏆 运动会：班级总分第一名\n';
            text += '🎤 科创：推荐参加AI配音师（无限制），天文竞赛有难度\n\n';

            // 数学
            text += '🔢 【数学】\n';
            text += '⚠️ 重视：理解（语文基础）、应用（人民币购物）、阅读（题干变长找关键词）\n';
            text += '📌 读题三步法：①指读 → ②圈关键词 → ③速读检查\n';
            text += '📝 做题习惯：按顺序做、不会的做标记、做完及时检查\n';
            text += '✅ 书写表扬：王熙然书写获得表扬\n';
            text += '📁 收纳：文件袋放要交的和未订正的，已订正的放家里\n';
            text += '📚 错题：整理错题本，培养独立思考\n';
            text += '💻 推荐：国家中小学智慧教育平台\n\n';

            // 体育
            text += '🏃 【体育】\n';
            text += '🚨 健康预警：超重、脊柱侧弯，三年级前必须干预\n';
            text += '📊 体测项目（杭州女生）：\n';
            text += '   1分钟跳绳 143/157个（及格/满分）\n';
            text += '   坐位体前屈 16/18.6cm（及格/满分）\n';
            text += '   50米跑 11.2/11.0秒（及格/满分）\n';
            text += '   肺活量 1200/1400ml（及格/满分）\n';
            text += '🎯 锻炼：30分钟趣味比赛（轮流跳绳/体前屈/50米/肺活量，比一比）\n';
            text += '💪 心理：培养抗挫折、抗压、坚持精神\n';
            text += '🏠 家庭：每天运动、跳绳目标157个满分、注意坐姿站姿、控制体重\n\n';

            // 育儿
            text += '🏠 【习惯培养】\n';
            text += '🎒 自理：自己整理书包、穿衣吃饭收拾\n';
            text += '⏰ 时间：吃饭20-30分钟，放钟表计时，切忌催促"快点"\n';
            text += '👓 专注：专注时别打扰，老人别问饿不饿渴不渴\n';
            text += '📚 阅读：每天20分钟，家长带指读，会读了别盯着\n';
            text += '🏃 运动：每天运动，按时睡觉起床\n';
            text += '🧹 家务：专门给一项家务（分碗筷、倒垃圾）\n\n';

            text += '🌱 【能力培养】\n';
            text += '🗣️ 表达：在外玩家长离远点，让孩子独立交往\n';
            text += '😠 情绪：发脾气别被拿捏，不让得逞\n';
            text += '🛡️ 自我保护：放手尝试教正确做法，应急演练（电梯、安全通道、落水等）\n';
            text += '🎯 自我定位：注重习惯非成绩；学习是我的事；能输能赢看自己；善待他人感恩长辈\n\n';

            text += '💑 【家庭关系】\n';
            text += '夫妻关系好，亲子关系才会好\n';
            text += '常陪伴每天沟通，储蓄感情为青春期做准备\n';
            text += '不骄纵，眼中有人，遵守规则\n';

            navigator.clipboard.writeText(text).then(() => {
                showToast('✅ 已复制全部要点！');
            }).catch(() => {
                showToast('复制失败，请手动复制');
            });
        }

        // 显示提示
        function showToast(msg) {
            const toast = document.getElementById('toast');
            toast.textContent = msg;
            toast.classList.add('show');
            setTimeout(() => toast.classList.remove('show'), 2000);
        }

        // 初始化
        document.addEventListener('DOMContentLoaded', () => {
            // 默认展开第一个卡片
            document.querySelectorAll('.content-section.active .card').forEach((card, i) => {
                if (i === 0) card.classList.add('expanded');
            });

            // 手机端默认展开导航栏
            const sidebar = document.getElementById('sidebarNav');
            if (window.innerWidth <= 768 && sidebar) {
                // 确保手机端初始状态是展开的
                sidebar.classList.remove('mobile-collapsed');
            }
        });
    
    </script>
</body>
</html>
