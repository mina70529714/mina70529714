<!DOCTYPE html>
<html lang="ar">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>فريق إيڤما - شروط</title>
    <style>
        body {
            font-family: 'Cairo', sans-serif;
            background-color: #f0f4f8;
            direction: rtl;
            text-align: right;
            margin: 0;
            padding: 0;
            min-width: 320px;
            min-height: 100vh;
        }

        .container {
            width: 70vw;
            margin: 20px auto;
            padding: 20px;
            background-color: #ffffff;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.2);
            border-radius: 10px;
            max-width: 100%;
            box-sizing: border-box;
        }

        .header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 20px;
        }

        .header img {
            width: 200px;
         
            height: auto;
        
            max-width: 100%;
            object-fit: contain;
        }
        .header .logo-left {
            margin-right: auto;
        }

        .header .logo-right {
            margin-left: auto;
        }

        .header h1 {
            font-family: 'Cairo', sans-serif;
            font-size: 2.5vw;
            color: #333;
            text-align: center;
            flex-grow: 1;
            margin: 0;
        }

        fieldset {
            border: 2px solid #28a745;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 20px;
        }

        legend {
            font-size: 1.8vw;
            padding: 0 10px;
            font-weight: bold;
            color: #28a745;
        }

        label {
            font-size: 1.2vw;
            color: #333;
            margin-bottom: 10px;
            display: block;
        }

        input[type="checkbox"] {
            margin-left: 0;
            margin-right: 10px;
        }

        button {
            padding: 12px 25px;
            font-size: 1.5vw;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            display: block;
            margin: 0 auto;
            opacity: 0.5;
        }

        button.enabled {
            opacity: 1;
        }

        button:hover {
            background-color: #45a049;
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="header">
            <img src="دون عنوان (21 x 21 سم).png" alt="Logo 1" class="logo-left"> 
            <h1>فريق إيڤما</h1> 
            <img src="2.jpg" alt="Logo 2" class="logo-right">
        </div>
        <fieldset>
            <legend>الشروط</legend>
            <ol>
                <li>- السن من ١٨ ( اولى جامعه ) الى ٤٠ سنة.</li>
                <li> ملزم بحضور اى كورس تنظمه اللجنه ( روحى او اكاديمى اعاقة )</li>
                <li>- عندك استعداد للتعامل المباشر مع الاولاد المعاقين</li>
                <li>ملتزم بحضور اجتماع شهرى للجنه او قداس</li>
                <li>موافقة اب الاعتراف على دخولك الفريق</li>
                <li>ملتزم بقوانين الفريق وطريقة المشاركه فى اى انشطه او مؤتمرات على حسب توزيعه قائد الفريق</li>

            </ol>
            <label>
                <input type="checkbox" id="accept_conditions" required> أوافق على الشروط
            </label>
            <button id="submit_button" onclick="window.location.href='pag 2 .html'" disabled>انتقل إلى التسجيل</button>
        </fieldset>
    </div>
    <script>
        document.getElementById('accept_conditions').addEventListener('change', function () {
            const button = document.getElementById('submit_button');
            button.disabled = !this.checked;
            button.classList.toggle('enabled', this.checked);
        });
    </script>
</body>

</html>
