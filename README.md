# haidswine
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>牧知汇 - 猪群健康管理</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Inter', sans-serif;
            background-color: #fafcf8;
            color: #1e2a1f;
            line-height: 1.5;
        }
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 24px;
        }
        .top-bar {
            background-color: #ffffff;
            border-bottom: 1px solid #e2e8c3;
            padding: 16px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            background-color: rgba(255, 255, 255, 0.96);
        }
        .nav-wrapper {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            flex-wrap: wrap;
            gap: 16px;
        }
        .logo-area h1 {
            font-size: 1.7rem;
            font-weight: 700;
            color: #2b5e2a;
        }
        .logo-area .tagline {
            font-size: 0.85rem;
            color: #5a7156;
        }
        .hero {
            background: linear-gradient(105deg, #eef5e6 0%, #d9e6c3 100%);
            border-radius: 32px;
            margin: 32px 0 40px 0;
            padding: 48px 40px;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
        }
        .hero-title {
            font-size: 3.2rem;
            font-weight: 800;
            color: #1f4820;
        }
        .hero-title span {
            background: linear-gradient(120deg, #3c7840, #7bb359);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
        }
        .hero-sub {
            font-size: 1.25rem;
            color: #2f5a2c;
            margin-top: 16px;
        }
        .section-header {
            margin: 32px 0 24px 0;
            border-bottom: 2px solid #cbdba7;
            padding-bottom: 12px;
        }
        .section-header h2 {
            font-size: 1.8rem;
            font-weight: 600;
            color: #2b572a;
        }
        .articles-grid {
            display: flex;
            flex-direction: column;
            gap: 24px;
            margin-bottom: 56px;
        }
        .article-card {
            background: #ffffff;
            border-radius: 28px;
            box-shadow: 0 4px 14px rgba(0, 0, 0, 0.03);
            border: 1px solid #e9f0e2;
            overflow: hidden;
        }
        .article-header {
            padding: 20px 28px 12px 28px;
            border-bottom: 1px dashed #e2ecd4;
            display: flex;
            flex-wrap: wrap;
            align-items: baseline;
            gap: 12px;
        }
        .article-category {
            background: #ebf5e3;
            color: #3f6b39;
            font-weight: 600;
            font-size: 0.75rem;
            padding: 4px 12px;
            border-radius: 40px;
            display: inline-flex;
            align-items: center;
            gap: 6px;
        }
        .article-title {
            font-size: 1.55rem;
            font-weight: 700;
            color: #1a3a1a;
        }
        .article-content {
            padding: 20px 28px 28px 28px;
            color: #2f3e2c;
            font-size: 1rem;
            line-height: 1.6;
        }
        .article-content p {
            margin-bottom: 12px;
        }
        .admin-guide {
            background: #fefef7;
            border-radius: 32px;
            border: 1px solid #dee9d2;
            padding: 28px;
            margin: 24px 0 48px;
        }
        .admin-guide h3 {
            font-size: 1.3rem;
            color: #2f632c;
            margin-bottom: 18px;
        }
        .guide-steps {
            display: flex;
            flex-wrap: wrap;
            gap: 24px;
            margin-top: 20px;
        }
        .step {
            flex: 1;
            background: #f5f9f0;
            padding: 20px;
            border-radius: 20px;
        }
        .step i {
            font-size: 2rem;
            color: #527a44;
            margin-bottom: 12px;
        }
        .step code {
            background: #e2e8d5;
            padding: 2px 8px;
            border-radius: 6px;
            font-size: 0.8rem;
        }
        .btn {
            background: #527a44;
            color: white;
            padding: 10px 24px;
            border-radius: 40px;
            text-decoration: none;
            display: inline-block;
            margin-top: 12px;
            font-size: 0.9rem;
        }
        footer {
            background: #eef3e8;
            border-radius: 40px 40px 0 0;
            padding: 32px 24px;
            text-align: center;
            color: #476642;
        }
        @media (max-width: 760px) {
            .hero-title { font-size: 2rem; }
            .article-title { font-size: 1.2rem; }
            .guide-steps { flex-direction: column; }
        }
        .loading {
            text-align: center;
            padding: 60px;
            color: #7c8e72;
        }
    </style>
</head>
<body>

<div class="top-bar">
    <div class="container nav-wrapper">
        <div class="logo-area">
            <h1>牧知汇</h1>
            <div class="tagline">猪群健康管理 · 精准繁育智库</div>
        </div>
        <div class="nav-links">
            <a href="#">首页</a>
            <a href="#">健康方案</a>
            <a href="#">繁殖效率</a>
            <a href="#">行业洞察</a>
        </div>
    </div>
</div>

<main class="container">
    <div class="hero">
        <div class="hero-content">
            <div class="hero-title">
                牧知汇 · <span>智领未来</span>
            </div>
            <div class="hero-sub">
                猪群健康管理 · 提高繁殖效率 · 成为国内顶尖的5%猪场
            </div>
        </div>
        <div class="hero-icon">
            <i class="fas fa-piggy-bank" style="font-size: 4rem; color: #548b3c;"></i>
        </div>
    </div>

    <div class="section-header">
        <h2><i class="fas fa-newspaper"></i> 知识库</h2>
    </div>

    <div id="articlesContainer" class="articles-grid">
        <div class="loading"><i class="fas fa-spinner fa-pulse"></i> 加载文章中...</div>
    </div>

    <!-- 内容管理指南 -->
    <div class="admin-guide">
        <h3><i class="fas fa-edit"></i> 如何管理内容？（无需后台）</h3>
        <div class="guide-steps">
            <div class="step">
                <i class="fab fa-github"></i>
                <h4>方式一：Github Issues</h4>
                <p>1. 创建Github仓库</p>
                <p>2. 在Issues中发布文章，标题格式：<code>[分类] 文章标题</code></p>
                <p>3. 正文写详细内容</p>
                <p>4. 添加Label标签作为分类</p>
                <a href="#" class="btn" id="githubGuideBtn">查看详细教程 <i class="fas fa-arrow-right"></i></a>
            </div>
            <div class="step">
                <i class="fas fa-database"></i>
                <h4>方式二：JSON文件托管</h4>
                <p>在Github/Gitee仓库中维护一个 <code>articles.json</code> 文件：</p>
                <code style="display: block; background: #e2e8d5; padding: 12px; border-radius: 12px; font-size: 11px; margin-top: 10px;">
[<br>
  {<br>
    "type": "繁殖效率",<br>
    "title": "文章标题",<br>
    "content": "正文内容"<br>
  }<br>
]
                </code>
                <a href="#" class="btn" id="jsonGuideBtn">配置教程</a>
            </div>
            <div class="step">
                <i class="fas fa-cloud-upload-alt"></i>
                <h4>当前配置状态</h4>
                <p id="configStatus">⚙️ 正在检测配置...</p>
                <button class="btn" id="reloadBtn" style="background: #8fbc6e;">🔄 刷新文章</button>
            </div>
        </div>
    </div>
</main>

<footer>
    <p>© 2025 牧知汇 | 猪群生产管理知识共享 · 提高繁殖效率 · 成为国内顶尖5%猪场</p>
</footer>

<script>
    // ==================== 配置区域 ====================
    // 【请修改这里】配置您的数据源
    
    // 方案一：使用 Github Issues (推荐)
    // 设置您的 Github 仓库信息
    const GITHUB_CONFIG = {
        enabled: false,  // 改为 true 启用
        owner: "asnails",  // 您的 Github 用户名
        repo: "haidswine",          // 仓库名称
        labels: ["article", "牧知汇"]     // 筛选标签
    };
    
    // 方案二：使用 JSON 文件 (更简单)
    // 将 articles.json 上传到您的网站同目录，或使用 Github raw 链接
    const JSON_CONFIG = {
        enabled: true,   // 启用 JSON 模式
        url: "articles.json"  // JSON 文件路径（可以是相对路径或完整URL）
        // 示例： "https://raw.githubusercontent.com/用户名/仓库名/main/articles.json"
    };
    
    // 示例默认数据（当无网络数据时展示）
    const DEFAULT_ARTICLES = [
        {
            type: "繁殖效率",
            title: "批次化生产提高母猪年产断奶仔数",
            content: "通过优化批次间隔与同步发情技术，结合智能化饲喂站，PSY从24.5提升至28.2。"
        },
        {
            type: "健康管理",
            title: "蓝耳病净化与群体免疫力提升方案",
            content: "基于封闭式管理及疫苗免疫评估，母猪流产率下降62%，仔猪存活率提升至95%以上。"
        },
        {
            type: "生产技术",
            title: "智能化环控与猪群舒适度指数",
            content: "环境监测技术联动风机，减少呼吸道疾病风险，每头母猪年治疗成本降低40元。"
        }
    ];
    
    // ==================== 核心逻辑 ====================
    
    async function loadArticles() {
        const container = document.getElementById('articlesContainer');
        container.innerHTML = '<div class="loading"><i class="fas fa-spinner fa-pulse"></i> 加载文章中...</div>';
        
        let articles = [];
        
        // 尝试从配置的数据源加载
        try {
            if (JSON_CONFIG.enabled && JSON_CONFIG.url) {
                articles = await loadFromJSON(JSON_CONFIG.url);
                updateConfigStatus("✅ 当前使用 JSON 文件管理内容", "#2f6b2c");
            } else if (GITHUB_CONFIG.enabled) {
                articles = await loadFromGithubIssues();
                updateConfigStatus("✅ 当前使用 Github Issues 管理内容", "#2f6b2c");
            } else {
                // 使用默认数据，并提示配置
                articles = DEFAULT_ARTICLES;
                updateConfigStatus("⚠️ 使用示例数据，请在上方配置您的数据源", "#c97e00");
            }
        } catch (error) {
            console.error("加载文章失败:", error);
            articles = DEFAULT_ARTICLES;
            updateConfigStatus("⚠️ 数据加载失败，显示示例数据。请检查配置", "#c97e00");
        }
        
        renderArticles(articles);
    }
    
    // 从 JSON 文件加载
    async function loadFromJSON(url) {
        const response = await fetch(url, {
            cache: 'no-cache',
            headers: { 'Cache-Control': 'no-cache' }
        });
        if (!response.ok) {
            throw new Error(`HTTP ${response.status}`);
        }
        const data = await response.json();
        if (Array.isArray(data)) {
            return data;
        } else if (data.articles && Array.isArray(data.articles)) {
            return data.articles;
        }
        return [];
    }
    
    // 从 Github Issues 加载
    async function loadFromGithubIssues() {
        const { owner, repo, labels } = GITHUB_CONFIG;
        const labelParam = labels.map(l => `labels=${encodeURIComponent(l)}`).join('&');
        const url = `https://api.github.com/repos/${owner}/${repo}/issues?state=open&${labelParam}&per_page=50`;
        
        const response = await fetch(url);
        if (!response.ok) {
            throw new Error(`Github API 错误: ${response.status}`);
        }
        
        const issues = await response.json();
        const articles = issues.map(issue => {
            // 解析标题格式：[分类] 文章标题
            let type = "行业资讯";
            let title = issue.title;
            const match = title.match(/^\[(.+?)\]\s*(.+)$/);
            if (match) {
                type = match[1];
                title = match[2];
            }
            
            return {
                type: type,
                title: title,
                content: issue.body || "暂无详细内容",
                issueUrl: issue.html_url
            };
        });
        
        return articles;
    }
    
    // 渲染文章（不显示发布时间和分类标签，但卡片头部保留【类型】样式）
    function renderArticles(articles) {
        const container = document.getElementById('articlesContainer');
        
        if (!articles || articles.length === 0) {
            container.innerHTML = `<div style="background:#f8faf2; border-radius:32px; padding:48px; text-align:center;">
                <i class="fas fa-feather-alt"></i> 暂无文章，请在配置的数据源中添加内容
            </div>`;
            return;
        }
        
        let html = '';
        articles.forEach(article => {
            // 处理正文段落
            let contentHtml = '';
            if (article.content) {
                const paragraphs = article.content.split(/\n/);
                paragraphs.forEach(para => {
                    if (para.trim()) {
                        contentHtml += `<p>${escapeHtml(para.trim())}</p>`;
                    }
                });
                if (!contentHtml) contentHtml = `<p>${escapeHtml(article.content)}</p>`;
            } else {
                contentHtml = `<p>暂无内容</p>`;
            }
            
            html += `
                <div class="article-card">
                    <div class="article-header">
                        <span class="article-category"><i class="fas fa-folder-open"></i> ${escapeHtml(article.type)}</span>
                        <div class="article-title">${escapeHtml(article.title)}</div>
                    </div>
                    <div class="article-content">
                        ${contentHtml}
                    </div>
                </div>
            `;
        });
        
        container.innerHTML = html;
    }
    
    function updateConfigStatus(message, color) {
        const statusEl = document.getElementById('configStatus');
        if (statusEl) {
            statusEl.innerHTML = message;
            statusEl.style.color = color;
        }
    }
    
    function escapeHtml(str) {
        if (!str) return '';
        return str.replace(/[&<>]/g, function(m) {
            if (m === '&') return '&amp;';
            if (m === '<') return '&lt;';
            if (m === '>') return '&gt;';
            return m;
        }).replace(/[\uD800-\uDBFF][\uDC00-\uDFFF]/g, function(c) {
            return c;
        });
    }
    
    // 教程提示
    function showTutorial(type) {
        if (type === 'github') {
            alert("📖 Github Issues 配置教程：\n\n1. 创建Github仓库\n2. Settings -> Issues 开启\n3. 创建Issue，标题格式：[分类] 文章标题\n4. 正文写文章内容\n5. 添加 label 为 'article'\n6. 修改上方代码中的 GITHUB_CONFIG 配置");
        } else {
            alert("📖 JSON 文件配置教程：\n\n1. 创建 articles.json 文件\n2. 格式参考示例代码\n3. 上传到网站同目录\n4. 或使用 Github Raw 链接\n5. 修改 JSON_CONFIG.url 指向你的文件");
        }
    }
    
    // 页面初始化
    document.addEventListener('DOMContentLoaded', () => {
        loadArticles();
        
        const reloadBtn = document.getElementById('reloadBtn');
        if (reloadBtn) {
            reloadBtn.addEventListener('click', () => loadArticles());
        }
        
        const githubBtn = document.getElementById('githubGuideBtn');
        const jsonBtn = document.getElementById('jsonGuideBtn');
        if (githubBtn) githubBtn.addEventListener('click', (e) => { e.preventDefault(); showTutorial('github'); });
        if (jsonBtn) jsonBtn.addEventListener('click', (e) => { e.preventDefault(); showTutorial('json'); });
    });
</script>
</body>
</html>
