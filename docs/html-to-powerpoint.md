<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CBT Across the Life Span</title>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://unpkg.com/pptxgenjs@3.12.0/dist/pptxgen.bundle.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Tajawal', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            overflow: hidden;
            direction: ltr;
        }

        .presentation-container {
            width: 100vw;
            height: 100vh;
            display: flex;
            flex-direction: column;
            position: relative;
        }

        .slide {
            display: none;
            width: 100%;
            height: calc(100vh - 80px);
            background: white;
            padding: 50px;
            overflow-y: auto;
            position: relative;
        }

        .slide.active {
            display: block;
            animation: slideIn 0.5s ease-in-out;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        h1 {
            color: #667eea;
            font-size: 2.5em;
            margin-bottom: 20px;
            text-align: center;
            border-bottom: 3px solid #764ba2;
            padding-bottom: 15px;
            font-weight: 700;
        }

        h2 {
            color: #764ba2;
            font-size: 2em;
            margin-top: 30px;
            margin-bottom: 15px;
            font-weight: 600;
        }

        h3 {
            color: #667eea;
            font-size: 1.5em;
            margin-top: 20px;
            margin-bottom: 10px;
            font-weight: 500;
        }

        h4 {
            color: #764ba2;
            font-size: 1.2em;
            margin-top: 15px;
            margin-bottom: 8px;
            font-weight: 500;
        }

        p, li {
            font-size: 1.1em;
            line-height: 1.6;
            margin-bottom: 10px;
            color: #333;
        }

        ul, ol {
            margin-left: 30px;
            margin-bottom: 15px;
        }

        .controls {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            height: 80px;
            background: rgba(102, 126, 234, 0.95);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 40px;
            box-shadow: 0 -4px 20px rgba(0,0,0,0.2);
            z-index: 1000;
        }

        button {
            background: white;
            color: #667eea;
            border: none;
            padding: 15px 30px;
            font-size: 1.1em;
            border-radius: 25px;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: bold;
            font-family: 'Tajawal', sans-serif;
        }

        button:hover {
            background: #764ba2;
            color: white;
            transform: scale(1.05);
        }

        button:disabled {
            opacity: 0.5;
            cursor: not-allowed;
        }

        .slide-counter {
            color: white;
            font-size: 1.2em;
            font-weight: bold;
        }

        .highlight {
            background: #fff3cd;
            padding: 3px 8px;
            border-radius: 4px;
            border-left: 3px solid #ffc107;
        }

        .box {
            background: #f8f9fa;
            border-left: 4px solid #667eea;
            padding: 15px;
            margin: 15px 0;
            border-radius: 5px;
        }

        .example {
            background: #e7f3ff;
            border-left: 4px solid #2196F3;
            padding
