# Riley-Landing-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>From Zero to $10K Months in 30 Days | PSD Framework</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html, body {
            overflow-x: hidden;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background: #fff;
        }
        
        .container {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 0;
            text-align: center;
        }
        
        .preheader {
            font-size: 14px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 20px;
            opacity: 0.9;
        }
        
        .hero h1 {
            font-size: 3.5em;
            font-weight: bold;
            margin-bottom: 20px;
            line-height: 1.2;
        }
        
        .hero .subheader {
            font-size: 1.4em;
            margin-bottom: 40px;
            opacity: 0.95;
            line-height: 1.4;
        }
        
        .vsl-container {
            margin: 40px 0;
            position: relative;
            display: inline-block;
        }
        
        .vsl-placeholder {
            width: 400px;
            height: 225px;
            background: #000;
            border-radius: 10px;
            position: relative;
            cursor: pointer;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }
        
        .play-button {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 80px;
            height: 80px;
            background: rgba(255,255,255,0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        
        .play-button:hover {
            background: rgba(255,255,255,1);
            transform: translate(-50%, -50%) scale(1.1);
        }
        
        .play-button::after {
            content: '';
            width: 0;
            height: 0;
            border-left: 25px solid #667eea;
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
            margin-left: 5px;
        }
        
        .cta-button {
            display: inline-block;
            background: #ff6b6b;
            color: white;
            padding: 20px 40px;
            font-size: 1.3em;
            font-weight: bold;
            text-decoration: none;
            border-radius: 50px;
            transition: all 0.3s ease;
            box-shadow: 0 5px 20px rgba(255,107,107,0.3);
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .cta-button:hover {
            background: #ff5252;
            transform: translateY(-2px);
            box-shadow: 0 7px 25px rgba(255,107,107,0.4);
        }
        
        /* Section Styling */
        .section {
            padding: 80px 0;
        }
        
        .section h2 {
            font-size: 2.5em;
            margin-bottom: 30px;
            text-align: center;
            color: #2c3e50;
            line-height: 1.2;
        }
        
        .section p {
            font-size: 1.2em;
            margin-bottom: 20px;
            line-height: 1.8;
        }
        
        .highlight {
            background: linear-gradient(120deg, #a8edea 0%, #fed6e3 100%);
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            border-left: 5px solid #667eea;
        }
        
        .testimonial {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 10px;
            margin: 30px 0;
            border-left: 5px solid #28a745;
            font-style: italic;
        }
        
        .testimonial strong {
            font-style: normal;
            color: #28a745;
        }
        
        /* Problem Section */
        .problem {
            background: #f8f9fa;
        }
        
        /* Origin Story */
        .origin {
            background: white;
        }
        
        /* Solution */
        .solution {
            background: #f8f9fa;
        }
        
        .framework-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }
        
        .step {
            background: white;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border-top: 5px solid #667eea;
        }
        
        .step h3 {
            color: #667eea;
            font-size: 1.5em;
            margin-bottom: 15px;
        }
        
        /* Product Section */
        .product {
            background: white;
        }
        
        .bullets {
            list-style: none;
            margin: 30px 0;
        }
        
        .bullets li {
            padding: 15px 0;
            padding-left: 30px;
            position: relative;
            font-size: 1.1em;
            line-height: 1.6;
        }
        
        .bullets li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #28a745;
            font-weight: bold;
            font-size: 1.2em;
        }
        
        /* Offer Section */
        .offer {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            text-align: center;
        }
        
        .offer h2 {
            color: white;
        }
        
        .guarantee {
            background: rgba(255,255,255,0.1);
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            border: 2px solid rgba(255,255,255,0.2);
        }
        
        /* FAQ Section */
        .faq {
            background: #f8f9fa;
        }
        
        .faq-item {
            background: white;
            padding: 25px;
            margin: 20px 0;
            border-radius: 10px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }
        
        .faq-item h3 {
            color: #667eea;
            margin-bottom: 15px;
        }
        
        /* Responsive Design */
        @media (max-width: 1024px) {
            .hero h1 {
                font-size: 3em;
            }
            .section {
                padding: 60px 0;
            }
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 0 15px;
            }
            
            .hero {
                padding: 40px 0;
            }
            
            .hero h1 {
                font-size: 2.2em;
            }
            
            .hero .subheader {
                font-size: 1.2em;
            }
            
            .vsl-placeholder {
                width: 100%;
                max-width: 350px;
                height: 197px;
            }
            
            .section {
                padding: 40px 0;
            }
            
            .section h2 {
                font-size: 2em;
            }
            
            .cta-button {
                padding: 15px 30px;
                font-size: 1.1em;
            }
            
            .framework-steps {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 480px) {
            .hero h1 {
                font-size: 1.8em;
            }
            
            .section h2 {
                font-size: 1.7em;
            }
            
            .vsl-placeholder {
                height: 175px;
            }
            
            .play-button {
                width: 60px;
                height: 60px;
            }
            
            .play-button::after {
                border-left: 18px solid #667eea;
                border-top: 10px solid transparent;
                border-bottom: 10px solid transparent;
            }
        }
        
        .bold { font-weight: bold; }
        .caps { text-transform: uppercase; }
        .italic { font-style: italic; }
        
        .center { text-align: center; }
        
        .large-text { font-size: 1.3em; }
        .small-caps { 
            font-variant: small-caps; 
            font-weight: bold;
            letter-spacing: 1px;
        }
    </style>
</head>
<body>
    <!-- HERO SECTION -->
    <section class="hero">
        <div class="container">
            <div class="preheader">For Struggling Startup Founders & Early-Stage Entrepreneurs</div>
            <h1>From Zero Revenue to Your First <span class="bold">$10K Month</span> in 30 Days</h1>
            <div class="subheader">
                Using the proven PSD Framework... without wasting months building products nobody wants
            </div>
            
            <div class="vsl-container">
                <div class="vsl-placeholder">
                    <div class="play-button"></div>
                </div>
            </div>
            
            <a href="#offer" class="cta-button">Book Your Free Strategy Call</a>
        </div>
    </section>

    <!-- PROBLEM IDENTIFICATION -->
    <section class="section problem">
        <div class="container">
            <h2>The Startup Death Spiral That's Killing Your Dreams</h2>
            
            <p>You had the big idea...</p>
            
            <p>You quit your job (or thought about it)...</p>
            
            <p>You spent months building the "perfect" solution...</p>
            
            <p class="large-text bold">And then... silence.</p>
            
            <div class="highlight">
                <p>You've tried launching on Product Hunt. You've posted in Facebook groups. You've sent cold emails that get ignored.</p>
                
                <p><span class="bold">Your savings account is shrinking.</span> Your family is asking when you'll "get a real job again."</p>
                
                <p>Meanwhile, you watch other founders on Twitter celebrating their first $10K months while you can't even get your first $100.</p>
            </div>
            
            <p>Here's what nobody tells you about startups...</p>
            
            <p>The problem isn't your idea. It's not your skills. It's not even your execution.</p>
            
            <p class="large-text bold">The problem is you're building in the wrong order.</p>
            
            <p>You're starting with the solution... then trying to find people who want it.</p>
            
            <p>But every successful founder I know does the exact opposite.</p>
            
            <div class="testimonial">
                <p>"I spent 8 months building an app that got 12 users. Then I learned Riley's approach and made $7,500 in my first month just by switching the order I did things."</p>
                <strong>- Sarah M., SaaS Founder</strong>
            </div>
        </div>
    </section>

    <!-- ORIGIN STORY -->
    <section class="section origin">
        <div class="container">
            <h2>How I Went From Failed Founder to $10K in 30 Days</h2>
            
            <p>Three years ago, I was you.</p>
            
            <p>I'd launched four different startups. All failures.</p>
            
            <p>I'd spent $30,000 of my own money. Worked 80-hour weeks. Built products that took months to develop.</p>
            
            <p><span class="bold">Zero revenue.</span></p>
            
            <p>I was about to give up and go back to my corporate job when I met a founder who'd built and sold three companies.</p>
            
            <p>Over coffee, he drew three letters on a napkin:</p>
            
            <p class="center large-text bold">P-S-D</p>
            
            <div class="highlight">
                <p>"Riley," he said, "you're doing this backwards."</p>
                
                <p>"Stop building solutions and hoping people want them."</p>
                
                <p>"Start with the problem. Then build the minimum solution. Then distribute it fast."</p>
                
                <p class="bold">"Problem. Solution. Distribution. In that exact order."</p>
            </div>
            
            <p>I thought he was crazy...</p>
            
            <p>But I had nothing left to lose.</p>
            
            <p>30 days later, I had my first $10,000 month.</p>
            
            <p>Not from a complex app. Not from months of development.</p>
            
            <p class="bold">From a simple solution to a real problem that I could sell immediately.</p>
            
            <p>That napkin sketch became the PSD Framework.</p>
            
            <p>And it's the exact same system I now use to help startup founders go from zero to their first consistent revenue...</p>
            
            <p class="bold">In 30 days or less.</p>
        </div>
    </section>

    <!-- SOLUTION REVELATION -->
    <section class="section solution">
        <div class="container">
            <h2>The PSD Framework: Why It Works When Everything Else Fails</h2>
            
            <p>Here's why 90% of startups fail...</p>
            
            <p>They start with the solution. They build first, then try to find buyers.</p>
            
            <p class="bold">But successful founders do it backwards.</p>
            
            <div class="framework-steps">
                <div class="step">
                    <h3>P - PROBLEM</h3>
                    <p>Find the biggest pain point in your target market. Not what you think they need. What they're actively complaining about and willing to pay to solve.</p>
                </div>
                
                <div class="step">
                    <h3>S - SOLUTION</h3>
                    <p>Create the minimum viable solution. Not a perfect product. A quick, testable offer that solves the problem you identified in step 1.</p>
                </div>
                
                <div class="step">
                    <h3>D - DISTRIBUTION</h3>
                    <p>Get it in front of people immediately. Through your network, referrals, and simple outreach. No waiting for the "perfect launch."</p>
                </div>
            </div>
            
            <div class="highlight">
                <p class="bold">Here's the difference:</p>
                
                <p><span class="bold">Old way:</span> Spend 6 months building → Launch → Hope people want it → Usually get zero sales</p>
                
                <p><span class="bold">PSD way:</span> Find problem → Draft quick solution → Test with real people → Make money while you iterate</p>
            </div>
            
            <p>This isn't theory. This is the exact process I used to go from $0 to $10K in 30 days.</p>
            
            <p>And it's what my clients use to:</p>
            
            <ul class="bullets">
                <li><span class="bold">Generate their first $1K in 7 days</span> instead of waiting months for "product-market fit"</li>
                <li><span class="bold">Validate ideas before building anything</span> so they never waste time on products nobody wants</li>
                <li><span class="bold">Turn networking conversations into paying customers</span> instead of just "picking people's brains"</li>
                <li><span class="bold">Build confidence as real entrepreneurs</span> instead of feeling like imposters who can't close deals</li>
            </ul>
            
            <div class="testimonial">
                <p>"I was stuck at $2K months for a year. Riley walked me through PSD and I hit $12K the next month. Same business, completely different approach."</p>
                <strong>- Marcus T., Tech Consultant</strong>
            </div>
        </div>
    </section>

    <!-- PRODUCT INTRODUCTION -->
    <section class="section product">
        <div class="container">
            <h2>Introducing: PSD Framework Strategic Advising</h2>
            
            <p>Look, I could sell you another course...</p>
            
            <p>Another "blueprint" you'll never finish...</p>
            
            <p>Another generic program that treats all startups the same...</p>
            
            <p class="bold">But that's not what gets results.</p>
            
            <div class="highlight">
                <p>What gets results is <span class="italic">personalized guidance</span> from someone who's done it.</p>
                
                <p>Someone who can look at your specific situation and tell you exactly which problem to solve, how to package your solution, and where to find your first customers.</p>
                
                <p>That's what PSD Framework Strategic Advising gives you.</p>
            </div>
            
            <p>Here's what you get:</p>
            
            <ul class="bullets">
                <li><span class="bold">1:1 Strategic Sessions</span> where I personally walk you through each step of PSD for your specific market and situation</li>
                <li><span class="bold">Problem Identification Workshop</span> so you stop guessing what people want and start solving what they're actually willing to pay for</li>
                <li><span class="bold">Rapid Solution Development</span> - I'll help you craft a testable offer in days, not months</li>
                <li><span class="bold">Distribution Strategy & Scripts</span> - The exact outreach methods and messages I use to turn conversations into customers</li>
                <li><span class="bold">Weekly Accountability Check-ins</span> because knowledge without implementation is worthless</li>
                <li><span class="bold">Direct Access for Questions</span> when you hit roadblocks or need quick guidance on next steps</li>
            </ul>
            
            <p>This isn't about theory. It's about getting you to revenue as fast as possible.</p>
            
            <p class="bold">While other founders spend months building products nobody wants, you'll be making money and iterating based on real customer feedback.</p>
        </div>
    </section>

    <!-- OFFER STRUCTURE -->
    <section class="section offer" id="offer">
        <div class="container">
            <h2>Your Fastest Path to $10K Months Starts With One Call</h2>
            
            <p>Here's what I'm offering...</p>
            
            <p>Instead of charging thousands upfront like other startup coaches...</p>
            
            <p>Instead of making you commit to long programs before you know if this works...</p>
            
            <p class="bold">I want to prove the PSD Framework works for YOU first.</p>
            
            <div class="highlight">
                <p class="large-text bold">Book a FREE 45-minute Strategic Call</p>
                
                <p>On this call, I'll:</p>
                <ul class="bullets">
                    <li>Analyze your current startup situation and identify the #1 thing blocking your revenue</li>
                    <li>Show you exactly which problem in your market you should focus on first</li>
                    <li>Map out your fastest path to $1K... then $10K months using PSD</li>
                    <li>Give you a specific action plan you can start implementing immediately</li>
                </ul>
                
                <p>Even if we never work together, you'll leave this call with clarity on exactly what to do next.</p>
            </div>
            
            <div class="guarantee">
                <p class="bold">My Personal Promise:</p>
                <p>If you don't get at least one actionable insight that could change your startup trajectory in the next 30 days, I'll personally send you $100 for wasting your time.</p>
                <p class="italic">That's how confident I am in the PSD Framework.</p>
            </div>
            
            <p class="bold">But here's the thing...</p>
            
            <p>I can only take a limited number of strategy calls each month.</p>
            
            <p>I'm not running some massive coaching empire. This is personal, hands-on advising.</p>
            
            <p class="large-text bold">And January is almost booked.</p>
            
            <a href="#" class="cta-button">Book Your Free Strategy Call Now</a>
            
            <p class="small-caps">Limited Spots Available - First Come, First Served</p>
        </div>
    </section>

    <!-- FAQ SECTION -->
    <section class="section faq">
        <div class="container">
            <h2>The Questions Every Smart Founder Asks</h2>
            
            <div class="faq-item">
                <h3>Can I afford this before my business is making money?</h3>
                <p>The strategy call is completely free. And here's what I've learned: you can't afford NOT to get help. Every month you spend building the wrong thing or targeting the wrong market costs you thousands in lost revenue and wasted time. Most of my clients make back their investment in their first month by finally focusing on what actually drives sales.</p>
            </div>
            
            <div class="faq-item">
                <h3>Will this actually work for me, or did it just work for Riley?</h3>
                <p>I get it. You've been burned by guru promises before. That's exactly why I offer the free strategy call first. You'll see the PSD Framework in action on your own business before making any commitment. Plus, this isn't some untested theory - it's the same approach used by every successful bootstrap founder I know. The framework works because it's based on what customers actually want, not what we think they want.</p>
            </div>
            
            <div class="faq-item">
                <h3>What if I can't execute the outreach part?</h3>
                <p>That's exactly what I help with. I don't just tell you to "do outreach" - I give you the specific scripts, strategies, and step-by-step process I use. Plus, we start with your existing network first, then expand from there. You're not cold-calling strangers. You're having strategic conversations with people who already know and trust you.</p>
            </div>
            
            <div class="faq-item">
                <h3>I don't have weeks or months to waste on another program.</h3>
                <p>Perfect. Because PSD isn't about long programs. It's about fast results. Most clients see their first sales within 2-3 weeks of implementing the framework. We're not building perfect products - we're validating problems and creating quick solutions people will pay for immediately. Speed is the point.</p>
            </div>
            
            <div class="center" style="margin-top: 50px;">
                <a href="#" class="cta-button">Stop Struggling - Book Your Call Today</a>
            </div>
        </div>
    </section>
</body>
</html>
