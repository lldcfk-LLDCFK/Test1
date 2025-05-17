<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <!-- 字符集声明应置于head最前面 -->
    <meta charset="UTF-8">
    <!-- 双重声明确保兼容性 -->
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <title>支持UP主</title>
    <style>
        /* 新增字体回退方案 */
        @font-face {
            font-family: 'HarmonyOS_Sans_SC';
            src: local('HarmonyOS Sans SC'), local('PingFang SC'), local('Microsoft YaHei');
        }

        body {
            background: #f0f0f0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            margin: 0;
            /* 增强字体兼容性 */
            font-family: 'HarmonyOS_Sans_SC', 'Microsoft YaHei', 'PingFang SC', 'Hiragino Sans GB', 'Noto Sans CJK SC', sans-serif;
        }

        /* 优化渐变兼容性 */
        .heart::before,
        .heart::after {
            background: linear-gradient(45deg, #ff3f3f, #ff1493);
            background: -webkit-linear-gradient(45deg, #ff3f3f, #ff1493); /* 兼容旧版浏览器 */
        }

        /* 新增文字阴影增强可读性 */
        .support-btn {
            text-shadow: 0 2px 2px rgba(0, 0, 0, 0.1);
            /* 新增禁止文字选择 */
            user-select: none;
            -webkit-user-select: none;
        }

        /* 新增移动端点击效果 */
        @media (hover: none) {
            .support-btn:active {
                transform: scale(0.95);
            }
        }
    </style>
</head>
<body>
    <!-- 添加aria标签增强可访问性 -->
    <div class="heart" aria-hidden="true"></div>
    <a href="https://space.bilibili.com/3546596132259892?spm_id_from=333.1007.0.0" 
       target="_blank" 
       class="support-btn"
       role="button"
       aria-label="前往B站支持UP主">
        <!-- 使用全角空格替代普通空格 -->
        支持支持UP吧　❤
    </a>
</body>
</html>
