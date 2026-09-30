# shanghai-trave
上海六日游行程攻略
<!DOCTYPE html>
<html lang="zh-CN" data-page-node-id="SD4SmOVcHnwmjsvcogoMCY">
<head data-page-node-id="qsXdQnFESsAL4CtODWM3VU">
    <meta charset="UTF-8" data-page-node-id="TPQDaTJCaohUUOQlNc3DU8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0" data-page-node-id="LR8MZWZ6VCRUeE6URhfclF">
    <title>上海及周边六日游行程攻略</title>
    <style>
        :root {
            --primary-color: #e74c3c;
            --secondary-color: #3498db;
            --accent-color: #f39c12;
            --success-color: #27ae60;
            --purple-color: #9b59b6;
            --text-dark: #2c3e50;
            --text-light: #7f8c8d;
            --bg-light: #f8f9fa;
            --border-radius: 16px;
            --shadow: 0 4px 20px rgba(0,0,0,0.08);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: "PingFang SC", "Microsoft YaHei", "Helvetica Neue", Arial, sans-serif;
            font-size: 14px;
            line-height: 1.8;
            color: var(--text-dark);
            background: linear-gradient(135deg, #f5f7fa 0%, #e4e8ec 100%);
            padding: 20px;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
        }
        
        /* 封面 */
        .cover {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: var(--border-radius);
            padding: 60px 40px;
            text-align: center;
            color: white;
            margin-bottom: 30px;
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }
        
        .cover::before {
            content: "🏙️";
            position: absolute;
            font-size: 150px;
            opacity: 0.1;
            top: -20px;
            right: -20px;
        }
        
        .cover h1 {
            font-size: 42px;
            font-weight: 700;
            margin-bottom: 15px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }
        
        .cover-subtitle {
            font-size: 20px;
            opacity: 0.95;
            margin-bottom: 30px;
        }
        
        .cover-badge {
            display: inline-block;
            background: rgba(255,255,255,0.2);
            padding: 10px 25px;
            border-radius: 30px;
            font-size: 16px;
            backdrop-filter: blur(10px);
        }
        
        /* 概览卡片 */
        .overview {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
            margin-bottom: 30px;
        }
        
        .overview-card {
            background: white;
            border-radius: var(--border-radius);
            padding: 20px;
            text-align: center;
            box-shadow: var(--shadow);
        }
        
        .overview-icon {
            font-size: 36px;
            margin-bottom: 10px;
        }
        
        .overview-value {
            font-size: 24px;
            font-weight: 700;
            color: var(--primary-color);
        }
        
        .overview-label {
            font-size: 13px;
            color: var(--text-light);
            margin-top: 5px;
        }
        
        /* 日期标签 */
        .day-tabs {
            display: flex;
            gap: 10px;
            margin-bottom: 25px;
            flex-wrap: wrap;
        }
        
        .day-tab {
            padding: 12px 24px;
            background: white;
            border-radius: 30px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            border: 2px solid transparent;
        }
        
        .day-tab:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .day-tab.active {
            background: var(--primary-color);
            color: white;
            border-color: var(--primary-color);
        }
        
        .day-tab-icon {
            margin-right: 8px;
        }
        
        /* 日程卡片 */
        .day-card {
            background: white;
            border-radius: var(--border-radius);
            padding: 35px;
            margin-bottom: 25px;
            box-shadow: var(--shadow);
        }
        
        .day-header {
            display: flex;
            align-items: center;
            margin-bottom: 25px;
            padding-bottom: 20px;
            border-bottom: 3px dashed #eee;
        }
        
        .day-number {
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            font-weight: 700;
            color: white;
            margin-right: 20px;
        }
        
        .day-1 .day-number { background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); }
        .day-2 .day-number { background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%); }
        .day-3 .day-number { background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%); }
        .day-4 .day-number { background: linear-gradient(135deg, #fa709a 0%, #fee140 100%); }
        .day-5 .day-number { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); }
        
        .day-title {
            flex: 1;
        }
        
        .day-title h2 {
            font-size: 26px;
            margin-bottom: 5px;
        }
        
        .day-theme {
            color: var(--text-light);
            font-size: 15px;
        }
        
        .day-weather {
            background: var(--bg-light);
            padding: 10px 20px;
            border-radius: 20px;
            font-size: 14px;
        }
        
        /* 时间线 */
        .timeline {
            position: relative;
            padding-left: 40px;
        }
        
        .timeline::before {
            content: "";
            position: absolute;
            left: 15px;
            top: 0;
            bottom: 0;
            width: 3px;
            background: linear-gradient(to bottom, var(--primary-color), var(--secondary-color));
            border-radius: 2px;
        }
        
        .timeline-item {
            position: relative;
            margin-bottom: 30px;
        }
        
        .timeline-item:last-child {
            margin-bottom: 0;
        }
        
        .timeline-dot {
            position: absolute;
            left: -33px;
            width: 24px;
            height: 24px;
            background: white;
            border: 3px solid var(--primary-color);
            border-radius: 50%;
        }
        
        .timeline-time {
            font-size: 13px;
            color: var(--primary-color);
            font-weight: 600;
            margin-bottom: 8px;
        }
        
        .timeline-title {
            font-size: 18px;
            font-weight: 600;
            margin-bottom: 10px;
        }
        
        .timeline-content {
            background: var(--bg-light);
            border-radius: 12px;
            padding: 18px;
        }
        
        /* 交通卡片 */
        .transport-card {
            background: linear-gradient(135deg, #e8f4fd 0%, #d4e9fa 100%);
            border-left: 4px solid var(--secondary-color);
            border-radius: 10px;
            padding: 15px 20px;
            margin-top: 12px;
        }
        
        .transport-header {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
        }
        
        .transport-icon {
            font-size: 20px;
            margin-right: 10px;
        }
        
        .transport-title {
            font-weight: 600;
            color: var(--secondary-color);
        }
        
        .transport-route {
            font-size: 14px;
            color: var(--text-dark);
            margin-bottom: 8px;
        }
        
        .transport-meta {
            display: flex;
            gap: 20px;
            font-size: 13px;
            color: var(--text-light);
        }
        
        .transport-meta span {
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        /* 景点卡片 */
        .attraction-card {
            background: linear-gradient(135deg, #fff9e6 0%, #fff3cd 100%);
            border-left: 4px solid var(--accent-color);
            border-radius: 10px;
            padding: 15px 20px;
            margin-top: 12px;
        }
        
        .attraction-header {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
        }
        
        .attraction-icon {
            font-size: 20px;
            margin-right: 10px;
        }
        
        .attraction-title {
            font-weight: 600;
            color: #b8860b;
        }
        
        .attraction-desc {
            font-size: 14px;
            color: var(--text-dark);
            line-height: 1.7;
        }
        
        /* 美食推荐 */
        .food-section {
            margin-top: 25px;
            padding-top: 25px;
            border-top: 2px dashed #eee;
        }
        
        .food-section-title {
            font-size: 20px;
            font-weight: 600;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .food-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
        }
        
        .food-card {
            background: white;
            border: 1px solid #eee;
            border-radius: 12px;
            padding: 18px;
            transition: all 0.3s ease;
        }
        
        .food-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.08);
        }
        
        .food-card-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 10px;
        }
        
        .food-name {
            font-weight: 600;
            font-size: 16px;
            color: var(--text-dark);
        }
        
        .food-price {
            background: var(--success-color);
            color: white;
            padding: 3px 10px;
            border-radius: 15px;
            font-size: 13px;
            font-weight: 600;
        }
        
        .food-type {
            font-size: 12px;
            color: var(--text-light);
            margin-bottom: 8px;
        }
        
        .food-address {
            font-size: 12px;
            color: var(--text-light);
            display: flex;
            align-items: center;
            gap: 5px;
            margin-bottom: 8px;
        }
        
        .food-recommend {
            font-size: 12px;
            color: #e74c3c;
            background: #fdf2f2;
            padding: 6px 10px;
            border-radius: 6px;
            margin-top: 8px;
        }
        
        /* 提示框 */
        .tip-box {
            background: linear-gradient(135deg, #e8f8f5 0%, #d1f2eb 100%);
            border-left: 4px solid var(--success-color);
            border-radius: 10px;
            padding: 15px 20px;
            margin-top: 15px;
        }
        
        .tip-header {
            display: flex;
            align-items: center;
            margin-bottom: 8px;
        }
        
        .tip-icon {
            font-size: 18px;
            margin-right: 8px;
        }
        
        .tip-title {
            font-weight: 600;
            color: #1e8449;
        }
        
        .tip-content {
            font-size: 14px;
            color: var(--text-dark);
        }
        
        /* 进度条 */
        .progress-bar {
            height: 8px;
            background: #eee;
            border-radius: 10px;
            margin-top: 10px;
            overflow: hidden;
        }
        
        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
            border-radius: 10px;
        }
        
        /* 两栏布局 */
        .two-columns {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }
        
        @media (max-width: 768px) {
            .overview {
                grid-template-columns: repeat(2, 1fr);
            }
            .food-grid {
                grid-template-columns: 1fr;
            }
            .two-columns {
                grid-template-columns: 1fr;
            }
        }
        
        /* 地图卡片 */
        .map-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #e4e8ec 100%);
            border-radius: 12px;
            padding: 20px;
            margin-top: 15px;
        }
        
        .map-route {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 8px;
        }
        
        .map-point {
            background: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 14px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
        }
        
        .map-arrow {
            color: var(--secondary-color);
            font-weight: bold;
        }
        
        /* 页脚 */
        .footer {
            text-align: center;
            padding: 30px;
            color: var(--text-light);
            font-size: 13px;
        }
        
        /* 高亮文字 */
        .highlight {
            background: linear-gradient(120deg, #ffd700 0%, #ffed4e 100%);
            padding: 2px 8px;
            border-radius: 4px;
            font-weight: 600;
        }
        
        /* 标签组 */
        .tag-group {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 10px;
        }
        
        .tag {
            background: var(--bg-light);
            padding: 5px 12px;
            border-radius: 15px;
            font-size: 12px;
            color: var(--text-light);
        }
        
        /* 分隔线 */
        .divider {
            height: 1px;
            background: linear-gradient(to right, transparent, #ddd, transparent);
            margin: 25px 0;
        }
    </style>
</head>
<body data-page-node-id="HpP2DERPawvubLACSryEPI">
    <div class="container" data-page-node-id="FBxyYExQzTDRea9f6TsdXN">
        <!-- 封面 -->
        <div class="cover" data-page-node-id="lyhfdvOX3LUEh2gHW4eEl6">
            <h1 data-page-node-id="LaCpNhjiW3CW3XtGa8S4ca">🏙️ 上海及周边六日游</h1>
            <p class="cover-subtitle" data-page-node-id="4aumCCfCrr84SwMBfEiFVG">10月1日 - 10月6日 · 江南水乡 · 园林古城</p>
            <div class="cover-badge" data-page-node-id="2jh0UQqrwV0IBCclGCYnGO">📅 行程总览 | 🚇 地铁出行 | 🍜 美食探店</div>
        </div>
        
        <!-- 概览 -->
        <div class="overview" data-page-node-id="32hJpj8fs09IywbxYErh6T">
            <div class="overview-card" data-page-node-id="bzSbqpwp6c62kTA4oKh70G">
                <div class="overview-icon" data-page-node-id="dFxPbFFgJ0mdPU0DHoQil8">📅</div>
                <div class="overview-value" data-page-node-id="w45cKKlEBcOELIJP9p0Wqh">6天</div>
                <div class="overview-label" data-page-node-id="G9jhEhZMrpKxDJBLd3RKsW">行程天数</div>
            </div>
            <div class="overview-card" data-page-node-id="44uEbk7xMnPjhTmYAbtg63">
                <div class="overview-icon" data-page-node-id="ruogbrykNeXqNctHjtHHmq">🏙️</div>
                <div class="overview-value" data-page-node-id="e2Wl0YdNdjMTsD6oIGZiFB">3城</div>
                <div class="overview-label" data-page-node-id="ZWRnOkrI6PamJKivxwylbV">上海·杭州·苏州</div>
            </div>
            <div class="overview-card" data-page-node-id="8fbFWbMzPooiCVBXyZlOyB">
                <div class="overview-icon" data-page-node-id="qj9xiBW7JDjbwLJd9A2KXG">🚇</div>
                <div class="overview-value" data-page-node-id="AtmHyqcivvYA6HifF8ToEI">15+</div>
                <div class="overview-label" data-page-node-id="RyAAW0zbTLPqtGFnyuSunT">地铁路线</div>
            </div>
            <div class="overview-card" data-page-node-id="L3ldtrbSQe01VAgWntaRp8">
                <div class="overview-icon" data-page-node-id="B4wEfcR2FEQXHzK85IsHkK">🍜</div>
                <div class="overview-value" data-page-node-id="HpAgJetAWb5QJR7OByZfhY">20+</div>
                <div class="overview-label" data-page-node-id="ZZOqwy1pIOBQSGE1AQ9X2g">美食推荐</div>
            </div>
        </div>
        
        <!-- 日期标签 -->
        <div class="day-tabs" data-page-node-id="VcvwPohYHjCfDD3FHANccX">
            <div class="day-tab active" data-page-node-id="QbxFlimDgX5dCfvfvkuvHQ"><span class="day-tab-icon" data-page-node-id="jbv7cugg6g5FC0rG4h4tck">👣</span>10.1 抵达</div>
            <div class="day-tab" data-page-node-id="nAsvaUtW5M86B54oCCCcf9"><span class="day-tab-icon" data-page-node-id="Vo4z8wHZcbMnhMBO2WLg8a">🌊</span>10.2 苏州河</div>
            <div class="day-tab" data-page-node-id="WrXRumGFNJZdkejmmuAZlH"><span class="day-tab-icon" data-page-node-id="4bTY8j8ngiGW7pmyy9SCok">📸</span>10.3 虹口</div>
            <div class="day-tab" data-page-node-id="JrX2ZYQ7h4aMWpwy0xGNLq"><span class="day-tab-icon" data-page-node-id="3UakYI7uC6ADBiEZQ3vgLy">🌸</span>10.4 杭州</div>
            <div class="day-tab" data-page-node-id="8FsE2Kj02UiFinM1M871hC"><span class="day-tab-icon" data-page-node-id="dmNV9f8t0mZZAGcgcawNcD">🏯</span>10.5 苏州</div>
            <div class="day-tab" data-page-node-id="JHjV2gkcZyiAI9yjMxLi8A"><span class="day-tab-icon" data-page-node-id="V32jyDxpV0tmZoeCFtoBWX">🏠</span>10.6 返程</div>
        </div>
        
        <!-- ==================== DAY 1 ==================== -->
        <div class="day-card day-1" data-page-node-id="runvmZHcLTPfysdH3b9yAi">
            <div class="day-header" data-page-node-id="tGIxdxI2G28KidH4Kzzp9T">
                <div class="day-number" data-page-node-id="hDqZut9cxIRIHt3FOtTJOy">D1</div>
                <div class="day-title" data-page-node-id="ioQF0fPsBRlkQIQss9TjOD">
                    <h2 data-page-node-id="reBC25JJLInV3FACjYqRLs">10月1日 · 抵达上海 → 七宝古镇</h2>
                    <p class="day-theme" data-page-node-id="4j8uVOBf0f5Cd136N8tBdZ">🎯 主题：初识上海 · 古镇漫步</p>
                </div>
                <div class="day-weather" data-page-node-id="1pAOCZG0WZJL7wyTIvktxk">🌤️ 10月上海 · 建议携带薄外套</div>
            </div>
            
            <div class="timeline" data-page-node-id="mHJGjZUZDP4AYD3TdCajaG">
                <div class="timeline-item" data-page-node-id="ameECCFr5x2zvk4emMbPBm">
                    <div class="timeline-dot" data-page-node-id="sHShQUEdeNiyTzb3KAmg5l"></div>
                    <div class="timeline-time" data-page-node-id="SmlnWEuZEcg0aHpsWwq0wF">🕐 15:50</div>
                    <div class="timeline-title" data-page-node-id="uHKFEhqn7BWfny6xSDXLRu">抵达上海站</div>
                    <div class="timeline-content" data-page-node-id="gsecdpzN5dFahtvf7adGga">
                        <p data-page-node-id="S2Mf97hhlrpQLCVkgZMgF4">到达上海站后，出站准备前往朱梅路住处</p>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="RtKCLchkRj7fpEetPPiNDs">
                    <div class="timeline-dot" data-page-node-id="jwAlVLL5DFjYy7aK0pYqH5"></div>
                    <div class="timeline-time" data-page-node-id="k6HeO7mIfqDH9tC0RE8ngV">🕐 16:30 - 17:30</div>
                    <div class="timeline-title" data-page-node-id="67sM29qGPCAc7wIZifjeKE">🚇 上海站 → 朱梅路</div>
                    <div class="transport-card" data-page-node-id="dMqBAfxPKzQJcRXqe0FcEn">
                        <div class="transport-header" data-page-node-id="R1cTiX6FrPUst9XNNI2kKI">
                            <span class="transport-icon" data-page-node-id="bTTpqPYhgLGUz3v5bVOeQD">🚇</span>
                            <span class="transport-title" data-page-node-id="VeJnaFmAgl4kyvlu0XWy6V">地铁1号线 → 15号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="almLH3e1fQW5u2pEQH1Myx">上海站(1号线) → 人民广场(换乘8号线) → 陆家浜路(换乘15号线) → 朱梅路</div>
                        <div class="transport-meta" data-page-node-id="HiH1m3c57eSLTArRTuxsDq">
                            <span data-page-node-id="zixbkQ94TdYQRuzvMhxTFa">⏱️ 约60分钟</span>
                            <span data-page-node-id="D3BSKTiMqXgFccEs5X1JVS">💰 约6元</span>
                            <span data-page-node-id="IylhiKs28oJUDVDCk9Np4U">🔄 换乘2次</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="Rm0JzKrYHVvOMeCdFO5NNE">
                    <div class="timeline-dot" data-page-node-id="B7Bd4QdC6ENA1GAH8zASLB"></div>
                    <div class="timeline-time" data-page-node-id="gmyHM5ZeCRHVgFI4FDYaXa">🕐 17:30 - 18:00</div>
                    <div class="timeline-title" data-page-node-id="WCAel4m63WlqkjrzR2GnyY">🏠 朱梅路休息</div>
                    <div class="timeline-content" data-page-node-id="CqjZ0f31FxtFrjz6wLqEOv">
                        <p data-page-node-id="US4UZ8FPcZspLkwOx86F5k">到达住处，稍作休息整顿，准备前往七宝古镇</p>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="MAmnEdixGkVuxWdOYbi0fd">
                    <div class="timeline-dot" data-page-node-id="P0PchArKzJiMTIl8LvtKDI"></div>
                    <div class="timeline-time" data-page-node-id="wk4MXwl0voVlEKAEx2PExn">🕐 18:00 - 19:00</div>
                    <div class="timeline-title" data-page-node-id="3lBb551zLUreCcusKl9Ax7">🚇 朱梅路 → 七宝古镇</div>
                    <div class="transport-card" data-page-node-id="dXpVobcvamo2ayDzbaSFvw">
                        <div class="transport-header" data-page-node-id="FBR7lBNGUVhaMVgFP3GPnZ">
                            <span class="transport-icon" data-page-node-id="oGpgWsvS3JuPLmRXwZ18ER">🚇</span>
                            <span class="transport-title" data-page-node-id="EwUYRjjGAaisNISSj28qjM">地铁15号线 → 9号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="33I1VrEg0iYDfJ1X9ipcGt">朱梅路(15号线) → 桂林公园(换乘9号线) → 七宝站(2号口出)</div>
                        <div class="transport-meta" data-page-node-id="rozFBq85Emgnq0Gw9ugO5s">
                            <span data-page-node-id="xy9PN2PHBIECjUQ8FRSdyk">⏱️ 约50分钟</span>
                            <span data-page-node-id="J4LjmgBClTAMSvX4iDwJuN">💰 约5元</span>
                            <span data-page-node-id="8Xm5dX3mNUNg9HJ8VDOUpS">🔄 换乘1次</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="YCs6RaPBaYqppMPn9agxr3">
                    <div class="timeline-dot" data-page-node-id="XLS03qz8k8G4S4iUCr5zqb"></div>
                    <div class="timeline-time" data-page-node-id="dO6h4hiGATQ1Xu3Y89v8F8">🕐 19:00 - 21:00</div>
                    <div class="timeline-title" data-page-node-id="0jOPXXs0szFIwLRcw3HQHy">🏮 七宝古镇夜游</div>
                    <div class="attraction-card" data-page-node-id="1XbLcNGaFLAdxEGPQSk5GN">
                        <div class="attraction-header" data-page-node-id="MYRoH1qZR4X9mJTpDMdzBQ">
                            <span class="attraction-icon" data-page-node-id="v9hsPhE9jnNHznzzZHPRGE">🏮</span>
                            <span class="attraction-title" data-page-node-id="uw1rKH2mCac7zFlRykTfNt">七宝古镇 · 江南水乡</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="N9AuKeGBE6GJ1SpxU61k5p">
                            七宝古镇是上海著名的历史文化名镇，距今已有千年历史。古镇内小桥流水、粉墙黛瓦，保留着明清时期的古建筑风貌。<br data-page-node-id="0K4qYY568JeJPpNkdpF0Kr"><br data-page-node-id="mg96etLX73Q7ruEGxUEJUa">
                            <strong data-page-node-id="YbaA92XCFKfLY1wR8goWeo">推荐游览：</strong>南大街（美食街）、北大街（文化街）、蒲汇塘桥（最佳拍照点）
                        </div>
                        <div class="tag-group" data-page-node-id="vN2JbXBzE3Zj6nmF2nIhcX">
                            <span class="tag" data-page-node-id="qaUVRT4Yi900Va4dRPtJuL">🎫 免费开放</span>
                            <span class="tag" data-page-node-id="M370nNrBBaqnH1kAMXfgrK">⏱️ 建议2-3小时</span>
                            <span class="tag" data-page-node-id="1tnpbqbV6ki10DrusNkklK">📸 夜景优美</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="1fCVs4S0zBYc9QyJLqP3Sq">
                    <div class="timeline-dot" data-page-node-id="HzmblyyM0eCMvptX6DBp7h"></div>
                    <div class="timeline-time" data-page-node-id="IsXaEEDJllUG1v4QZUupql">🕐 21:00 - 22:00</div>
                    <div class="timeline-title" data-page-node-id="lDhoZ3yEyW7Zi9ivbIEP08">🚇 返回朱梅路</div>
                    <div class="transport-card" data-page-node-id="mqUfbmlGcuTOaD3NuBpl6B">
                        <div class="transport-header" data-page-node-id="7CK0iw58ecWn5UK1XWbbBt">
                            <span class="transport-icon" data-page-node-id="0Wxq3MHf6Jo2gMngfZVEuP">🚇</span>
                            <span class="transport-title" data-page-node-id="9ZHqFADRPCV6U0SKWeu5eL">地铁9号线 → 15号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="j2GGjlnANKwVH5cqdImACg">七宝站(9号线) → 桂林公园(换乘15号线) → 朱梅路</div>
                        <div class="transport-meta" data-page-node-id="6mirON4s1AQkJcPABRPWTl">
                            <span data-page-node-id="RRaWIOeZD2cNZYxZiQvAXs">⏱️ 约50分钟</span>
                            <span data-page-node-id="dIMjq1EJN9RoPrA2AY4wek">💰 约5元</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- 美食推荐 -->
            <div class="food-section" data-page-node-id="PBur86VztPMtnAm30J9TVD">
                <div class="food-section-title" data-page-node-id="nppRA2LdVbONithdCQFizW">
                    <span data-page-node-id="4ZED4QoA19ZtDJLcYMcseN">🍜</span>
                    <span data-page-node-id="74JtZ0mlH2LZJy6uPhCMWo">七宝古镇美食推荐</span>
                    <span style="font-size: 12px; color: #27ae60; font-weight: normal;" data-page-node-id="DBXlCEzA1R3oVbVEiAjJsf">人均均 &lt; 200元</span>
                </div>
                <div class="food-grid" data-page-node-id="7gEktE2Eeml89EJVGv34rk">
                    <div class="food-card" data-page-node-id="yIRRoysM2vPVqo0BLEIxGM">
                        <div class="food-card-header" data-page-node-id="ajnCbEbe3VyZEHttdcGqp2">
                            <span class="food-name" data-page-node-id="JM406HZ2B6ekBX6qWejUwb">七宝老街汤团店</span>
                            <span class="food-price" data-page-node-id="JlWnWL1OHbjEOxibvTgsek">人均16元</span>
                        </div>
                        <div class="food-type" data-page-node-id="hFRRSlcyak4xlMANEggBce">🥟 传统小吃</div>
                        <div class="food-address" data-page-node-id="4J3naA1zna1L7NaLoFK3nd">📍 南大街26号</div>
                        <div class="food-recommend" data-page-node-id="6K16R6kCY3Gu8ufilEUXXB">⭐ 推荐：鲜肉汤团、豆沙汤团，5元/个</div>
                    </div>
                    <div class="food-card" data-page-node-id="0268Md7K5WdCVgoKi2ZDhN">
                        <div class="food-card-header" data-page-node-id="31TfxlDAQrlUUO2iyYbSo4">
                            <span class="food-name" data-page-node-id="OhsUw26LvY2xu1u39Xw6ZP">宝丰饭店</span>
                            <span class="food-price" data-page-node-id="zlfhS5T6m0FMsl9r7j6Kxa">人均60元</span>
                        </div>
                        <div class="food-type" data-page-node-id="WVgevMv9euSdLbQHmRjeR6">🍖 本帮菜</div>
                        <div class="food-address" data-page-node-id="Mb1ljWPrW8FqJaU5pUGrGE">📍 南大街5号</div>
                        <div class="food-recommend" data-page-node-id="MjHVjpHBpFJOxwNlNf1zhJ">⭐ 推荐：白切羊肉面35元、白切羊肉</div>
                    </div>
                    <div class="food-card" data-page-node-id="Aq3wlCrF55cYlZMFF41jAh">
                        <div class="food-card-header" data-page-node-id="jEKJSMIOKBlzng87dvCRH2">
                            <span class="food-name" data-page-node-id="hLwRLiKHequ8KKmLrFDANT">宝丰海棠糕</span>
                            <span class="food-price" data-page-node-id="S2YcmE1XweTCuXqG59lcvR">人均10元</span>
                        </div>
                        <div class="food-type" data-page-node-id="6q9wpfTQ3kcQRhHBjwFSks">🍰 传统甜点</div>
                        <div class="food-address" data-page-node-id="90251GXXBVPpxzN0egEvYX">📍 南大街3号</div>
                        <div class="food-recommend" data-page-node-id="qSftsV8JtADuhBANus1UHl">⭐ 推荐：海棠糕7元、梅花糕10元</div>
                    </div>
                    <div class="food-card" data-page-node-id="hz1O325Nz4AYDPRaiCbjDt">
                        <div class="food-card-header" data-page-node-id="2CqtAbvHab9qXsWzOdTnhl">
                            <span class="food-name" data-page-node-id="leuDcQ6AaF6DIl1XJN76rv">顺昌仁寿灌蛋</span>
                            <span class="food-price" data-page-node-id="K2rF9eILeiao4yTDCDJlEX">人均18元</span>
                        </div>
                        <div class="food-type" data-page-node-id="91Sf6fYFLqUvI3hnDiAric">🥚 非遗美食</div>
                        <div class="food-address" data-page-node-id="P6nVrQNlr9Iv7dY9lqCMk4">📍 南大街43号</div>
                        <div class="food-recommend" data-page-node-id="Ndn3FvuXek749jtjPBI7yI">⭐ 推荐：灌蛋15-18元，肉馅塞入鸭蛋</div>
                    </div>
                    <div class="food-card" data-page-node-id="AeJYdkGMy86XGc27q1XTiA">
                        <div class="food-card-header" data-page-node-id="2uFl101fj5LBamoWHHax71">
                            <span class="food-name" data-page-node-id="X7gzeOR1pdaR6n7P2oB8jQ">管老太臭豆腐</span>
                            <span class="food-price" data-page-node-id="AoPutx6v2oOMirQYSdFxlU">人均15元</span>
                        </div>
                        <div class="food-type" data-page-node-id="tl4G8KZcNaK7ZGmp7retOi">🧈 特色小吃</div>
                        <div class="food-address" data-page-node-id="r3gLndinCGAH3MVZRJxWwa">📍 南大街18号</div>
                        <div class="food-recommend" data-page-node-id="LJfltVbBhS81wcOdDGV1xS">⭐ 推荐：臭豆腐10-15元/份，外酥里嫩</div>
                    </div>
                    <div class="food-card" data-page-node-id="Ua8Lv6AccbVDMlO3HVcHGO">
                        <div class="food-card-header" data-page-node-id="Daw0XjcbSMFEkUH3rImEJ7">
                            <span class="food-name" data-page-node-id="DuykiJRcxA5iPmrl10NcMd">老五葱油饼</span>
                            <span class="food-price" data-page-node-id="bQBpVTikv0gJ8RlftIyWLB">人均8元</span>
                        </div>
                        <div class="food-type" data-page-node-id="pNPAQyHkdKkOT3WyM0yzOB">🫓 网红小吃</div>
                        <div class="food-address" data-page-node-id="lewl0nZoF6gDQND3FXllTo">📍 南大街12号</div>
                        <div class="food-recommend" data-page-node-id="iESRKNQjDFKhWvh2wPA5Rm">⭐ 推荐：葱油饼8元/个，外脆里嫩</div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- ==================== DAY 2 ==================== -->
        <div class="day-card day-2" data-page-node-id="oG88tJMCwFCq4GBLGDWof8">
            <div class="day-header" data-page-node-id="GDUbOV4prDWzOso3o6ye4x">
                <div class="day-number" data-page-node-id="eMjp4W87UCeHhyypZ57Mxr">D2</div>
                <div class="day-title" data-page-node-id="Y1OPetmzZaW5BPc2o9hzhs">
                    <h2 data-page-node-id="3KoQ7a6pxHECSYkvabFXc2">10月2日 · 苏州河漫步 → 东方明珠</h2>
                    <p class="day-theme" data-page-node-id="lZuCLsIt6gIDFmpZo8aysJ">🎯 主题：城市漫步 · 浦江游览</p>
                </div>
                <div class="day-weather" data-page-node-id="Wl6ILg7YL9YUqLbm9Oq4dO">🌤️ 适合步行的一天</div>
            </div>
            
            <div class="timeline" data-page-node-id="150ov7GGud3kzydjGCAroF">
                <div class="timeline-item" data-page-node-id="L8H1RTl4qGzr3DiaYD3tEH">
                    <div class="timeline-dot" data-page-node-id="Gs8CvDbgJCNu0fCIPAcVlM"></div>
                    <div class="timeline-time" data-page-node-id="71aSvFbfx4U4DFrvTnFdqP">🕐 09:00</div>
                    <div class="timeline-title" data-page-node-id="hmOGj7QMNXyU9n3DR6ozQV">🚇 朱梅路 → 天潼路站</div>
                    <div class="transport-card" data-page-node-id="jqZWkUe27MelYLoojUcJiv">
                        <div class="transport-header" data-page-node-id="1cCzPYJXaE7pHOhelIhLpv">
                            <span class="transport-icon" data-page-node-id="fUQ1c6C4w8w3YbGFgAPgLy">🚇</span>
                            <span class="transport-title" data-page-node-id="mCw2xAIcQQlVYIiFOqlgEt">地铁15号线 → 12号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="07g60qov3RufPpoiTMRRTm">朱梅路(15号线) → 大渡河路(换乘12号线) → 天潼路站(3号口出)</div>
                        <div class="transport-meta" data-page-node-id="1HWJtsr5FG2K8UuuiT9rE6">
                            <span data-page-node-id="qNpYuDSlzE60EZTPPHX8VE">⏱️ 约45分钟</span>
                            <span data-page-node-id="rAh444GqZPp2wBUWm1Irim">💰 约5元</span>
                            <span data-page-node-id="bhv6m1DHWEU2wrCTJpEhfA">🔄 换乘1次</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="unRBm2YJoifRsN5Eatc6Qr">
                    <div class="timeline-dot" data-page-node-id="TQXRS965u1BPCfZIQwldwI"></div>
                    <div class="timeline-time" data-page-node-id="rIyvdlGgGOsMfOixqe808a">🕐 09:45 - 12:00</div>
                    <div class="timeline-title" data-page-node-id="5Am4Cn0T742m1QvR3VnsF4">🌊 苏州河漫步</div>
                    <div class="attraction-card" data-page-node-id="F5pkTXZIU7UTggXwRqC77d">
                        <div class="attraction-header" data-page-node-id="LPDLXrAug0nbbt92IQluPE">
                            <span class="attraction-icon" data-page-node-id="WjRA71SGideeClyU9IWmOz">🌊</span>
                            <span class="attraction-title" data-page-node-id="aFZo6XLdGapg1YmGDQAo3r">苏州河 · 城市河流</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="gq7KP8YbwpEJF7X1JQAmCr">
                            从12号线天潼路站3号口出来右转，沿苏州河步道漫步。苏州河是上海的母亲河，两岸风光旖旎，可以看到历史建筑与现代摩天楼的完美融合。<br data-page-node-id="uNmxEEref93m9HGKeo7Cce"><br data-page-node-id="Y4fddDnui7axv0D3oPzL3z">
                            <strong data-page-node-id="uCBjTvPhNbBrAoaZkIlYaa">推荐路线：</strong>天潼路站 → 外白渡桥 → 苏州河步道 → 外滩源 → 东方明珠
                        </div>
                        <div class="tag-group" data-page-node-id="VPBJSdAacan7PhF62o3kcz">
                            <span class="tag" data-page-node-id="c0kCRd7kVtNObkB7lGbf3r">🎫 免费</span>
                            <span class="tag" data-page-node-id="lDlEGiThtdwPTlFI6yRwJ0">🚶 步行约2小时</span>
                            <span class="tag" data-page-node-id="h2zMI7FRCNSpKFSyw4XZji">📸 拍照圣地</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="1LKfZQS7yDgiB1SbbTCr3S">
                    <div class="timeline-dot" data-page-node-id="ARD0dq0Ve4OYCwJmBqWUYF"></div>
                    <div class="timeline-time" data-page-node-id="QOV22wvmTT7g4cD5VvI9gR">🕐 12:00 - 14:00</div>
                    <div class="timeline-title" data-page-node-id="7EInRAL89EVDUB4Um09156">🍽️ 午餐时间</div>
                    <div class="attraction-card" data-page-node-id="EtARb8TTfYHIILDUbDwbLB">
                        <div class="attraction-header" data-page-node-id="PN3XM3ngM5AWehzbBK6bqO">
                            <span class="attraction-icon" data-page-node-id="9UcpfuFadlJY4VVh4ElD13">☕</span>
                            <span class="attraction-title" data-page-node-id="RxJ3Gp3U3ABH3MasqIYvA0">汭REi·FLOWER COFFEE BAR</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="39EXZKez1YYOaIkqCsAap7">
                            网红咖啡店，可一边品尝咖啡，一边欣赏东方明珠塔的无敌景观。户外座位区是最佳观赏位置。<br data-page-node-id="UOK796lCjdHpqHB6QJYHVL"><br data-page-node-id="AYDywrR11tk2dPMSOEfhYC">
                            <strong data-page-node-id="b50e0pZkzfMsaoANP27x91">推荐：</strong>桂花拿铁38元、玫瑰拿铁、各式蛋糕甜点
                        </div>
                        <div class="tag-group" data-page-node-id="slUA1KCjhsLxBAvUYvB93g">
                            <span class="tag" data-page-node-id="yr1E2O3vN8hpWIz9aabJ63">📍 北苏州路234号</span>
                            <span class="tag" data-page-node-id="d7MBKOAevB2qejAC6ZBMgs">💰 人均50元</span>
                            <span class="tag" data-page-node-id="DhNXJrv3vitE6HoE5O8UhP">🌸 花园咖啡</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="5Yz1QOxFrjC3w9CJ5Cg8AI">
                    <div class="timeline-dot" data-page-node-id="NNoEYPTbsl0J2vs5nUH7fV"></div>
                    <div class="timeline-time" data-page-node-id="Fc1LvoPmeEqjQ7b9erK5FH">🕐 14:00 - 17:00</div>
                    <div class="timeline-title" data-page-node-id="GjsS2fG7j6OIvagwHCecDc">🗼 东方明珠游览</div>
                    <div class="attraction-card" data-page-node-id="mLn1iJ5PhTeK65Y7ashIRE">
                        <div class="attraction-header" data-page-node-id="eDHyC2mWgfjmYZET6bPJCg">
                            <span class="attraction-icon" data-page-node-id="mmoN2y0oGSQsz36F8xOq15">🗼</span>
                            <span class="attraction-title" data-page-node-id="fL6XOWp69M1X14Xekz6Wdv">东方明珠塔 · 上海地标</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="PIk18RtIIEOTjLybDEDaIY">
                            东方明珠塔高468米，是上海的标志性建筑。登上观光层可以俯瞰整个上海全景，天气好的时候可以看到远处的黄浦江和陆家嘴金融区。<br data-page-node-id="ZXv695q8WOuSINviorem1H"><br data-page-node-id="sKU578AhqFo5X9Xs1X1pF8">
                            <strong data-page-node-id="i0jCzazbxM42IxktwaaXIH">推荐：</strong>263米主观光层、259米悬空观光廊
                        </div>
                        <div class="tag-group" data-page-node-id="HRLxyzGXtGKrd1xVBsTMBz">
                            <span class="tag" data-page-node-id="dV3rBA2erw2gPwgfnZNDRy">🎫 门票约120元</span>
                            <span class="tag" data-page-node-id="3Mfc3NUuNezGVQ6p3JhZzP">⏱️ 建议2-3小时</span>
                            <span class="tag" data-page-node-id="VXs3uLDiKLXhdZnDgRuJIU">🌆 夜景更美</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- 美食推荐 -->
            <div class="food-section" data-page-node-id="EPRxBxj7rgwcJr6xJmloJe">
                <div class="food-section-title" data-page-node-id="XFLAGBZZVclgDh2kZ9kTfW">
                    <span data-page-node-id="hEtatledV009A7Ke2dTkko">🍽️</span>
                    <span data-page-node-id="9AIYAjngF59mv43CYPp40B">苏州河/东方明珠附近美食</span>
                </div>
                <div class="food-grid" data-page-node-id="6iK5YlgGNfsNM43H1VRGNP">
                    <div class="food-card" data-page-node-id="EtX9vrs0RUh481HSauXHF6">
                        <div class="food-card-header" data-page-node-id="qIBKwmd5FmyBRJxuddFx7M">
                            <span class="food-name" data-page-node-id="qVe1mVec0aK6jeDBJ88JE4">汭REi·FLOWER COFFEE</span>
                            <span class="food-price" data-page-node-id="H2tBUH2REHIiiU5AKBF0ky">人均50元</span>
                        </div>
                        <div class="food-type" data-page-node-id="wBqqNKX0qFO8HrlwT9NJBk">☕ 网红咖啡</div>
                        <div class="food-address" data-page-node-id="sD0AFLGuln6VrlUoQ5eaX8">📍 北苏州路234号（近邮政博物馆）</div>
                        <div class="food-recommend" data-page-node-id="dces2W1edhR41NS8cOP6LM">⭐ 推荐：桂花拿铁38元，可赏东方明珠景</div>
                    </div>
                    <div class="food-card" data-page-node-id="fDv6G3sGrB9teMEbBYfbgi">
                        <div class="food-card-header" data-page-node-id="YX3L272SURwR2N8VNZ5bI9">
                            <span class="food-name" data-page-node-id="VYTE0NQxQR1PNxcWZGmo5v">上海邮政博物馆咖啡</span>
                            <span class="food-price" data-page-node-id="jDViEfioHEvOx8ia5bNZnf">人均40元</span>
                        </div>
                        <div class="food-type" data-page-node-id="Dj0NmJtitDxgxCKR5h9PE3">☕ 特色咖啡</div>
                        <div class="food-address" data-page-node-id="idytLWXdbscvCMY2fk22JC">📍 天潼路433号</div>
                        <div class="food-recommend" data-page-node-id="JGMLGA6y9oRHZJFjAUdu4a">⭐ 推荐：邮政主题咖啡，环境独特</div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- ==================== DAY 3 ==================== -->
        <div class="day-card day-3" data-page-node-id="xw6ZKTSU5rTHRbDrycdwr2">
            <div class="day-header" data-page-node-id="D9WnnhWJWYcqb2ALjxGB9z">
                <div class="day-number" data-page-node-id="7WRNuH7xWxUNeZNEynKVVM">D3</div>
                <div class="day-title" data-page-node-id="QisGgKounuRCKzCqtrWbxw">
                    <h2 data-page-node-id="9q9uYGy3GmwjwAoiXbIMzD">10月3日 · 虹口写真拍摄</h2>
                    <p class="day-theme" data-page-node-id="DlDk0LE10mMkoME9c9y2Km">🎯 主题：文艺打卡 · 今潮8弄</p>
                </div>
                <div class="day-weather" data-page-node-id="reTmRlJOq4VK3GSW15HrLI">📸 拍照的好天气</div>
            </div>
            
            <div class="timeline" data-page-node-id="WBjn2U2w4dAuS0znlCfjAm">
                <div class="timeline-item" data-page-node-id="JBkx6GWyXgqMhpaSznvxqV">
                    <div class="timeline-dot" data-page-node-id="rwqo3shGeCqoxkHN2mJ1Bz"></div>
                    <div class="timeline-time" data-page-node-id="EWjDG4iM5h8BSHqGIKbbrt">🕐 08:00</div>
                    <div class="timeline-title" data-page-node-id="8pec8Nnwv8TvBgMCA3CWMU">🚇 朱梅路 → 四川北路</div>
                    <div class="transport-card" data-page-node-id="QTQ04xtocRAULmcLDYEPfW">
                        <div class="transport-header" data-page-node-id="KBC6vHCyjz1V1tC38j5mQc">
                            <span class="transport-icon" data-page-node-id="DLUh5AqCn1EtU2XqA64p64">🚇</span>
                            <span class="transport-title" data-page-node-id="ubbYIgrPepVoeXXXWJBN42">地铁15号线 → 10号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="EgjoOZBEiamkwlo9HFq6OT">朱梅路(15号线) → 桂林公园(换乘9号线) → 陆家浜路(换乘10号线) → 四川北路站(3号口出)</div>
                        <div class="transport-meta" data-page-node-id="CJOcVg4lszv9G61Zuhod13">
                            <span data-page-node-id="ggFz5BwxAcGxuH6bjBpW8x">⏱️ 约55分钟</span>
                            <span data-page-node-id="nAE9X3sI1kgPqo4MXer4Vd">💰 约6元</span>
                            <span data-page-node-id="PXvIZkgwhY5Hkh4EPFxvHJ">🔄 换乘2次</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="XypfUYbP7pDXogvNV1oSE8">
                    <div class="timeline-dot" data-page-node-id="V5EQJUyRMufNc5XsXQQefO"></div>
                    <div class="timeline-time" data-page-node-id="8BQ0momOZHUWYvx24C4kAv">🕐 09:00 - 12:00</div>
                    <div class="timeline-title" data-page-node-id="e9pDoEuEl3ClAILdBJulzM">📸 写真拍摄</div>
                    <div class="attraction-card" data-page-node-id="8wWQMVAYNMMGB3ikrrIOLM">
                        <div class="attraction-header" data-page-node-id="igc7CTd7kYexXH9qDVThXv">
                            <span class="attraction-icon" data-page-node-id="JJMHfkCkgB1AvAaHzoIatJ">📸</span>
                            <span class="attraction-title" data-page-node-id="YIyS0VOaJFuYnAk30r1Obz">今潮8弄 · 石库门里弄</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="PdY8Ys1fK8mTRCtt0y8bwb">
                            今潮8弄是上海著名的网红打卡地，由1928年建成的"公益坊"城市更新而来。保留了8条里弄、60幢石库门及8幢独立历史建筑，融合了历史风貌与现代潮流。<br data-page-node-id="R0u0sMBhm2mZ1tox9dwDBg"><br data-page-node-id="9MrFbrCiqD5Bq6VdVl3gGV">
                            <strong data-page-node-id="KOpriTXJbspcDSjBjLnACj">拍摄亮点：</strong>海派文化中心、石库门建筑群、巴金图书馆、"时光折叠"互动墙
                        </div>
                        <div class="tag-group" data-page-node-id="fHctryvkK5Xu0fYH4a0WXG">
                            <span class="tag" data-page-node-id="DFvEQSVK9XOFVZo7l0Yzj2">📍 四川北路989弄</span>
                            <span class="tag" data-page-node-id="JxYS9w6q0XnetJ7pHkIUZl">🎫 免费开放</span>
                            <span class="tag" data-page-node-id="5nK7RbjfX8Bz6Yj9ToEwUv">⏱️ 10:00-22:00</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="IunHSPegnYeVfVDi18FbHf">
                    <div class="timeline-dot" data-page-node-id="ukTMEEvR9Dx3OyQAcbZ0VE"></div>
                    <div class="timeline-time" data-page-node-id="FiKq3oQtiSKOQri9dHrwFb">🕐 12:00 - 14:00</div>
                    <div class="timeline-title" data-page-node-id="zPAkVA52bSBFozjgDHp4uf">🍽️ 午餐</div>
                    <div class="attraction-card" data-page-node-id="eegHDRMGmPL6hYJlu3KsH5">
                        <div class="attraction-header" data-page-node-id="WtJdlAYYDsoOoq2TL0Fd2u">
                            <span class="attraction-icon" data-page-node-id="yvGzUtFafvXfCvCBk7lnmL">🍜</span>
                            <span class="attraction-title" data-page-node-id="P0sLFp9lgnGSs1DrGpKqGi">今潮8弄内餐厅</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="Qym9X1NYLZD2eKoEWKHAgg">
                            今潮8弄内有多家特色餐厅和咖啡馆，可以边吃边逛。
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="O72J0eD3bD1rqeP8Q8gJpu">
                    <div class="timeline-dot" data-page-node-id="6IeVKJjmQPiCGNjP5oceTR"></div>
                    <div class="timeline-time" data-page-node-id="JZiDH93VtoN0PcFtoNC5MX">🕐 14:00 - 17:00</div>
                    <div class="timeline-title" data-page-node-id="1PBCCVxR9fgtzUqi5RgdYi">🚶 附近逛逛</div>
                    <div class="attraction-card" data-page-node-id="AHtRGxkEnzwg9o4EhLXpRJ">
                        <div class="attraction-header" data-page-node-id="YSwakpKGW6WhcX7o5KtTOD">
                            <span class="attraction-icon" data-page-node-id="3KXVQiPvZx2t10b0eyvUyl">🛍️</span>
                            <span class="attraction-title" data-page-node-id="3pLKIzlBtNCTCYJyaG4HHY">四川北路商圈</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="I99a4b5kkYkKAzPwgVICft">
                            四川北路是上海著名的商业街，可以逛逛附近的商场和特色小店，感受老上海的都市风情。
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- 美食推荐 -->
            <div class="food-section" data-page-node-id="mOBEOj4LlIeEMiqUecrHFE">
                <div class="food-section-title" data-page-node-id="m7HqWi7Yqly35PhURLadtW">
                    <span data-page-node-id="40wylDSAXBppQxz7SBPI6l">🍽️</span>
                    <span data-page-node-id="kOZIHfAGkIzxvfOhZ0Es7i">今潮8弄/四川北路美食推荐</span>
                </div>
                <div class="food-grid" data-page-node-id="AVGxxYOY7IasB7NEc6Ooyx">
                    <div class="food-card" data-page-node-id="AeiC0pLSt1a8WailgSRUKw">
                        <div class="food-card-header" data-page-node-id="0t2UsEtCJ6DBHHuwGNBYJW">
                            <span class="food-name" data-page-node-id="144CAFuGBJxe57JHmYCbY4">MONO COFFEE</span>
                            <span class="food-price" data-page-node-id="c03Rb9EQO2fE2uY7XuB5Pd">人均51元</span>
                        </div>
                        <div class="food-type" data-page-node-id="LSFvvTldP05Uia3AvtgDj1">☕ 精品咖啡</div>
                        <div class="food-address" data-page-node-id="xGI4W2FAHa7MEF1ffSgHMe">📍 四川北路989弄今潮8弄3号楼101室</div>
                        <div class="food-recommend" data-page-node-id="o5yDycYJz1AGJw871KL4ux">⭐ 推荐：手冲咖啡、特色甜点</div>
                    </div>
                    <div class="food-card" data-page-node-id="Pf92xetBGFsDWpFzRYiQlX">
                        <div class="food-card-header" data-page-node-id="FHRtLjHmcqqQnSwhWrRk2s">
                            <span class="food-name" data-page-node-id="q5cJnU6NHCO6B0if9HzQCB">一尺花园</span>
                            <span class="food-price" data-page-node-id="gTaPoBkCdImlBqXQnzuCYS">人均62元</span>
                        </div>
                        <div class="food-type" data-page-node-id="dytJWSLLSdg1cqDlm9zGI4">🌿 花园咖啡</div>
                        <div class="food-address" data-page-node-id="Er6NTu9XkNJwXqgNDGzOpm">📍 四川北路989弄今潮8弄8号楼</div>
                        <div class="food-recommend" data-page-node-id="98mZJ9YwBb996Vs6loUnZ5">⭐ 推荐：1907年老洋房改造，环境优雅</div>
                    </div>
                    <div class="food-card" data-page-node-id="iwBW31BpvEiBwokZwdptoV">
                        <div class="food-card-header" data-page-node-id="mV4kAeAKymExr909xSoA3Y">
                            <span class="food-name" data-page-node-id="4zcWoF4tTv4nK8HYpNY5gE">星巴克(今潮8弄店)</span>
                            <span class="food-price" data-page-node-id="HhLWoBgU7vACcJmBu87hK5">人均35元</span>
                        </div>
                        <div class="food-type" data-page-node-id="sbtRYgjZagdsTFv9HP3oPv">☕ 连锁咖啡</div>
                        <div class="food-address" data-page-node-id="DMxLEfSDtsbDTBqHahfRHY">📍 四川北路今潮8弄</div>
                        <div class="food-recommend" data-page-node-id="uMEFTUjajA6k7irDn7D5Aw">⭐ 推荐：拿铁、卡布奇诺</div>
                    </div>
                    <div class="food-card" data-page-node-id="ryNlvn4UcKg4CSdfBfCKuD">
                        <div class="food-card-header" data-page-node-id="PC3rD0yMMzLfkCyMNS5znk">
                            <span class="food-name" data-page-node-id="h3Tx523JjOByHUFz8rOcMh">裕兴记·蟹黄面馆</span>
                            <span class="food-price" data-page-node-id="KsHjk19DnwMvAkxi4m1AZS">人均43元</span>
                        </div>
                        <div class="food-type" data-page-node-id="7q8HFmH4Ftm2MqedEJ7AyF">🍜 苏式面馆</div>
                        <div class="food-address" data-page-node-id="7594cD7xyQzodPxbNGsH6C">📍 四川北路1318号盛邦大厦1层</div>
                        <div class="food-recommend" data-page-node-id="3rS3h9p4rE3BrEPQyPvtGP">⭐ 推荐：蟹粉虾仁面，味道浓郁</div>
                    </div>
                    <div class="food-card" data-page-node-id="qYa9RyFBhHNHljzPeJr7HS">
                        <div class="food-card-header" data-page-node-id="aTITFls0YmsGG7F8MDWv92">
                            <span class="food-name" data-page-node-id="D8oFOhS3G1g66yuRViiMsJ">3号仓库·餐厅</span>
                            <span class="food-price" data-page-node-id="wK3xHkLp8H8U5ibfvBGhow">人均146元</span>
                        </div>
                        <div class="food-type" data-page-node-id="bFQFXDtBrfSeZqGzcmaqPr">🍽️ 创意中餐</div>
                        <div class="food-address" data-page-node-id="4eOI0sypgGcxsmzQ6gyn2y">📍 四川北路939号滨港商业中心L6层</div>
                        <div class="food-recommend" data-page-node-id="PSrkfW6Mur60ODrFqphROK">⭐ 推荐：环境优雅，适合聚餐</div>
                    </div>
                    <div class="food-card" data-page-node-id="P4H6F750m0UFgMhXDJTIY1">
                        <div class="food-card-header" data-page-node-id="8U7EVNeGMyaNnBuhzkzGyX">
                            <span class="food-name" data-page-node-id="ptgUmB89T5BUR3D5OJL3TL">金粤轩(北外滩店)</span>
                            <span class="food-price" data-page-node-id="LZ3BVEsun5T09k0w6OIUL0">人均150元</span>
                        </div>
                        <div class="food-type" data-page-node-id="LHjlpFNwfqcOMJP6hyyYGQ">🥟 粤菜</div>
                        <div class="food-address" data-page-node-id="7D4W9uZkVsc7CbV6fPEBks">📍 天潼路328号星荟中心1楼</div>
                        <div class="food-recommend" data-page-node-id="K6vxXrQUbHiu754nGswmHS">⭐ 推荐：精致粤菜，服务好</div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- ==================== DAY 4 ==================== -->
        <div class="day-card day-4" data-page-node-id="5NNqHkXTxhHdxLF8C7X03j">
            <div class="day-header" data-page-node-id="6rj6CSnUalQTF4pGUv8Q70">
                <div class="day-number" data-page-node-id="OSx1n0oXOV5vKLdaZkMt26">D4</div>
                <div class="day-title" data-page-node-id="kUIkuJamQcRK1gsVku7k6U">
                    <h2 data-page-node-id="YFKddQByLCAdgjqNyx0RHb">10月4日 · 杭州西湖一日游</h2>
                    <p class="day-theme" data-page-node-id="fHLAVPtixRca22swYIan8S">🎯 主题：西湖美景 · 杭帮菜</p>
                </div>
                <div class="day-weather" data-page-node-id="y9lHBhie5578zRFTX02imC">🌸 江南好风景</div>
            </div>
            
            <div class="timeline" data-page-node-id="wc3WD9zqSpi5WBitoxYLyD">
                <div class="timeline-item" data-page-node-id="YKHKTGP3HKYvRiea4nWp6R">
                    <div class="timeline-dot" data-page-node-id="NAAOhQATYuJtOrEB3BpPSO"></div>
                    <div class="timeline-time" data-page-node-id="Mkvga0yx2K8fPvBKko41K8">🕐 07:00</div>
                    <div class="timeline-title" data-page-node-id="hjDDerMZHfLJUKZ8BoONLh">🚇 朱梅路 → 虹桥站</div>
                    <div class="transport-card" data-page-node-id="ZdI5gZlXAoABzUxiVtvy9a">
                        <div class="transport-header" data-page-node-id="2MXmAkbn8yOdYBHCSNf4CX">
                            <span class="transport-icon" data-page-node-id="blHNBGlW5B91ZqcbK5SJRJ">🚇</span>
                            <span class="transport-title" data-page-node-id="FKXwjZNkgPEw8tbamEUzXZ">地铁15号线 → 2号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="tB4KvW7oeMyvgCUMsigAvM">朱梅路(15号线) → 桂林公园(换乘9号线) → 陆家浜路(换乘10号线) → 虹桥2号航站楼(换乘2号线) → 虹桥火车站</div>
                        <div class="transport-meta" data-page-node-id="njvDKubBdekTXjAEGC7ADW">
                            <span data-page-node-id="gudKAG4Vxy3pzGePxQBCXn">⏱️ 约70分钟</span>
                            <span data-page-node-id="CwTXSPuSuBj2HqwT1R0y7w">💰 约7元</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="uOYa0JozDF1FWiDvsCYMIb">
                    <div class="timeline-dot" data-page-node-id="puprsUq2r8w4Gyi9b6QF01"></div>
                    <div class="timeline-time" data-page-node-id="oEAatv70m6It25Ak64v82Z">🕐 07:56 - 08:41</div>
                    <div class="timeline-title" data-page-node-id="qpxFPn74KPpF6C6BfL9vHk">🚄 虹桥站 → 杭州东</div>
                    <div class="transport-card" data-page-node-id="yi1q8x3siJWODanYJ0cTUW">
                        <div class="transport-header" data-page-node-id="NvFMgmCjGYwmNnn5AyMcY4">
                            <span class="transport-icon" data-page-node-id="VLLyfIxpXCBwGWv9ww1jpH">🚄</span>
                            <span class="transport-title" data-page-node-id="uvDWsoy8PMtKMWFJhTJc7S">高铁 G7541 / G7543</span>
                        </div>
                        <div class="transport-route" data-page-node-id="8jHw7zBgEc9WkUKjRKDEQz">虹桥站 → 杭州东站</div>
                        <div class="transport-meta" data-page-node-id="QmNz7Ftqg5ReuRrv9JT5vj">
                            <span data-page-node-id="AEnCljsQdCE1eaqVVzqHlA">⏱️ 约45分钟</span>
                            <span data-page-node-id="2N9CiAS5dt0qGdTJP8Wy0x">💰 二等座约73元</span>
                            <span data-page-node-id="JEMONWu6ehZ90G6tAWmEpq">🚄 高铁</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="bYUCFGJedIKAxwhTpKkHFo">
                    <div class="timeline-dot" data-page-node-id="8HmsHUGG30INA9waZ9r7J6"></div>
                    <div class="timeline-time" data-page-node-id="yRJEG5QRfB7MQ64UP2KXrw">🕐 09:00 - 12:00</div>
                    <div class="timeline-title" data-page-node-id="mqZLAKjWzNsbGVqXuWEGcv">🌸 西湖游览（上午）</div>
                    <div class="attraction-card" data-page-node-id="7KEhUbqf7zRPPZBMgZKDrU">
                        <div class="attraction-header" data-page-node-id="ynfeSoFaCX3JBAkR9ChPca">
                            <span class="attraction-icon" data-page-node-id="rlpeX734YwYDtNCM47pf3n">🌸</span>
                            <span class="attraction-title" data-page-node-id="3ANrBr7cMjQFnNsgvlsGZd">西湖 · 人间天堂</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="zYFRER6en2tvXoKfpwYVbJ">
                            西湖是杭州最著名的景点，被誉为"人间天堂"。10月的西湖秋高气爽，湖面波光粼粼，两岸桂花飘香。<br data-page-node-id="lbFK5l7LTn7NmzzfwnN1Ro"><br data-page-node-id="HTQefib0sMlYgmKKxzCD4B">
                            <strong data-page-node-id="Fk5GMAwzyVNT3mjCBKZIl9">推荐路线：</strong>断桥残雪 → 白堤 → 孤山 → 苏堤春晓 → 花港观鱼
                        </div>
                        <div class="tag-group" data-page-node-id="wS9A2OZZIytSJINoMNUZzZ">
                            <span class="tag" data-page-node-id="hqccPQcPZMB40dYjPemlcr">🎫 免费开放</span>
                            <span class="tag" data-page-node-id="tkqEV8CTSUBDBFYN2XQCtk">🚶 步行或游船</span>
                            <span class="tag" data-page-node-id="Fr6FHvkrvuwSX5TdDs8jvK">📸 风景如画</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="1WdmiULTGe963CSFJJprLd">
                    <div class="timeline-dot" data-page-node-id="TncGcYEINnrGo3eyVtlbH0"></div>
                    <div class="timeline-time" data-page-node-id="D56I9lUoHwAdW1GnWBH6Gl">🕐 12:00 - 14:00</div>
                    <div class="timeline-title" data-page-node-id="5dUwVZLHkYYvVcqWMYA3nE">🍽️ 午餐 · 杭帮菜</div>
                    <div class="attraction-card" data-page-node-id="zvfdkD5InEFuE4hziMWenR">
                        <div class="attraction-header" data-page-node-id="Fj4UGPuHc4zJwsJfl3Sh4L">
                            <span class="attraction-icon" data-page-node-id="VnFwp9f5K7FSVxlH51WJmG">🍲</span>
                            <span class="attraction-title" data-page-node-id="jlzZNvYf1T7OUZBT82HbV2">西湖边杭帮菜</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="mlHkrrTZzJ0IRw8tObPwPN">
                            在西湖边品尝正宗杭帮菜，推荐东坡肉、西湖醋鱼、龙井虾仁等经典菜肴。
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="1ymOLEZNURp2cVinYEzZEF">
                    <div class="timeline-dot" data-page-node-id="KbjpIRhI67QsMxIj6uAQhi"></div>
                    <div class="timeline-time" data-page-node-id="yzGYZJxhedErJoTl9NcHcU">🕐 14:00 - 18:00</div>
                    <div class="timeline-title" data-page-node-id="rYz0pgIgVyMISSxz3SHuLI">🌸 西湖游览（下午）</div>
                    <div class="attraction-card" data-page-node-id="FceeCLyb5nJW2siXFKSQyW">
                        <div class="attraction-header" data-page-node-id="DeDzGEY7KjEAgCaKS2zHtS">
                            <span class="attraction-icon" data-page-node-id="6ISwJGEu7jXGx3VTMNNgBx">🚣</span>
                            <span class="attraction-title" data-page-node-id="NMyeKgzRwOKEKNAiJZHDvT">西湖游船</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="13dgyZ4qL7Nvo18UycuRBP">
                            乘坐西湖游船，欣赏湖光山色，感受"欲把西湖比西子，淡妆浓抹总相宜"的意境。<br data-page-node-id="NqCMKzKvHvNB2lR5kCxP2a"><br data-page-node-id="l2Fims5232mPPaZhaFYhdu">
                            <strong data-page-node-id="TN1rHtkvDay3fLGsSqgSUu">推荐：</strong>三潭印月（岛上游览）、雷峰塔（登高望远）
                        </div>
                        <div class="tag-group" data-page-node-id="tJ3HYWSdBeUKnXSsNcB86R">
                            <span class="tag" data-page-node-id="WxHIJOT6Y484jFVBG1Mo6w">🎫 游船约50元</span>
                            <span class="tag" data-page-node-id="D2hjURnonzwBBk2jt0i13m">⏱️ 约1小时</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="2sQok9rBk8XCKEYhkvVMKX">
                    <div class="timeline-dot" data-page-node-id="z5R4Sbm7mGklQ1HO4VAre9"></div>
                    <div class="timeline-time" data-page-node-id="KBqTJnkqbRviMXqSUmRCmx">🕐 18:00 - 19:00</div>
                    <div class="timeline-title" data-page-node-id="bukTYWTssh9DSABSF3EZHk">🚇 前往杭州东站</div>
                    <div class="transport-card" data-page-node-id="WbBPQ87BNk3gIc2HtVp3mB">
                        <div class="transport-header" data-page-node-id="s5Wc2vjZmPViy7XXhQzAhW">
                            <span class="transport-icon" data-page-node-id="khgWhJ5nAoIQhn8P9QNfwW">🚇</span>
                            <span class="transport-title" data-page-node-id="zcQoEbFn5STd263x2Mu0DI">地铁1号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="FExm3qe8qhjsAsNyDe4pvI">凤起路站(1号线) → 杭州东站</div>
                        <div class="transport-meta" data-page-node-id="gjNivJkASKdFdsoMRFAnhq">
                            <span data-page-node-id="StEwIDoIOOqlQESvYTlekF">⏱️ 约30分钟</span>
                            <span data-page-node-id="9EudLWrPg7NUBFA7fvAyab">💰 约4元</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="XaTo1wjZtdmWOjI1NLOn1c">
                    <div class="timeline-dot" data-page-node-id="e0sCGSBGYlktyUtBbOmGtD"></div>
                    <div class="timeline-time" data-page-node-id="7gSwnUmB7xMt6vH5zZ0Wxk">🕐 21:16 - 22:01</div>
                    <div class="timeline-title" data-page-node-id="PhQz6YpsGSARRRi5wVgcSh">🚄 杭州东 → 虹桥站</div>
                    <div class="transport-card" data-page-node-id="COcQRUYDOsXbWxXBaVoe1R">
                        <div class="transport-header" data-page-node-id="jRqcm3vQBMEg9oSBg90OSN">
                            <span class="transport-icon" data-page-node-id="VLEgdiE3JwmR0munxlitod">🚄</span>
                            <span class="transport-title" data-page-node-id="NA3TqiKWcBvfPdHnIjfdFX">高铁 G7548 / G7550</span>
                        </div>
                        <div class="transport-route" data-page-node-id="UFEl7qN97wzDMnVPaMqaxk">杭州东站 → 虹桥站</div>
                        <div class="transport-meta" data-page-node-id="MavmtmYu2zNE1Gyn2EZXjS">
                            <span data-page-node-id="A3aBHd5cwKCQMqHBeZ31RD">⏱️ 约45分钟</span>
                            <span data-page-node-id="pj98V6ruqt3tHMjhdhu8sA">💰 二等座约73元</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="rfG9VR8LyaUZdrHaCnRRQd">
                    <div class="timeline-dot" data-page-node-id="eJT32uMP6DlLhOaV6Bts3d"></div>
                    <div class="timeline-time" data-page-node-id="aR411TGeqlaDnjoZxPd4ES">🕐 22:30</div>
                    <div class="timeline-title" data-page-node-id="pKtwCc3kIASxnuRJLXT6wQ">🚇 返回朱梅路</div>
                    <div class="transport-card" data-page-node-id="Ps2xv8hCsQzvQSmGQUGlbc">
                        <div class="transport-header" data-page-node-id="QQ07tMtxzhRqeEeKgsYPNx">
                            <span class="transport-icon" data-page-node-id="jj4ERffTJO9EqGuDB2jFGe">🚇</span>
                            <span class="transport-title" data-page-node-id="yPk7UiqdMsK7SLVBciOK6u">地铁2号线 → 15号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="PCCLCrnovge9BCNVHS1DDC">虹桥火车站(2号线) → 人民广场(换乘1号线) → 常熟路(换乘15号线) → 朱梅路</div>
                        <div class="transport-meta" data-page-node-id="kPyDvsHzVsYOoaGhgoWDpX">
                            <span data-page-node-id="GBa2T9fkcFwmHqhjsYuxhr">⏱️ 约70分钟</span>
                            <span data-page-node-id="zkkIpv8Gpq5Hf2ECCbNxX5">💰 约7元</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- 美食推荐 -->
            <div class="food-section" data-page-node-id="xv17FaD6SPd5qBS36V7QsS">
                <div class="food-section-title" data-page-node-id="LBZCyXYQtHukRMAuCoeJPg">
                    <span data-page-node-id="yHQdo4oVC5jtg4tusJk8B2">🍲</span>
                    <span data-page-node-id="bHvVxnqDlU7g4aOJZezHrL">杭州西湖美食推荐</span>
                </div>
                <div class="food-grid" data-page-node-id="nCFFznFD6F0cpoHRWWiPBE">
                    <div class="food-card" data-page-node-id="tpKw2TzHD6eTvDZ3iHFTBd">
                        <div class="food-card-header" data-page-node-id="uCbuWXecHexziCQjwhluGZ">
                            <span class="food-name" data-page-node-id="3hVfSu9NbGF93BGqzONTu1">外婆家(白堤店)</span>
                            <span class="food-price" data-page-node-id="GByuEo4MlHf5cdALmKtz95">人均54元</span>
                        </div>
                        <div class="food-type" data-page-node-id="gFjXqSPVgoCEeCMKUMDIwb">🥘 杭帮菜</div>
                        <div class="food-address" data-page-node-id="QWta30snmT55A9QwVfAUCY">📍 孤山路28号</div>
                        <div class="food-recommend" data-page-node-id="9AOBlZInnKEuxTFrfXZElS">⭐ 推荐：茶香鸡、糖醋里脊、东坡肉</div>
                    </div>
                    <div class="food-card" data-page-node-id="XLSGeAEC33Fj7Zirs3hDgA">
                        <div class="food-card-header" data-page-node-id="6KiQ3yei0qkg2OZU36iKaP">
                            <span class="food-name" data-page-node-id="mG4OhAdFqvZJ0fBGDkRXxc">绿茶餐厅(灵隐店)</span>
                            <span class="food-price" data-page-node-id="7DiUVYSfDubI7qYwNXZr9Y">人均85元</span>
                        </div>
                        <div class="food-type" data-page-node-id="RmzXcaRFGKmE7XbHCoFC8r">🥘 杭帮菜</div>
                        <div class="food-address" data-page-node-id="9vjgsRbgOBCB5tlzN1O55r">📍 灵隐路1号</div>
                        <div class="food-recommend" data-page-node-id="WGeukz7rIPCBLfmWmVfLGr">⭐ 推荐：油爆虾、绿茶饼、面包诱惑</div>
                    </div>
                    <div class="food-card" data-page-node-id="8uXfCE2luDegLZuKrDkTtE">
                        <div class="food-card-header" data-page-node-id="bY8PwZluzuO54DE4U8TqB0">
                            <span class="food-name" data-page-node-id="r0mFRomKkVlDy8RGzjbK7R">知味观(湖滨店)</span>
                            <span class="food-price" data-page-node-id="rmVEixtCwiuZpBhoGnLme9">人均150元</span>
                        </div>
                        <div class="food-type" data-page-node-id="tRYBc1gV9VzxEiz9vjKdWN">🥟 老字号</div>
                        <div class="food-address" data-page-node-id="h9w8H067ApJu4WGPgMlXaR">📍 仁和路83号</div>
                        <div class="food-recommend" data-page-node-id="CfnTq9LJUTGFJRinMWzq8Z">⭐ 推荐：小笼包、龙井虾仁、东坡肉</div>
                    </div>
                    <div class="food-card" data-page-node-id="GFiXq7R9LZ48v8K687dLyh">
                        <div class="food-card-header" data-page-node-id="MBFHiScgOzBcwdIcBRYlfh">
                            <span class="food-name" data-page-node-id="XgGtKP9Hac0lbPa2hrRNM7">新白鹿餐厅</span>
                            <span class="food-price" data-page-node-id="yb7g2IflaMP5ctc8eqDi2L">人均120元</span>
                        </div>
                        <div class="food-type" data-page-node-id="5KBbNLMkXIPDVy5BEUH0K1">🥘 杭帮菜</div>
                        <div class="food-address" data-page-node-id="j7ld4IGEPDLG7dsfkchZ3A">📍 龙游路56号</div>
                        <div class="food-recommend" data-page-node-id="zQHmlhqXNgE2UZleinI6cM">⭐ 推荐：乾隆鱼头、蛋黄南瓜、糖醋排骨</div>
                    </div>
                    <div class="food-card" data-page-node-id="jToJfqmZzVGn01bXmQQIa3">
                        <div class="food-card-header" data-page-node-id="dEUr82U2cKHx9Ll0TbE4LB">
                            <span class="food-name" data-page-node-id="kQD6JO0vni9pkN3vG4lOiQ">朴墅餐厅(青芝坞)</span>
                            <span class="food-price" data-page-node-id="6XxLFtRV0Gf8HauxGkiHCZ">人均111元</span>
                        </div>
                        <div class="food-type" data-page-node-id="gwL11HLl0WLxe3Qhf2vRfv">🥘 杭帮菜</div>
                        <div class="food-address" data-page-node-id="FzuHVDdRIt3wFOm8BXH4Bo">📍 玉古路61-1号</div>
                        <div class="food-recommend" data-page-node-id="FQZTo8DbaPNEie6XtHC4v7">⭐ 推荐：西湖龙井虾仁，环境文艺</div>
                    </div>
                    <div class="food-card" data-page-node-id="4yvuZjW1HnRaSCNjc83fv0">
                        <div class="food-card-header" data-page-node-id="8e1fuYSeZhgewhYiyPMZSg">
                            <span class="food-name" data-page-node-id="a5dqK6YEymaPBC5So6eVnd">四季盛宴</span>
                            <span class="food-price" data-page-node-id="kKz4yB3chNFlunXXcTotAt">人均199元</span>
                        </div>
                        <div class="food-type" data-page-node-id="k35xCLhEKeaWsLUPox1KEi">🥘 高档杭帮菜</div>
                        <div class="food-address" data-page-node-id="vSTZQ5gzCtoMIrvhxnNq7d">📍 灵隐路1号2楼</div>
                        <div class="food-recommend" data-page-node-id="rOy6YBLJbhGLokEUdJa5Pv">⭐ 推荐：环境优雅，适合宴请</div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- ==================== DAY 5 ==================== -->
        <div class="day-card day-5" data-page-node-id="IMkW94erp648PYflybotnd">
            <div class="day-header" data-page-node-id="2oC49kJHre88Ln3WxbYGqN">
                <div class="day-number" data-page-node-id="E5rKPOYj4XGrvbDP63BCw2">D5</div>
                <div class="day-title" data-page-node-id="9X5S5Wu6Xbj3Gl9AkL2C1K">
                    <h2 data-page-node-id="UiGY8VYrULGGc4FAyqamnI">10月5日 · 苏州园林一日游</h2>
                    <p class="day-theme" data-page-node-id="zdncsmewsySh7KPmHWHDMl">🎯 主题：园林艺术 · 姑苏韵味</p>
                </div>
                <div class="day-weather" data-page-node-id="k2tPlKymedHcaNxaF8MtJZ">🏯 江南园林甲天下</div>
            </div>
            
            <div class="timeline" data-page-node-id="5qwEjGxrEZKpHtQiF91DYH">
                <div class="timeline-item" data-page-node-id="lfpg6EkumwrS6n4jdAzHYN">
                    <div class="timeline-dot" data-page-node-id="NptV4DK6kyz4hhoffc2YoJ"></div>
                    <div class="timeline-time" data-page-node-id="nLYjWYYP44E6DWfiVJpBOi">🕐 07:00</div>
                    <div class="timeline-title" data-page-node-id="eYsj8l58geO4PZCeA7okXZ">🚇 朱梅路 → 虹桥站</div>
                    <div class="transport-card" data-page-node-id="ok9XkZaKm3uyD1UHRhIArX">
                        <div class="transport-header" data-page-node-id="StybasdhErZ8k0oHvEJgp7">
                            <span class="transport-icon" data-page-node-id="XGCZxhRzbSRfAtW2ZKMnPc">🚇</span>
                            <span class="transport-title" data-page-node-id="UyBF3Jta98O7yDZ8oV5tkD">地铁15号线 → 2号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="rdMHo8GKPEelTeYMzshATk">朱梅路(15号线) → 桂林公园(换乘9号线) → 陆家浜路(换乘10号线) → 虹桥2号航站楼(换乘2号线) → 虹桥火车站</div>
                        <div class="transport-meta" data-page-node-id="UncjneWw0DPOWuB1nbjjM4">
                            <span data-page-node-id="MdCxosJO7uSLC15YEb1MAH">⏱️ 约70分钟</span>
                            <span data-page-node-id="ecFHEUkD4PRZGf12nG9CwW">💰 约7元</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="VwHW0VppEaSgF4PTleIqCs">
                    <div class="timeline-dot" data-page-node-id="rH2ZEIvEZTaFGNUFhA902p"></div>
                    <div class="timeline-time" data-page-node-id="HgSGdyXsPzWTtqjJrb8c3i">🕐 08:52 - 09:22</div>
                    <div class="timeline-title" data-page-node-id="gP9Ko0B3z97XwYo1ownSil">🚄 虹桥站 → 苏州站</div>
                    <div class="transport-card" data-page-node-id="db5AtLYzlB3LsX8kjqjg83">
                        <div class="transport-header" data-page-node-id="Of4aQeKwyMmU8UENBM7mDt">
                            <span class="transport-icon" data-page-node-id="H1qHokv0gZDytOnRBLnTKN">🚄</span>
                            <span class="transport-title" data-page-node-id="FBd3NILwOw29qPBAKZJxB1">高铁 G7503 / G7505</span>
                        </div>
                        <div class="transport-route" data-page-node-id="xv5x9KeX582UwnHs2uwysF">虹桥站 → 苏州站</div>
                        <div class="transport-meta" data-page-node-id="vkAONoPPLhP1A0vHvLi2gN">
                            <span data-page-node-id="v97WE6XaOomnSDYZHhvPNc">⏱️ 约30分钟</span>
                            <span data-page-node-id="7mgqRIE7rVWZDJU4cqIZxg">💰 二等座约40元</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="QNzutYZ8CVjdI444xmH75Q">
                    <div class="timeline-dot" data-page-node-id="skxaDhNtL12oL96fVgxK2T"></div>
                    <div class="timeline-time" data-page-node-id="Dvcbze8Gxpij25CIO7QWxc">🕐 09:30 - 10:00</div>
                    <div class="timeline-title" data-page-node-id="kPf4sULeD5Itlpn3vn6qVR">🚇 苏州站 → 西园寺</div>
                    <div class="transport-card" data-page-node-id="ia4rlAJI7l9ZryTQT8XF0B">
                        <div class="transport-header" data-page-node-id="FCDD9JPAVfj6v8Tjqe6hVS">
                            <span class="transport-icon" data-page-node-id="2oz1BVILNVChDiEMehwzCM">🚇</span>
                            <span class="transport-title" data-page-node-id="s4XmJh7VETY9BaD6jdNIyw">地铁4号线 → 2号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="TKr1V52EG7e1ifJQw2hbG2">苏州站(4号线) → 广济南路(换乘2号线) → 三香广场站(3号口出)</div>
                        <div class="transport-meta" data-page-node-id="7tYh2iZeeTUaBB3ke7nJPE">
                            <span data-page-node-id="zvnV8huEAk47t81xfn7Cjd">⏱️ 约25分钟</span>
                            <span data-page-node-id="JcSrlmrsQ7UewcI12d0ipG">💰 约3元</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="ZvGPaUXAMDRkiAfumhkwNL">
                    <div class="timeline-dot" data-page-node-id="pQXxWDy1eACHJUi05qSn2R"></div>
                    <div class="timeline-time" data-page-node-id="CyohQXcF9vXw6iFLOTIMDN">🕐 10:00 - 12:00</div>
                    <div class="timeline-title" data-page-node-id="lpJZHpv6P7R91UftVZUJCe">🏯 西园寺</div>
                    <div class="attraction-card" data-page-node-id="tmiOmlW9PjyxDB6XcOsEVZ">
                        <div class="attraction-header" data-page-node-id="QDG3uwbtDQC4EOFiALjcmu">
                            <span class="attraction-icon" data-page-node-id="mT2iPPIZBi1Wv5eSJ1Eejg">🏯</span>
                            <span class="attraction-title" data-page-node-id="jmJskMtIDkygyj8oN40E0v">西园寺 · 千年古刹</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="2m066rOV8MqfhA0LlmkWmS">
                            西园寺是苏州著名的佛教寺院，始建于南朝梁代，距今已有1500多年历史。寺内建筑宏伟，环境清幽，是闹市中的一片净土。<br data-page-node-id="dgbN7rYKnxZCfts80A4vbM"><br data-page-node-id="ErOaWAmQUUZsroYBREVdA5">
                            <strong data-page-node-id="onvqTkjENoXsoWxBucJxvL">必看：</strong>观音殿、大雄宝殿、藏经楼、素斋馆
                        </div>
                        <div class="tag-group" data-page-node-id="Yf0p1eworEecDTLqEqtZXF">
                            <span class="tag" data-page-node-id="cipsHIFbnIg4fwrSnrs7CA">🎫 门票约20元</span>
                            <span class="tag" data-page-node-id="7McOhRuTY732SeT2eR9G6e">⏱️ 建议1-2小时</span>
                            <span class="tag" data-page-node-id="Tt0QDCEXG98QvC3AyTsU2s">🙏 祈福圣地</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="1Tjx2TBHRApNFi8oRNsoo2">
                    <div class="timeline-dot" data-page-node-id="SQ8pOG0nWbWKbTrjuEFA5X"></div>
                    <div class="timeline-time" data-page-node-id="iDFFnXZsNf8MEfJI60RRoF">🕐 12:00 - 13:00</div>
                    <div class="timeline-title" data-page-node-id="s9VHYvEAQxVWrOwkKPzfH3">🍜 西园寺素面</div>
                    <div class="attraction-card" data-page-node-id="j33qohkKccD5TLSJZtNIOL">
                        <div class="attraction-header" data-page-node-id="DwIYFxJaGb4bMAHROcVYrQ">
                            <span class="attraction-icon" data-page-node-id="3R7AkGnBPBQ8AWWLat66Ok">🍜</span>
                            <span class="attraction-title" data-page-node-id="7GsYOgaUV2cy8fExsuVKA0">西园寺素斋馆</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="F4VCaqBmx0HPLPjW1QnLmQ">
                            西园寺的素面是苏州著名的美食，15元一碗的观音面是招牌。浇头丰富，有香菇、笋片、面筋、木耳等，汤底用菌菇熬制，鲜美可口。
                        </div>
                        <div class="tag-group" data-page-node-id="qEcqYkEAgOwOFP5zg5nlBI">
                            <span class="tag" data-page-node-id="j8NFKfrVijHdxfFhFRxsiT">💰 观音面15元</span>
                            <span class="tag" data-page-node-id="LFJWtCAttooJERiAzZEhG0">⭐ 必吃推荐</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="pmPscPUk9OytwDHxLuB5Rw">
                    <div class="timeline-dot" data-page-node-id="L9wuSXNx1P67rs9WZHpU0H"></div>
                    <div class="timeline-time" data-page-node-id="1wRwLDePXhehQL3Fq8XEY3">🕐 13:30 - 15:30</div>
                    <div class="timeline-title" data-page-node-id="45TpQJjiMNEdpC5vMXL2OT">🏞️ 留园</div>
                    <div class="attraction-card" data-page-node-id="6LzH4eFtdiPFfBvEQ7x2pY">
                        <div class="attraction-header" data-page-node-id="KENt6BlO2CTFECVvq6GuFB">
                            <span class="attraction-icon" data-page-node-id="8mJFZ8Vu8GFZ2zyY6CAu6q">🏞️</span>
                            <span class="attraction-title" data-page-node-id="Kme8oQn2vQ7BV0xFDOQXFU">留园 · 中国四大名园</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="LS4xD4TvPdS1vcMDQZ151B">
                            留园是中国四大名园之一，以建筑空间处理精湛著称。园内布局紧凑，设计精巧，通过借景、框景等手法，营造出丰富的空间层次。<br data-page-node-id="GgnkstiPPZBu6dPkHW0Sk9"><br data-page-node-id="CKz5lzmXoZM7l6LMDmBdDI">
                            <strong data-page-node-id="Ps9VGOTMaEpxG3uBjvw65B">必看：</strong>冠云峰、林泉耆硕之馆、五峰仙馆、揖峰指柏轩
                        </div>
                        <div class="tag-group" data-page-node-id="0whVLB5e5IDhsYkB27fZu5">
                            <span class="tag" data-page-node-id="uirxHXUC6FIuLQ0a26ACE0">🎫 门票约55元</span>
                            <span class="tag" data-page-node-id="ePyHM2AOrvFSg8CvKFyL9V">⏱️ 建议2小时</span>
                            <span class="tag" data-page-node-id="D3UZPaZRKs4rNrYUGPbkjc">🏆 世界遗产</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="QDzUafBYN60eukOaG0gkGa">
                    <div class="timeline-dot" data-page-node-id="P2VPo39Vc33THNEoRuw2ll"></div>
                    <div class="timeline-time" data-page-node-id="bLC8KKU7HIA12i3D08Hxhs">🕐 16:00 - 18:00</div>
                    <div class="timeline-title" data-page-node-id="nsG1C3Xqh98aT7kwXvbdRp">⛰️ 虎丘</div>
                    <div class="attraction-card" data-page-node-id="NwLjxe1YpFCev06K9Dt0L7">
                        <div class="attraction-header" data-page-node-id="WuZYeDzrQBZL58yxGGmJnb">
                            <span class="attraction-icon" data-page-node-id="Cjn6J8b2iBUwZxSp3IhtMX">⛰️</span>
                            <span class="attraction-title" data-page-node-id="XfWZq38EZcdgSjuJJFCkZl">虎丘 · 吴中第一名胜</span>
                        </div>
                        <div class="attraction-desc" data-page-node-id="gwKjBnqv3kAGMN5BPLl4i8">
                            虎丘是苏州的标志性景点，素有"吴中第一名胜"的美誉。虎丘塔是中国的"比萨斜塔"，已有千年历史，是苏州的象征。<br data-page-node-id="LMAFNCciKRK7lsR9EQKSgY"><br data-page-node-id="XG32tC2V4HaCvNyd3eRIUF">
                            <strong data-page-node-id="q4WunUbTWxHnBkWmwmrq4H">必看：</strong>虎丘塔、剑池、试剑石、拥翠山庄
                        </div>
                        <div class="tag-group" data-page-node-id="9kGnV7v0jkhjjsCDqPCMby">
                            <span class="tag" data-page-node-id="f1VyqOuiicWz5GxxgOe2al">🎫 门票约60元</span>
                            <span class="tag" data-page-node-id="gukFDPN5FEb5vFIMoJc5wH">⏱️ 建议2小时</span>
                            <span class="tag" data-page-node-id="oMtD2VTCd05uimR2wPUgwe">📸 拍照胜地</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="FjTOJzuGIJoIqGogUDNdCp">
                    <div class="timeline-dot" data-page-node-id="l2FYksf32FNWoNbB9nrXzJ"></div>
                    <div class="timeline-time" data-page-node-id="zbe0EcLh18gUi5uH60wGdf">🕐 18:30 - 19:30</div>
                    <div class="timeline-title" data-page-node-id="2HMNlHeLCfM0FDmR2txcmB">🚇 返回苏州站</div>
                    <div class="transport-card" data-page-node-id="OorMelQ2cebkP2xx8azozp">
                        <div class="transport-header" data-page-node-id="4umBFjGGp85cMFAOt3BhCA">
                            <span class="transport-icon" data-page-node-id="DEREM4u9quCAPZVpEGtise">🚇</span>
                            <span class="transport-title" data-page-node-id="FKvtGNHCbpE40DNkIJicvO">地铁2号线 → 4号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="EU32HpAGijtY2spGRLvMbp">三香广场站(2号线) → 广济南路(换乘4号线) → 苏州站</div>
                        <div class="transport-meta" data-page-node-id="sw8AaDEuqiMepYIdkvPhIR">
                            <span data-page-node-id="CbqW2RM5OepejNCE41A3Gi">⏱️ 约25分钟</span>
                            <span data-page-node-id="BP9dRJpVIhW1GP3ZMBnFAI">💰 约3元</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="sJ6x071HynBuaBkhJYYYoh">
                    <div class="timeline-dot" data-page-node-id="5ca9qdvloZ3HdxTXly7khB"></div>
                    <div class="timeline-time" data-page-node-id="ODSz4ZvWUS8e94U6THyrNs">🕐 21:48 - 22:18</div>
                    <div class="timeline-title" data-page-node-id="fxA5yNEAoRqlhNDhF4AypT">🚄 苏州站 → 虹桥站</div>
                    <div class="transport-card" data-page-node-id="spJdOm6Z6vwZvLtpt8sZ0O">
                        <div class="transport-header" data-page-node-id="dxDHG0tZVtSYKgzFnnHmQQ">
                            <span class="transport-icon" data-page-node-id="BHGOuE8ZNsA1dvtgLDAQQj">🚄</span>
                            <span class="transport-title" data-page-node-id="71XkUTvYUVXnYeEwKbzdNx">高铁 G7590 / G7592</span>
                        </div>
                        <div class="transport-route" data-page-node-id="Od7RpqW5areLCRSuUvLBAB">苏州站 → 虹桥站</div>
                        <div class="transport-meta" data-page-node-id="CTOw5YiQzhtOb9waeU5LkB">
                            <span data-page-node-id="xQbyFv3XGlaabAJx5nxDZL">⏱️ 约30分钟</span>
                            <span data-page-node-id="OvifDIAayy1amdBVyYhQEh">💰 二等座约40元</span>
                        </div>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="xGO31aSOsUhpTXDZlBdhvv">
                    <div class="timeline-dot" data-page-node-id="UuD4dNZDdCVbRSeGae8bWs"></div>
                    <div class="timeline-time" data-page-node-id="gx5GKhDprFGfn6Yh5c4X5v">🕐 22:30</div>
                    <div class="timeline-title" data-page-node-id="tjAEzZbNfLdZnVYJWsjFe4">🚇 返回朱梅路</div>
                    <div class="transport-card" data-page-node-id="dxLaCyMOI2VyaBwdCDU22U">
                        <div class="transport-header" data-page-node-id="MlJXTyL3xmZXlu983gc9kJ">
                            <span class="transport-icon" data-page-node-id="rnWthl1YWBAXgPNXvaRqkq">🚇</span>
                            <span class="transport-title" data-page-node-id="k9BFiOGwKq4fYn7BbebTsI">地铁2号线 → 15号线</span>
                        </div>
                        <div class="transport-route" data-page-node-id="Nc5u2A1crNLtAU7CKH6ZpE">虹桥火车站(2号线) → 人民广场(换乘1号线) → 常熟路(换乘15号线) → 朱梅路</div>
                        <div class="transport-meta" data-page-node-id="2KJYyzQWYJheD6xDCzHdVR">
                            <span data-page-node-id="1oXkdAEtG9xbBLhs0UGDnM">⏱️ 约70分钟</span>
                            <span data-page-node-id="PmA6PbcC3ocUKT7pYkBJKQ">💰 约7元</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- 美食推荐 -->
            <div class="food-section" data-page-node-id="2BayG9ywch6KG6z9flhXAF">
                <div class="food-section-title" data-page-node-id="inT9uZQuXzzVUNIInFNlJb">
                    <span data-page-node-id="WvJMaFrkMjU4p2HSAdldCh">🍜</span>
                    <span data-page-node-id="9P874a1UXxSGcUhObA0jAC">苏州美食推荐</span>
                </div>
                <div class="food-grid" data-page-node-id="ysnMTyRfqQBFp24c86K1mM">
                    <div class="food-card" data-page-node-id="TIZrnQbu7G8ArBcoKAeIh6">
                        <div class="food-card-header" data-page-node-id="CYmSPrM6iu591sp50BxneJ">
                            <span class="food-name" data-page-node-id="lsUe1X9yvCKAHumKfxg3of">西园寺素面</span>
                            <span class="food-price" data-page-node-id="yeklxnlMCvTVejMutJA73H">人均15元</span>
                        </div>
                        <div class="food-type" data-page-node-id="3tfS7sUSbtMLIxoG9QTLTo">🍜 素斋</div>
                        <div class="food-address" data-page-node-id="g1v8sjHCpZBEOsqV8rU6KK">📍 西园寺内</div>
                        <div class="food-recommend" data-page-node-id="Fg30dGM7FS2gukSRQIir0K">⭐ 推荐：观音面15元，浇头丰富，鲜美可口</div>
                    </div>
                    <div class="food-card" data-page-node-id="5JdRPDVMS6FSqslHFmOxcN">
                        <div class="food-card-header" data-page-node-id="GWcx8hI5CDs7A1c39XVCr8">
                            <span class="food-name" data-page-node-id="E3zTvL2FsKbsnH7YiiyAC4">老石头面馆</span>
                            <span class="food-price" data-page-node-id="8RetQlOhEnWDct55cNhAIs">人均18元</span>
                        </div>
                        <div class="food-type" data-page-node-id="HM3WVVZFoGQJFU3x1wAGuw">🍜 苏式面</div>
                        <div class="food-address" data-page-node-id="dpXQ3G1BhNqKZE3E8tUnIi">📍 留园路附近</div>
                        <div class="food-recommend" data-page-node-id="mrs48nBtYM2Ngu6QQKEeXD">⭐ 推荐：爆鱼面18元，爆鱼酥脆</div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- ==================== DAY 6 ==================== -->
        <div class="day-card day-6" data-page-node-id="YZbe9UfP9utkXppHMq61ad">
            <div class="day-header" data-page-node-id="hUiHDIKl8ZpqLwrfOZQxM6">
                <div class="day-number" data-page-node-id="295IaVMX81oJfgBo4JYMzp">D6</div>
                <div class="day-title" data-page-node-id="Thz0YpSBAVzDxk9m8qBD0C">
                    <h2 data-page-node-id="20b7ULlJ7IqObFuFyAgAjT">10月6日 · 返程</h2>
                    <p class="day-theme" data-page-node-id="o0KomFimSAfwBFtZhokcvY">🎯 主题：整理行装 · 温馨返程</p>
                </div>
                <div class="day-weather" data-page-node-id="YNA9J6pdChKu2596fwgRWJ">🏠 回家</div>
            </div>
            
            <div class="timeline" data-page-node-id="UjlPK487WDowkBSftTAfb5">
                <div class="timeline-item" data-page-node-id="GFdKhsYFpEON14vcbg7Cs0">
                    <div class="timeline-dot" data-page-node-id="jrbCs9tvvOHPAvCAkMECrO"></div>
                    <div class="timeline-time" data-page-node-id="KE5k6yddq8YryKSEoZdAOt">🕐 上午</div>
                    <div class="timeline-title" data-page-node-id="yGuzr4iwGB9lmtf0m77JYV">🏠 整理行装</div>
                    <div class="timeline-content" data-page-node-id="uqQxjHNhvzg1c7Gkk7ZG4G">
                        <p data-page-node-id="ecbuRPHCBIYOo09BRrG9cU">在朱梅路住处整理行李，准备返程。可以适当休息，为旅途画上圆满句号。</p>
                    </div>
                </div>
                
                <div class="timeline-item" data-page-node-id="BE1Y9agcBSQx9irCRQ6gG4">
                    <div class="timeline-dot" data-page-node-id="ileNbPzT981A6WBFqRDlUX"></div>
                    <div class="timeline-time" data-page-node-id="uhM1W2XYe0rDk5iYMsKjBO">🕐 下午</div>
                    <div class="timeline-title" data-page-node-id="PwcvJ9ihqBrGpiF4Gz4d6Z">🚇 前往火车站/机场</div>
                    <div class="transport-card" data-page-node-id="uBASvk1s6cUGjzUyaKA5cz">
                        <div class="transport-header" data-page-node-id="tM7zV6Wg4jpOLYbur91kAw">
                            <span class="transport-icon" data-page-node-id="BWavN9qIrseP30c5lqLD2w">🚇</span>
                            <span class="transport-title" data-page-node-id="86TKgwFleiuwBIHZ7q3nbH">地铁路线（根据实际出发）</span>
                        </div>
                        <div class="transport-route" data-page-node-id="hZ65aldRJ97PrWbnkSCtQg">朱梅路 → 虹桥火车站/虹桥机场</div>
                        <div class="transport-meta" data-page-node-id="x95PEoL1AEBzGHWiQNuUHI">
                            <span data-page-node-id="rRF4w05vsGdK5k12eLxZKQ">⏱️ 约70分钟</span>
                            <span data-page-node-id="FdXR8QNGSiT8R4RfJYgfsH">💰 约7元</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="tip-box" data-page-node-id="VxSgkhtIvU6SICmDPkZqVW">
                <div class="tip-header" data-page-node-id="1vC03D85RUYxEasKxDttHE">
                    <span class="tip-icon" data-page-node-id="NlOiNik4ddwlfaFER0eFIf">💡</span>
                    <span class="tip-title" data-page-node-id="C3Gamj9OJn8Qx9DSMGCLgM">返程提示</span>
                </div>
                <div class="tip-content" data-page-node-id="MmoLDEdFe0FvzeBZDLe2HT">
                    建议提前2小时到达火车站/机场，预留充足时间办理乘车手续。
                </div>
            </div>
        </div>
        
        <!-- 预算参考 -->
        <div class="day-card" data-page-node-id="7ELBQy53C9v55m2BNNgTzJ">
            <div class="day-header" data-page-node-id="MoUCliOoOt2AdC9lm6wAW7">
                <div class="day-number" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);" data-page-node-id="buOfx73ZKf8wLEgX0wj6WA">💰</div>
                <div class="day-title" data-page-node-id="Yej90jQWNRdtvY0teqD8Js">
                    <h2 data-page-node-id="Barj7RtUK7GcsUy6gH6Bn0">预算参考</h2>
                    <p class="day-theme" data-page-node-id="5JPG57WjT3DsCzSxQS98PK">人均费用估算</p>
                </div>
            </div>
            
            <div class="two-columns" data-page-node-id="3hucvwNFwRDBlnnzngiFbB">
                <div data-page-node-id="egBAlQlnnS1tTyYRfwYT4M">
                    <h4 style="margin-bottom: 15px; color: var(--primary-color);" data-page-node-id="blziGcJF1uS2bkwFqWdVg2">🚇 交通费用</h4>
                    <div class="timeline-content" style="background: var(--bg-light);" data-page-node-id="frWh5WOpnO5X1g2AX0FRCE">
                        <p data-page-node-id="yRHt87gJvE08MyZtx0igX0">• 上海市内地铁：约50元</p>
                        <p data-page-node-id="9XvtsRP5R3hfa7GWTaco1R">• 虹桥↔杭州高铁：约146元</p>
                        <p data-page-node-id="DKmNVPdbQXRTbplhrcvZBl">• 虹桥↔苏州高铁：约80元</p>
                        <p data-page-node-id="khNwh6HEnNkgnxZRtPVAIc">• 杭州/苏州地铁：约30元</p>
                        <p style="font-weight: 600; color: var(--primary-color); margin-top: 10px;" data-page-node-id="FXTUDFyUUfsXQlEL2r0MIg">交通小计：约306元</p>
                    </div>
                </div>
                <div data-page-node-id="85EwAtySWy7uHV6xBf9dKn">
                    <h4 style="margin-bottom: 15px; color: var(--accent-color);" data-page-node-id="NytK3PO9n2uyno6R0HPACH">🎫 景点门票</h4>
                    <div class="timeline-content" style="background: var(--bg-light);" data-page-node-id="94HBVzadujrRtZoG1f6yoZ">
                        <p data-page-node-id="VWIUV8jKOaBppEtBAJtVoy">• 东方明珠：约120元</p>
                        <p data-page-node-id="46Hh1mg8pPXSyAX2u6EACo">• 西湖游船：约50元</p>
                        <p data-page-node-id="uWKlyUXsJCHOJYjuRjokIF">• 西园寺：约20元</p>
                        <p data-page-node-id="WySZrQYefJC9WF6BCGmJ9J">• 留园：约55元</p>
                        <p data-page-node-id="jz1q3qHbShCIGxRF3Fq2DV">• 虎丘：约60元</p>
                        <p style="font-weight: 600; color: var(--accent-color); margin-top: 10px;" data-page-node-id="PETbP0rWwEgHTMQT8sK0Zg">门票小计：约305元</p>
                    </div>
                </div>
            </div>
            
            <div style="margin-top: 20px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 20px; border-radius: 12px; text-align: center;" data-page-node-id="qU5mKeEzQaYxCYtmD9S3zR">
                <p style="font-size: 18px; font-weight: 600;" data-page-node-id="ThAxEtyhQJMNDskD6JmTHn">💰 人均总预算（不含住宿和餐饮）</p>
                <p style="font-size: 36px; font-weight: 700; margin: 10px 0;" data-page-node-id="hjqTOUh5F3qwFXHlZGBiWw">约 611 元</p>
                <p style="opacity: 0.9;" data-page-node-id="Ir51NzNb4A7GKA7GAcCWiG">餐饮人均约500-800元（6天）| 住宿视酒店档次而定</p>
            </div>
        </div>
        
        <!-- 实用提示 -->
        <div class="day-card" data-page-node-id="Xut7Zo0gIlwFwN5Q2j5Kvf">
            <div class="day-header" data-page-node-id="UkypK1LPOD4rFKizrnaVtw">
                <div class="day-number" style="background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);" data-page-node-id="LFj9xBHDHGbyGzgtscl9My">📝</div>
                <div class="day-title" data-page-node-id="ocoRPeoD3a4TF3lQ7oYpP3">
                    <h2 data-page-node-id="BMBA5hdOR0PgBuKajcp3be">实用提示</h2>
                    <p class="day-theme" data-page-node-id="yTNbg8B7cSp1rbqt1ataGB">出行前必读</p>
                </div>
            </div>
            
            <div class="two-columns" data-page-node-id="48XtapvBWNAzRxumUGDxne">
                <div class="tip-box" data-page-node-id="UhtwoFUpVvL0Z5HByRaPCy">
                    <div class="tip-header" data-page-node-id="HCpTdgOpawMTomZLcE3o2z">
                        <span class="tip-icon" data-page-node-id="ZQ38nrwrvszE9CohEFylXI">📱</span>
                        <span class="tip-title" data-page-node-id="QDkoLJ5sinA1qGCBhOXZof">必备APP</span>
                    </div>
                    <div class="tip-content" data-page-node-id="Klz6AJvYrZ0nNQzdjhFPqw">
                        • 地铁：Metro大都会（上海）、杭州地铁、苏e行<br data-page-node-id="tObWu80y3oFHIdlOhy2iwE">
                        • 高铁：12306<br data-page-node-id="fzFeiZCf8fjorG390ruiLR">
                        • 打车：滴滴出行<br data-page-node-id="yG1bUF1CSeNfPzi4VayZHj">
                        • 美食：大众点评
                    </div>
                </div>
                <div class="tip-box" data-page-node-id="lB5CvGpzC8zPHcdMkJoYQI">
                    <div class="tip-header" data-page-node-id="MgMtQ2EcABVMSdKV64NuQF">
                        <span class="tip-icon" data-page-node-id="8nbQasHyq3Z2PL4LA2ND1o">🎒</span>
                        <span class="tip-title" data-page-node-id="bRtNBhGVCzl9cijULBWwx5">行前准备</span>
                    </div>
                    <div class="tip-content" data-page-node-id="vjALne9WgTJgXWpLPKAs0F">
                        • 身份证（乘车、购票必备）<br data-page-node-id="IkdLg60hBbRb1TbPCQ3W0f">
                        • 充电宝、数据线<br data-page-node-id="SMs8hvwcyjCXVBE5Hv6w9r">
                        • 薄外套（10月早晚温差大）<br data-page-node-id="Fq5pOAoLHcXexachdAwvIm">
                        • 舒适步行鞋<br data-page-node-id="LMeH9ygkF9YY2EaKSj9gKC">
                        • 常用药品
                    </div>
                </div>
            </div>
            
            <div class="tip-box" style="margin-top: 15px;" data-page-node-id="KWkoEdNDq9wtTb048c4bXC">
                <div class="tip-header" data-page-node-id="fI9lhuX55BoiHhvpFyCVuU">
                    <span class="tip-icon" data-page-node-id="sXJDLHsEd6ECFReyPShMQx">⚠️</span>
                    <span class="tip-title" data-page-node-id="HvdYgxBX0MshhzSP0luLhT">安全提示</span>
                </div>
                <div class="tip-content" data-page-node-id="t4KbM6Ap8y1sGm0XSdariZ">
                    • 国庆期间景点人多，注意保管好随身物品<br data-page-node-id="yiFHlvUHZOADKoMK38wT7S">
                    • 乘坐地铁时注意脚下安全，站稳扶好<br data-page-node-id="L9ZgjguwoC0awVAnwQTs6l">
                    • 高铁乘车请提前到达车站，预留充足时间<br data-page-node-id="JN7uW9cazkOx8HGz4DDQNC">
                    • 品尝美食时注意饮食卫生
                </div>
            </div>
        </div>
        
        <!-- 页脚 -->
        <div class="footer" data-page-node-id="cDpI9TAZozgS3PVVJgfBCB">
            <p data-page-node-id="MSk0r6xlmAIXNZee0veFe2">📅 上海及周边六日游行程攻略 | 10月1日-10月6日</p>
            <p style="margin-top: 10px;" data-page-node-id="ck5Wioqq9YA7hbXJBMQuT0">祝您旅途愉快！🌟</p>
        </div>
    </div>
</body>
</html>
