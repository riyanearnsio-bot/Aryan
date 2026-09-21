<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Premium Redeem Access</title>

<style>
*{
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    margin:0;
    font-family:Arial,Helvetica,sans-serif;
    background:#080d18;
    color:#fff;
}

body::before{
    content:"";
    position:fixed;
    inset:0;
    background:
        radial-gradient(circle at 20% 10%,#16498b55,transparent 35%),
        radial-gradient(circle at 90% 80%,#8b2bb955,transparent 35%);
    pointer-events:none;
}

.container{
    width:min(100% - 28px,460px);
    margin:auto;
    position:relative;
}

header{
    padding:22px 0 10px;
    text-align:center;
}

.logo{
    display:inline-flex;
    align-items:center;
    gap:8px;
    color:#ffe08a;
    font-weight:800;
    letter-spacing:1.5px;
    font-size:13px;
}

.hero{
    text-align:center;
    padding:18px 4px 22px;
}

.hero h1{
    font-size:34px;
    line-height:1.08;
    margin:12px 0 10px;
}

.hero h1 span{
    color:#ffd75c;
}

.hero p{
    margin:0;
    color:#b8c1d0;
    line-height:1.55;
}

.card{
    background:linear-gradient(
        150deg,
        #151d2bfa,
        #121620f5
    );

    border:1px solid #ffffff1c;
    border-radius:24px;
    padding:20px;

    box-shadow:0 20px 70px #0008;
}

.price{
    font-size:36px;
    font-weight:900;
    text-align:center;
    margin:4px 0 16px;
    color:#ffe27a;
}

.qr{
    display:block;
    width:100%;
    max-width:350px;
    margin:0 auto;
    border-radius:15px;
    background:#fff;
}

.steps{
    display:grid;
    gap:10px;
    margin:18px 0;
}

.step{
    display:flex;
    gap:12px;
    align-items:flex-start;

    padding:12px;

    border-radius:14px;
    background:#ffffff08;
    border:1px solid #ffffff12;
}

.num{
    min-width:30px;
    height:30px;

    border-radius:9px;

    background:#2c77ff;

    display:grid;
    place-items:center;

    font-weight:800;
}

.step b{
    display:block;
    margin-bottom:3px;
}

.step small{
    color:#9fa8b8;
    line-height:1.35;
}

.btn{
    width:100%;

    border:0;
    border-radius:14px;

    padding:16px;

    font-size:17px;
    font-weight:800;

    cursor:pointer;
}

.open{
    background:
        linear-gradient(
            90deg,
            #ffca28,
            #ff8f00
        );

    color:#171717;
}

.open:active{
    transform:scale(.99);
}

.note{
    margin-top:14px;

    padding:12px;

    border-radius:12px;

    background:#ffcc0010;
    border:1px solid #ffcc0030;

    color:#c9ced8;

    font-size:12px;
    line-height:1.5;
}

section{
    padding:28px 2px;
}

section h2{
    font-size:22px;
    margin:0 0 14px;
}

.faq{
    border-top:1px solid #ffffff18;
    padding:14px 0;
}

.faq b{
    display:block;
    margin-bottom:6px;
}

.faq p{
    margin:0;
    color:#aeb6c5;
    font-size:13px;
    line-height:1.5;
}

footer{
    text-align:center;
    color:#7f8795;
    font-size:11px;
    padding:8px 0 30px;
}
</style>
</head>


<body>

<div class="container">

    <!-- HEADER -->
    <header>
        <div class="logo">
            ✦ PREMIUM DIGITAL ACCESS
        </div>
    </header>


    <!-- HERO -->
    <div class="hero">

        <h1>
            Redeem Code
            <span>Access</span>
        </h1>

        <p>
            Payment instructions और access link
            एक ही जगह पर।
        </p>

    </div>


    <!-- PAYMENT CARD -->
    <main class="card">

        <div class="price">
            ₹99
        </div>


        <!--
        अपनी QR image का नाम payment-qr.jpg रखें
        और इसी HTML के साथ same folder में रखें।
        -->

        <img
            class="qr"
            src="payment-qr.jpg"
            alt="UPI Payment QR"
        >


        <!-- STEPS -->
        <div class="steps">

            <div class="step">

                <div class="num">
                    1
                </div>

                <div>

                    <b>
                        QR Scan करें
                    </b>

                    <small>
                        अपने UPI app से ऊपर दिया गया
                        QR scan करें और ₹99 payment करें।
                    </small>

                </div>

            </div>


            <div class="step">

                <div class="num">
                    2
                </div>

                <div>

                    <b>
                        Payment पूरा करें
                    </b>

                    <small>
                        Payment करने से पहले अपने UPI
                        app में recipient और amount
                        जरूर check करें।
                    </small>

                </div>

            </div>


            <div class="step">

                <div class="num">
                    3
                </div>

                <div>

                    <b>
                        Redeem Page खोलें
                    </b>

                    <small>
                        नीचे दिए button से redeem-code
                        page पर जाएँ।
                    </small>

                </div>

            </div>

        </div>


        <!-- OPEN BUTTON -->

        <button
            class="btn open"
            onclick="openRedeem()"
        >
            OPEN REDEEM CODE
        </button>


        <!-- NOTICE -->

        <div class="note">

            <b>ध्यान दें:</b>

            यह static landing page payment को
            automatically verify नहीं करता।

            वास्तविक payment verification के लिए
            payment gateway और server-side
            verification लगाना जरूरी है।

            इसे किसी official Garena या Free Fire
            website के रूप में प्रस्तुत न करें।

        </div>

    </main>


    <!-- FAQ -->

    <section>

        <h2>
            कैसे काम करता है?
        </h2>


        <div class="faq">

            <b>
                क्या payment automatically verify होगा?
            </b>

            <p>
                नहीं। इस static HTML page में
                automatic payment verification नहीं है।
                इसके लिए वास्तविक payment gateway
                और backend verification चाहिए।
            </p>

        </div>


        <div class="faq">

            <b>
                Redeem codes कहाँ मिलेंगे?
            </b>

            <p>
                OPEN button आपके दिए हुए external
                redeem page पर ले जाएगा।
                केवल वैध और अधिकृत codes का इस्तेमाल करें।
            </p>

        </div>


        <div class="faq">

            <b>
                क्या यह Garena की official website है?
            </b>

            <p>
                नहीं। यह independent landing page है।
            </p>

        </div>

    </section>


    <!-- FOOTER -->

    <footer>

        © 2026 Premium Access
        • Independent Website

    </footer>

</div>



<script>

/*
==================================================
        REDEEM PAGE LINK
==================================================

यहाँ अपना redeem page link डालें।
*/

const REDEEM_LINK =
"https://earnsio.cc/r/aryanbhai";



/*
==================================================
        OPEN REDEEM PAGE
==================================================
*/

function openRedeem(){

    if(
        !REDEEM_LINK ||
        REDEEM_LINK === "YOUR_REDEEM_PAGE_LINK"
    ){

        alert(
            "Redeem page link अभी add नहीं किया गया है।"
        );

        return;
    }


    window.location.href =
        REDEEM_LINK;
}

</script>

</body>
</html>
