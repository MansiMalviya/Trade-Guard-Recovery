<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TradeGuard Recovery</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }

        body {
            background-color: #f8f9fa;
            color: #212529;
            line-height: 1.6;
        }

        header {
            background-color: #1d3557;
            color: #fff;
            padding: 2rem 1rem;
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
        }

        header p {
            font-size: 1.2rem;
            margin-top: 0.5rem;
        }

        section.hero {
            background: linear-gradient(120deg, #e0f7fa, #fce4ec);
            padding: 3rem 1rem;
            text-align: center;
            animation: fadeIn 2s ease-in;
        }

        section.hero img {
            width: 80px;
            margin-bottom: 1rem;
        }

        .traffic-light {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            margin: 2rem auto;
        }

        .traffic-light div {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            position: relative;
            transition: transform 0.3s ease;
        }

        .traffic-light div:hover {
            transform: scale(1.2);
        }

        .traffic-light div::after {
            content: attr(data-text);
            position: absolute;
            left: 60px;
            top: 50%;
            transform: translateY(-50%);
            white-space: nowrap;
            font-size: 0.75rem;
            color: #333;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .traffic-light div:hover::after {
            opacity: 1;
        }

        .red { background-color: #e63946; }
        .yellow { background-color: #ffca28; }
        .green { background-color: #43a047; }

        .features, .pricing {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 2rem;
            padding: 3rem 2rem;
        }

        .feature-box {
            background-color: white;
            border-radius: 10px;
            padding: 1.5rem;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .feature-box:hover {
            transform: translateY(-5px);
        }

        .feature-box h3 {
            color: #1d3557;
            margin-bottom: 0.8rem;
        }

        .contact-form {
            padding: 3rem 2rem;
            background-color: #fff3cd;
        }

        .contact-form h2 {
            text-align: center;
            margin-bottom: 1rem;
            color: #1d3557;
        }

        .contact-form form {
            max-width: 600px;
            margin: auto;
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .contact-form input, .contact-form textarea {
            padding: 0.8rem;
            border-radius: 8px;
            border: 1px solid #ccc;
            font-size: 1rem;
        }

        .contact-form button {
            padding: 0.8rem;
            background-color: #1d3557;
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            cursor: pointer;
        }

        footer {
            text-align: center;
            padding: 1rem;
            background-color: #1d3557;
            color: white;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .pricing-header {
            text-align: center;
            margin-top: 3rem;
            font-size: 2rem;
            font-weight: 600;
            color: #1d3557;
        }
    </style>
</head>

<body>
    <header>
        <h1>TradeGuard Recovery</h1>
        <p>Helping You Understand Where to Stop, Start & Move Forward in the Stock Market</p>
    </header>

    <section class="hero">
        <img src="https://img.icons8.com/fluency/96/light-on.png" alt="AI symbol">
        <h2>Smart AI-Based Recovery Guidance</h2>
        <p>We analyze your trading loss and guide you ethically on the right path forward — no tips, no fraud, just recovery support.</p>

        <div class="traffic-light">
            <div class="red" data-text="Stop - Recognize mistakes"></div>
            <div class="yellow" data-text="Pause - Learn & reflect"></div>
            <div class="green" data-text="Go - Restart with wisdom"></div>
        </div>
    </section>

    <section class="features">
        <div class="feature-box">
            <h3>Loss Analysis Report</h3>
            <p>Detailed report on where you went wrong and how to avoid repeating the same mistakes.</p>
        </div>
        <div class="feature-box">
            <h3>Recovery Mentorship</h3>
            <p>1-on-1 calls, structured learning, and mindset resetting for safer market re-entry.</p>
        </div>
        <div class="feature-box">
            <h3>Fraud Advisory Checks</h3>
            <p>Find out whether the advisory or algo firm misled you — we analyze and explain.</p>
        </div>
        <div class="feature-box">
            <h3>AI-Powered Roadmap</h3>
            <p>Custom strategy on what to do next — stay away or come back strong.</p>
        </div>
    </section>

    <h2 class="pricing-header">Our Plans</h2>
    <section class="pricing">
        <div class="feature-box">
            <h3>Basic Plan</h3>
            <p>Loss Audit + WhatsApp Guidance</p>
            <strong>₹999</strong>
        </div>
        <div class="feature-box">
            <h3>Premium Call</h3>
            <p>30-min Zoom Call + Roadmap PDF</p>
            <strong>₹1,499</strong>
        </div>
        <div class="feature-box">
            <h3>Advisory Check</h3>
            <p>Fraud Analysis + Report</p>
            <strong>₹2,499</strong>
        </div>
        <div class="feature-box">
            <h3>Mentorship Pack</h3>
            <p>15 Days Guidance + 3 Calls + Daily Chat</p>
            <strong>₹3,499</strong>
        </div>
        <div class="feature-box">
            <h3>30-Day Handholding</h3>
            <p>All-in-One Personalized Service</p>
            <strong>₹5,999</strong>
        </div>
        <div class="feature-box">
            <h3>All-in-One Monthly Plan</h3>
            <p>Complete Recovery Support + Monitoring + Advisory Checks</p>
            <strong>₹14,999</strong>
        </div>
    </section>

    <section class="contact-form">
        <h2>Contact Us</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <input type="tel" placeholder="Mobile Number" required>
            <textarea rows="4" placeholder="Your Query..." required></textarea>
            <button type="submit">Submit</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 TradeGuard Recovery. All rights reserved.</p>
    </footer>
</body>

</html>
