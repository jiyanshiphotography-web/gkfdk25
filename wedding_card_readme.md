# 💌 विवाह आमंत्रण पत्र (Indian Wedding Card HTML Template)

यह एक पारंपरिक भारतीय शादी के कार्ड (Wedding Invitation Card) का पूरा **HTML और CSS** कोड है। इसमें कार्ड के बिल्कुल वैसे ही डिज़ाइन (बॉर्डर, दो-भाग लेआउट, श्लोक, और वर-वधू विवरण) को शामिल किया गया है।

---

## 💻 पूरा HTML और CSS कोड (Complete Code)

नीचे दिए गए कोड को कॉपी करके `index.html` या `wedding_card.html` नाम से सेव करें और ब्राउज़र में खोलें:

```html
<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>विवाह आमंत्रण पत्र</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #e6e6e6;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            padding: 20px;
        }
        .main-card {
            width: 750px;
            background: #ffffff;
            border: 5px solid #000;
            padding: 12px;
            box-shadow: 0 0 15px rgba(0,0,0,0.3);
        }
        .box {
            border: 2px solid #000;
            padding: 15px;
            margin-bottom: 12px;
            position: relative;
            text-align: center;
        }
        .box:last-child {
            margin-bottom: 0;
        }
        /* कोने के डिज़ाइन के लिए */
        .corner-tl, .corner-tr, .corner-bl, .corner-br {
            position: absolute;
            width: 25px;
            height: 25px;
            border: 3px solid #000;
        }
        .corner-tl { top: 4px; left: 4px; border-right: none; border-bottom: none; }
        .corner-tr { top: 4px; right: 4px; border-left: none; border-bottom: none; }
        .corner-bl { bottom: 4px; left: 4px; border-right: none; border-top: none; }
        .corner-br { bottom: 4px; right: 4px; border-left: none; border-top: none; }

        .shlok {
            font-size: 14px;
            font-weight: bold;
            line-height: 1.5;
        }
        .sub-heading {
            font-size: 13px;
            margin: 10px 0;
        }
        .title-banner {
            border: 2px solid #000;
            display: inline-block;
            padding: 4px 20px;
            font-weight: bold;
            font-size: 16px;
            border-radius: 25px;
            margin: 10px 0;
            background: #fff;
        }
        .events-table {
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin-top: 12px;
        }
        .event-box {
            width: 42%;
        }
        .event-title {
            font-weight: bold;
            font-size: 16px;
            border-bottom: 1px dashed #000;
            display: inline-block;
            padding-bottom: 3px;
            margin-bottom: 6px;
        }
        .event-date {
            font-size: 13px;
            line-height: 1.4;
        }
        .center-icon {
            font-size: 28px;
        }
        .note {
            margin-top: 15px;
            font-size: 13px;
            font-weight: bold;
            border: 1px solid #000;
            border-radius: 15px;
            padding: 4px 12px;
            display: inline-block;
        }
        /* नीचे वाले बॉक्स का लेआउट */
        .details-container {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-top: 10px;
            text-align: left;
            font-size: 13px;
            line-height: 1.6;
        }
        .left-column {
            width: 42%;
        }
        .center-column {
            width: 16%;
            text-align: center;
            align-self: center;
        }
        .center-column h2 {
            margin: 0;
            font-size: 20px;
            border: 1px solid #000;
            border-radius: 50%;
            padding: 8px;
            display: inline-block;
        }
        .right-column {
            width: 42%;
            text-align: right;
        }
        .groom-details {
            text-align: right;
        }
        .address-box {
            text-align: left;
            margin-top: 20px;
            padding-left: 20px;
        }
        .name-highlight {
            font-size: 17px;
            font-weight: bold;
            display: block;
            margin: 3px 0;
        }
        .blessing-text {
            text-align: center;
            font-size: 13px;
            font-weight: bold;
            margin-top: 15px;
            border-top: 1px dotted #000;
            padding-top: 8px;
        }
    </style>
</head>
<body>

<div class="main-card">

    <!-- ऊपर वाला बॉक्स (कार्यक्रम विवरण) -->
    <div class="box">
        <div class="corner-tl"></div>
        <div class="corner-tr"></div>
        <div class="corner-bl"></div>
        <div class="corner-br"></div>

        <div class="shlok">!! श्री गणेशाय नमः !!</div>
        <div class="shlok">|| मंगलम् भगवान विष्णुः मंगलम् गरुड़ध्वजः</div>
        <div class="shlok">मंगलम् पुण्डरीकाक्षः मंगलाय तनोऽहरिः ||</div>
        <div class="sub-heading">सौभाग्य हमारा तब होगा, जब दर्शन आपका पायेंगे। हृदय कमल खिल जाएगा, जब आप हमारे द्वार आयेंगे।।</div>
        
        <div><span class="title-banner">卐 वैवाहिक कार्यक्रम 卐</span></div>
        
        <div class="events-table">
            <div class="event-box">
                <div class="event-title">!! पूजा एवं मटकोर !!</div>
                <div class="event-date">दिनांक 27.06.2023, मंगलवार<br>(आषाढ़ शुक्ल नवमी)</div>
            </div>
            <div class="center-icon">🕉️</div>
            <div class="event-box">
                <div class="event-title">!! शुभ विवाह !!</div>
                <div class="event-date">दिनांक 28.06.2023, बुधवार<br>(आषाढ़ शुक्ल दशमी)</div>
            </div>
        </div>

        <div>
            <span class="note">नोट: समस्त वैवाहिक कार्यक्रम मेरे निवास स्थान पतौरा प्राण टोला से सम्पन्न होगी।</span>
        </div>
    </div>

    <!-- नीचे वाला बॉक्स (वर-वधू एवं परिवार विवरण) -->
    <div class="box">
        <div class="corner-tl"></div>
        <div class="corner-tr"></div>
        <div class="corner-bl"></div>
        <div class="corner-br"></div>

        <div class="shlok">!! श्री गणेशाय नमः !!</div>
        
        <div class="details-container">
            <!-- बाएं तरफ: कन्या पक्ष -->
            <div class="left-column">
                स्नेही स्वजन,<br>
                &nbsp;&nbsp;&nbsp;&nbsp;परमपिता परमेश्वर की असीम अनुकम्पा सें मेरी सुपुत्री,<br>
                <span class="name-highlight">आयुष्मति कुमारी रजनी</span>
                सुपुत्री - श्रीमती प्रभा देवी एवं<br>
                &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;श्री लक्ष्मण राम<br><br>
                <strong>दर्शनाभिलाषी:-</strong><br>
                महेन्द्र राम, हीरालाल राम<br>
                लालबाबू राम, अजय राम<br>
                विरेन्द्र राम, उपेन्द्र राम<br>
                शैलेन्द्र राम, सुभाष राम<br>
                आलोक कुमार एवं समस्त राम परिवार।
            </div>

            <!-- बीच में: संग / परिणयोत्सव -->
            <div class="center-column">
                <h2>संग</h2>
                <div style="font-size: 12px; font-weight: bold; margin-top: 5px;">के<br>परिणयोत्सव</div>
            </div>

            <!-- दाएं तरफ: वर पक्ष -->
            <div class="right-column">
                <div class="groom-details">
                    <br><br>
                    <span class="name-highlight">आयुष्मान् संदीप कुमार</span>
                    सुपुत्र- श्रीमती मीरा देवी एवं<br>
                    श्री सतदेव राम<br>
                    पता- शांतिपुरी, वार्ड नं0- 3
                </div>
                <div class="address-box">
                    <strong>आकांक्षी:-</strong><br>
                    <strong style="font-size: 15px;">श्री लक्ष्मण राम</strong><br>
                    पता- पतौरा प्राण टोला<br>
                    पो0- पतौरा, थाना- मु0 मोतिहारी<br>
                    जिला- पूर्वी चंपारण<br>
                    मो0- 89999999999
                </div>
            </div>
        </div>

        <div class="blessing-text">
            पर आपकी स्नेहिल उपस्थिति एवं आर्शीवचनों से वर-वधू को अभिसिंचित कर हमें अनुगृहित करें।
        </div>
    </div>

</div>

</body>
</html>
```

---

## 🚀 उपयोग कैसे करें (How to Use)
1. ऊपर दिए गए कोड को कॉपी करें।
2. अपने कंप्यूटर में एक नई फाइल `wedding.html` बनाएं और कोड पेस्ट करके सेव करें।
3. फाइल को किसी भी ब्राउज़र (Chrome, Edge आदि) में खोलें।
4. प्रिंट करने के लिए ब्राउज़र में `Ctrl + P` दबाएं।