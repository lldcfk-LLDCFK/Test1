<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>支持UP主</title>
    <style>
        body {
            background: #f0f0f0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            margin: 0;
            font-family: 'Microsoft YaHei', sans-serif;
        }

        /* 爱心动画 */
        .heart {
            position: relative;
            width: 100px;
            height: 90px;
            animation: heartbeat 1.2s infinite;
            margin-bottom: 40px;
        }
        .heart::before,
        .heart::after {
            content: '';
            position: absolute;
            width: 50px;
            height: 80px;
            background: linear-gradient(45deg, #ff3f3f, #ff1493);
            border-radius: 50px 50px 0 0;
        }
        .heart::before {
            left: 50px;
            transform: rotate(-45deg);
            transform-origin: 0 100%;
        }
        .heart::after {
            left: 0;
            transform: rotate(45deg);
            transform-origin: 100% 100%;
        }

        /* 按钮样式 */
        .support-btn {
            padding: 15px 30px;
            font-size: 1.2rem;
            background: linear-gradient(135deg, #00a1d6, #0092ff);
            color: white;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 146, 255, 0.3);
            text-decoration: none;
        }
        .support-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 20px rgba(0, 146, 255, 0.5);
        }

        /* 心跳动画 */
        @keyframes heartbeat {
            0% { transform: scale(1); }
            15% { transform: scale(1.3); }
            30% { transform: scale(1); }
            45% { transform: scale(1.15); }
            60% { transform: scale(1); }
        }
    </style>
</head>
<body>
    <div class="heart"></div>
    <a href="https://space.bilibili.com/3546596132259892?spm_id_from=333.1007.0.0" target="_blank" class="support-btn">
        支持支持UP吧 ❤
    </a>
</body>
</html>
