<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Jeffrina V - Portfolio</title>

    <style>

        * {

            margin: 0;

            padding: 0;

            box-sizing: border-box;

        }



        body {

            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

            line-height: 1.6;

            color: #333;

            background: linear-gradient(135deg, #0f2027 0%, #203a43 50%, #2c5364 100%);

            min-height: 100vh;

        }



        .container {

            max-width: 1200px;

            margin: 0 auto;

            padding: 20px;

        }



        header {

            text-align: center;

            padding: 60px 20px;

            color: white;

            animation: fadeInDown 1s ease;

        }



        @keyframes fadeInDown {

            from {

                opacity: 0;

                transform: translateY(-30px);

            }

            to {

                opacity: 1;

                transform: translateY(0);

            }

        }



        @keyframes fadeInUp {

            from {

                opacity: 0;

                transform: translateY(30px);

            }

            to {

                opacity: 1;

                transform: translateY(0);

            }

        }



        @keyframes slideInLeft {

            from {

                opacity: 0;

                transform: translateX(-50px);

            }

            to {

                opacity: 1;

                transform: translateX(0);

            }

        }



        @keyframes pulse {

            0%, 100% {

                transform: scale(1);

            }

            50% {

                transform: scale(1.05);

            }

        }



        @keyframes shimmer {

            0% {

                background-position: -1000px 0;

            }

            100% {

                background-position: 1000px 0;

            }

        }



        .profile-img {

            width: 150px;

            height: 150px;

            border-radius: 50%;

            border: 5px solid #d4af37;

            margin-bottom: 20px;

            object-fit: cover;

            animation: fadeInDown 1.2s ease, pulse 3s ease-in-out infinite;

            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.4);

        }



        h1 {

            font-size: 2.8em;

            margin-bottom: 10px;

            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);

            color: #d4af37;

            animation: fadeInDown 1.3s ease;

        }



        .tagline {

            font-size: 1.3em;

            opacity: 0.95;

            margin-bottom: 10px;

            color: #fff;

            animation: fadeInDown 1.4s ease;

        }



        .location {

            font-size: 1em;

            opacity: 0.9;

            margin-bottom: 30px;

            animation: fadeInDown 1.5s ease;

        }



        .social-links {

            display: flex;

            justify-content: center;

            gap: 20px;

            flex-wrap: wrap;

            animation: fadeInUp 1.6s ease;

        }



        .social-btn {

            display: inline-flex;

            align-items: center;

            gap: 10px;

            padding: 12px 25px;

            background: linear-gradient(135deg, #d4af37 0%, #f0d978 100%);

            color: #0f2027;

            text-decoration: none;

            border-radius: 30px;

            font-weight: bold;

            transition: all 0.3s ease;

            box-shadow: 0 4px 15px rgba(212, 175, 55, 0.3);

        }



        .social-btn:hover {

            transform: translateY(-3px) scale(1.05);

            box-shadow: 0 6px 20px rgba(212, 175, 55, 0.5);

            background: linear-gradient(135deg, #f0d978 0%, #d4af37 100%);

        }



        .social-btn:active {

            transform: translateY(-1px) scale(1.02);

        }



        .social-btn svg {

            width: 24px;

            height: 24px;

        }



        section {

            background: white;

            margin: 30px 0;

            padding: 40px;

            border-radius: 15px;

            box-shadow: 0 10px 30px rgba(0,0,0,0.15);

            animation: fadeInUp 1s ease;

            border-top: 4px solid #d4af37;

            transition: all 0.3s ease;

        }



        section:hover {

            transform: translateY(-5px);

            box-shadow: 0 15px 40px rgba(0,0,0,0.2);

        }



        h2 {

            color: #0f2027;

            margin-bottom: 25px;

            font-size: 2em;

            border-bottom: 3px solid #d4af37;

            padding-bottom: 10px;

            display: flex;

            align-items: center;

            gap: 10px;

        }



        .section-icon {

            font-size: 1.2em;

            animation: pulse 2s ease-in-out infinite;

        }



        .about-content {

            font-size: 1.1em;

            color: #555;

            line-height: 1.8;

        }



        .skills-grid {

            display: grid;

            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));

            gap: 20px;

            margin-top: 20px;

        }



        .skill-card {

            background: linear-gradient(135deg, #0f2027 0%, #203a43 100%);

            padding: 25px;

            border-radius: 10px;

            color: white;

            transition: transform 0.3s ease, box-shadow 0.3s ease;

            animation: slideInLeft 1s ease;

            border: 2px solid #d4af37;

        }



        .skill-card:nth-child(1) { animation-delay: 0.1s; }

        .skill-card:nth-child(2) { animation-delay: 0.2s; }

        .skill-card:nth-child(3) { animation-delay: 0.3s; }

        .skill-card:nth-child(4) { animation-delay: 0.4s; }



        .skill-card:hover {

            transform: scale(1.05) translateY(-5px) rotate(2deg);

            box-shadow: 0 10px 25px rgba(212, 175, 55, 0.3);

        }



        .skill-card h3 {

            margin-bottom: 15px;

            font-size: 1.3em;

            border-bottom: 2px solid #d4af37;

            padding-bottom: 10px;

            color: #d4af37;

        }



        .skill-card ul {

            list-style: none;

            padding-left: 0;

        }



        .skill-card li {

            padding: 5px 0;

            padding-left: 20px;

            position: relative;

            transition: all 0.3s ease;

        }



        .skill-card li:hover {

            padding-left: 25px;

            color: #d4af37;

        }



        .skill-card li:before {

            content: "▹";

            position: absolute;

            left: 0;

            color: #d4af37;

            font-weight: bold;

        }



        .experience-card {

            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);

            padding: 30px;

            margin: 20px 0;

            border-radius: 10px;

            border-left: 5px solid #0f2027;

            transition: all 0.3s ease;

            animation: fadeInUp 1s ease;

        }



        .experience-card:hover {

            transform: translateX(10px);

            box-shadow: 0 5px 15px rgba(15, 32, 39, 0.2);

            border-left-width: 8px;

        }



        .experience-header {

            display: flex;

            justify-content: space-between;

            align-items: flex-start;

            flex-wrap: wrap;

            margin-bottom: 15px;

        }



        .experience-title {

            color: #0f2027;

            font-size: 1.4em;

            font-weight: bold;

        }



        .experience-date {

            color: #fff;

            font-style: italic;

            font-size: 0.9em;

            background: linear-gradient(135deg, #d4af37 0%, #f0d978 100%);

            padding: 8px 20px;

            border-radius: 20px;

            font-weight: 600;

        }



        .experience-company {

            color: #555;

            font-weight: 600;

            margin-bottom: 10px;

        }



        .project-card {

            background: linear-gradient(135deg, #f8f9fa 0%, #fff 100%);

            padding: 25px;

            margin: 20px 0;

            border-radius: 10px;

            border-left: 5px solid #203a43;

            transition: all 0.3s ease;

            animation: fadeInUp 1s ease;

        }



        .project-card:hover {

            transform: translateX(10px);

            box-shadow: 0 5px 15px rgba(32, 58, 67, 0.2);

            border-left-width: 8px;

        }



        .project-card h3 {

            color: #203a43;

            margin-bottom: 10px;

            font-size: 1.4em;

        }



        .project-tech {

            color: #0f2027;

            font-weight: 600;

            font-size: 0.9em;

            margin-top: 10px;

            padding: 8px 15px;

            background: #e9ecef;

            border-radius: 5px;

            display: inline-block;

        }



        .education-card {

            background: white;

            padding: 25px;

            margin: 20px 0;

            border-radius: 10px;

            border: 2px solid #0f2027;

            transition: all 0.3s ease;

        }



        .education-card:hover {

            box-shadow: 0 8px 20px rgba(15, 32, 39, 0.2);

            transform: translateY(-5px);

            border-color: #d4af37;

        }



        .education-card h3 {

            color: #0f2027;

            margin-bottom: 10px;

            font-size: 1.3em;

        }



        .education-details {

            color: #666;

            margin: 5px 0;

        }



        .percentage {

            background: linear-gradient(135deg, #0f2027 0%, #203a43 100%);

            color: white;

            padding: 8px 20px;

            border-radius: 20px;

            display: inline-block;

            margin-top: 10px;

            font-weight: bold;

            border: 2px solid #d4af37;

            font-size: 1.1em;

        }



        .certificate-card {

            background: linear-gradient(135deg, #fff 0%, #f8f9fa 100%);

            padding: 30px;

            margin: 20px 0;

            border-radius: 15px;

            border: 3px solid #d4af37;

            transition: all 0.3s ease;

            position: relative;

            overflow: hidden;

            box-shadow: 0 5px 15px rgba(212, 175, 55, 0.2);

        }



        .certificate-card:before {

            content: "🏆";

            position: absolute;

            top: -10px;

            right: -10px;

            font-size: 80px;

            opacity: 0.1;

            transform: rotate(15deg);

        }



        .certificate-card:hover {

            transform: scale(1.02) translateY(-5px);

            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.4);

            border-color: #0f2027;

        }



        .certificate-card h3 {

            color: #0f2027;

            margin-bottom: 10px;

            font-size: 1.4em;

            font-weight: bold;

        }



        .workshop-card {

            background: linear-gradient(135deg, #f8f9fa 0%, #fff 100%);

            padding: 30px;

            margin: 20px 0;

            border-radius: 15px;

            border: 3px solid #203a43;

            transition: all 0.3s ease;

            position: relative;

            overflow: hidden;

            box-shadow: 0 5px 15px rgba(32, 58, 67, 0.2);

        }



        .workshop-card:before {

            content: "🎓";

            position: absolute;

            top: -10px;

            right: -10px;

            font-size: 80px;

            opacity: 0.1;

            transform: rotate(-15deg);

        }



        .workshop-card:hover {

            transform: scale(1.02) translateY(-5px);

            box-shadow: 0 10px 30px rgba(32, 58, 67, 0.4);

            border-color: #d4af37;

        }



        .workshop-card h3 {

            color: #203a43;

            margin-bottom: 10px;

            font-size: 1.4em;

            font-weight: bold;

        }



        .languages-grid {

            display: grid;

            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));

            gap: 15px;

            margin-top: 20px;

        }



        .language-item {

            background: linear-gradient(135deg, #0f2027 0%, #203a43 100%);

            color: white;

            padding: 20px;

            border-radius: 10px;

            text-align: center;

            transition: all 0.3s ease;

            border: 2px solid #d4af37;

        }



        .language-item:hover {

            transform: translateY(-5px) scale(1.05);

            box-shadow: 0 10px 20px rgba(212, 175, 55, 0.3);

        }



        .language-name {

            font-weight: bold;

            font-size: 1.2em;

            margin-bottom: 5px;

            color: #d4af37;

        }



        .language-level {

            font-size: 0.9em;

            opacity: 0.9;

        }



        .contact-info {

            display: grid;

            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));

            gap: 20px;

            margin-top: 20px;

        }



        .contact-item {

            background: linear-gradient(135deg, #f8f9fa 0%, #fff 100%);

            padding: 25px;

            border-radius: 10px;

            text-align: center;

            transition: all 0.3s ease;

            border: 2px solid #0f2027;

        }



        .contact-item:hover {

            background: linear-gradient(135deg, #0f2027 0%, #203a43 100%);

            color: white;

            transform: translateY(-5px);

            border-color: #d4af37;

        }



        .contact-item:hover h3 {

            color: #d4af37;

        }



        .contact-item a {

            color: inherit;

            text-decoration: none;

            font-weight: bold;

        }



        footer {

            text-align: center;

            padding: 40px 20px;

            color: white;

            margin-top: 50px;

            background: rgba(0,0,0,0.2);

            border-radius: 15px;

        }



        footer p {

            margin: 10px 0;

            font-size: 1em;

        }



        .footer-heart {

            color: #d4af37;

            animation: pulse 1.5s ease-in-out infinite;

        }



        @media (max-width: 768px) {

            h1 {

                font-size: 2em;

            }

            

            section {

                padding: 25px;

            }

            

            .skills-grid {

                grid-template-columns: 1fr;

            }



            .experience-header {

                flex-direction: column;

            }



            .social-links {

                gap: 10px;

            }



            .social-btn {

                padding: 10px 20px;

                font-size: 0.9em;

            }

        }



        .fade-in {

            opacity: 0;

            animation: fadeInUp 1s ease forwards;

        }



        .badge {

            display: inline-block;

            background: linear-gradient(135deg, #0f2027 0%, #203a43 100%);

            color: white;

            padding: 5px 12px;

            border-radius: 15px;

            font-size: 0.85em;

            margin: 5px 5px 5px 0;

            border: 1px solid #d4af37;

            transition: all 0.3s ease;

        }



        .badge:hover {

            transform: scale(1.1);

            background: linear-gradient(135deg, #d4af37 0%, #f0d978 100%);

            color: #0f2027;

        }


        .download-resume-btn {

            display: inline-block;

            background: linear-gradient(135deg, #d4af37 0%, #f0d978 100%);

            color: #0f2027;

            padding: 15px 40px;

            border-radius: 30px;

            text-decoration: none;

            font-weight: bold;

            font-size: 1.1em;

            margin: 20px auto;

            transition: all 0.3s ease;

            box-shadow: 0 5px 15px rgba(212, 175, 55, 0.3);

            border: 2px solid #0f2027;

        }



        .download-resume-btn:hover {

            transform: translateY(-3px) scale(1.05);

            box-shadow: 0 8px 25px rgba(212, 175, 55, 0.5);

            background: linear-gradient(135deg, #f0d978 0%, #d4af37 100%);

        }



        .download-resume-btn svg {

            width: 20px;

            height: 20px;

            margin-right: 10px;

            vertical-align: middle;

        }



        .skill-item {

            margin-bottom: 20px;

        }



        .skill-name {

            display: flex;

            justify-content: space-between;

            margin-bottom: 8px;

            font-weight: 600;

            color: #0f2027;

        }



        .skill-bar {

            width: 100%;

            height: 12px;

            background: #e9ecef;

            border-radius: 10px;

            overflow: hidden;

            position: relative;

        }



        .skill-progress {

            height: 100%;

            background: linear-gradient(135deg, #d4af37 0%, #f0d978 100%);

            border-radius: 10px;

            transition: width 1.5s ease;

            position: relative;

            overflow: hidden;

        }



        .skill-progress::after {

            content: '';

            position: absolute;

            top: 0;

            left: 0;

            bottom: 0;

            right: 0;

            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);

            animation: shimmer 2s infinite;

        }



        .github-link {

            display: inline-flex;

            align-items: center;

            gap: 8px;

            color: #203a43;

            text-decoration: none;

            font-weight: 600;

            padding: 8px 15px;

            background: #e9ecef;

            border-radius: 20px;

            transition: all 0.3s ease;

            margin-top: 10px;

        }



        .github-link:hover {

            background: #0f2027;

            color: #d4af37;

            transform: translateX(5px);

        }



        .github-link svg {

            width: 18px;

            height: 18px;

        }



        .hobby-grid {

            display: grid;

            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));

            gap: 20px;

            margin-top: 20px;

        }



        .hobby-card {

            background: linear-gradient(135deg, #fff 0%, #f8f9fa 100%);

            padding: 25px;

            border-radius: 10px;

            text-align: center;

            transition: all 0.3s ease;

            border: 2px solid #d4af37;

        }



        .hobby-card:hover {

            transform: translateY(-5px) scale(1.05);

            box-shadow: 0 10px 20px rgba(212, 175, 55, 0.3);

            border-color: #0f2027;

        }



        .hobby-icon {

            font-size: 2.5em;

            margin-bottom: 10px;

        }



        .hobby-title {

            font-weight: bold;

            color: #0f2027;

            font-size: 1.1em;

    }
    

            position: fixed;

            bottom: 30px;

            right: 30px;

            background: linear-gradient(135deg, #d4af37 0%, #f0d978 100%);

            color: #0f2027;

            width: 50px;

            height: 50px;

            border-radius: 50%;

            display: flex;

            align-items: center;

            justify-content: center;

            cursor: pointer;

            box-shadow: 0 4px 15px rgba(212, 175, 55, 0.4);

            transition: all 0.3s ease;

            opacity: 0;

            pointer-events: none;

            z-index: 1000;

            font-size: 1.5em;

            font-weight: bold;

        }



        .scroll-top.visible {

            opacity: 1;

            pointer-events: all;

        }



        .scroll-top:hover {

            transform: translateY(-5px);

            box-shadow: 0 6px 20px rgba(212, 175, 55, 0.6);

        }



        @keyframes fadeIn {

            from { opacity: 0; }

            to { opacity: 1; }

        }



        body {

            animation: fadeIn 0.5s ease-in;

        }

    </style>

    </head>

    <body>

    <div class="container">

        <header>

                   <img src="https://i.ibb.co/202Sjqz6/1768154942607.jpg" alt="Jeffrina V - Profile Photo" class="profile-img">
     

            <h1>Jeffrina V</h1>

            <p class="tagline">Aspiring Data Analyst & Developer</p>

            <p class="location">📍 Coimbatore, Tamil Nadu, India</p>

            

            <div class="social-links">

                <a href="https://www.linkedin.com/in/jeffrina-v-39a0aa354" target="_blank" rel="noopener noreferrer" class="social-btn">

                    <svg fill="currentColor" viewBox="0 0 24 24"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>

                    LinkedIn

                </a>

                

                <a href="https://github.com/Jeffrina-V" target="_blank" rel="noopener noreferrer" class="social-btn">

                    <svg fill="currentColor" viewBox="0 0 24 24"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>

                    GitHub

                </a>

                

                <a href="mailto:jeffrinaviviliya@gmail.com" class="social-btn">

                    <svg fill="currentColor" viewBox="0 0 24 24"><path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg>

                    Email

                </a>



                         <a href="tel:+918838540526" class="social-btn">

                    <svg fill="currentColor" viewBox="0 0 24 24"><path d="M20.01 15.38c-1.23 0-2.42-.2-3.53-.56-.35-.12-.74-.03-1.01.24l-1.57 1.97c-2.83-1.35-5.48-3.9-6.89-6.83l1.95-1.66c.27-.28.35-.67.24-1.02-.37-1.11-.56-2.3-.56-3.53 0-.54-.45-.99-.99-.99H4.19C3.65 3 3 3.24 3 3.99 3 13.28 10.73 21 20.01 21c.71 0 .99-.63.99-1.18v-3.45c0-.54-.45-.99-.99-.99z"/></svg>

                    Call

                </a>

            </div>
                 <div style="margin-top: 30px;">

                <a href="https://drive.google.com/uc?export=download&id=1izsRMxQASWVokF1HpN8sp1TRf0LiD8B8" class="download-resume-btn" target="_blank" rel="noopener noreferrer">

                    <svg fill="currentColor" viewBox="0 0 24 24"><path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/></svg>

                    Download Resume

                </a>

            </div>



        </header>



        <section class="fade-in">

            <h2><span class="section-icon">👤</span> Professional Summary</h2>

            <div class="about-content">

                <p>Aspiring Data Analyst and Developer with strong foundations in programming and data visualization. Skilled in Power BI, Tableau, and Excel for analytics, with experience in Python, C++, and Java for software solutions. Passionate about building real-world projects and contributing to data-driven decision-making and technology development.</p>

                <p style="margin-top: 15px;">Currently seeking opportunities in data analysis, business intelligence, and software development roles where I can apply my technical skills and analytical mindset to solve complex business problems and drive impactful insights.</p>

            </div>

        </section>
             <section class="fade-in">
            <h2><span class="section-icon">💼</span> Professional Experience</h2>
            
            <div class="experience-card">
                <div class="experience-header">
                    <div>
                        <div class="experience-title">Technology Job Simulation</div>
                        <div class="experience-company">Deloitte Australia - via Forage</div>
                    </div>
                    <div class="experience-date">January 2026</div>
                </div>
                <p>Completed a comprehensive job simulation involving software development and coding challenges. Successfully wrote a detailed proposal for creating an interactive dashboard, demonstrating strong analytical and technical writing skills. Gained hands-on experience in real-world business technology scenarios and client-focused solution development.</p>
                <div style="margin-top: 15px;">
                    <span class="badge">Python Programming</span>
                    <span class="badge">Software Development</span>
                    <span class="badge">Dashboard Design</span>
                    <span class="badge">Technical Proposal Writing</span>
                </div>
            </div>
            


            

            <div class="experience-card">

                <div class="experience-header">

                    <div>

                        <div class="experience-title">Data Analyst Intern</div>

                        <div class="experience-company">InnoByte Services, New Delhi</div>

                    </div>

                    <div class="experience-date">August 2025</div>

                </div>

                <p>Demonstrated exceptional dedication, professionalism, and a keen interest in the field of Data Analysis. Consistently performed duties with a high level of competence and enthusiasm. Worked independently as well as part of a team, contributing positively to the department's success.</p>

                <div style="margin-top: 15px;">

                    <span class="badge">Data Analysis</span>

                    <span class="badge">Team Collaboration</span>

                    <span class="badge">Problem Solving</span>

                    <span class="badge">Independent Work</span>

                </div>

            </div>

        </section>



        <section class="fade-in">

            <h2><span class="section-icon">💻</span> Technical Skills</h2>
       <div style="margin-bottom: 30px;">

                <h3 style="color: #0f2027; margin-bottom: 20px; font-size: 1.3em;">Programming Languages</h3>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>Python</span>

                        <span>85%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 85%;"></div>

                    </div>

                </div>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>C++</span>

                        <span>75%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 75%;"></div>

                    </div>

                </div>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>Java</span>

                        <span>70%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 70%;"></div>

                    </div>

                </div>

            </div>



            <div style="margin-bottom: 30px;">

                <h3 style="color: #0f2027; margin-bottom: 20px; font-size: 1.3em;">Data Analytics Tools</h3>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>Power BI</span>

                        <span>80%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 80%;"></div>

                    </div>

                </div>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>Tableau</span>

                        <span>85%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 85%;"></div>

                    </div>

                </div>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>MS Excel</span>

                        <span>90%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 90%;"></div>

                    </div>

                </div>

            </div>



            <div style="margin-bottom: 30px;">

                <h3 style="color: #0f2027; margin-bottom: 20px; font-size: 1.3em;">Web Development</h3>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>HTML5</span>

                        <span>90%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 90%;"></div>

                    </div>

                </div>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>CSS3</span>

                        <span>85%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 85%;"></div>

                    </div>

                </div>

                <div class="skill-item">

                    <div class="skill-name">

                        <span>JavaScript</span>

                        <span>75%</span>

                    </div>

                    <div class="skill-bar">

                        <div class="skill-progress" style="width: 75%;"></div>

                    </div>

                </div>

            </div>


                       <div>

                <h3 style="color: #0f2027; margin-bottom: 20px; font-size: 1.3em;">Soft Skills</h3>

                <div style="display: flex; flex-wrap: wrap; gap: 10px;">

                    <span class="badge">Teamwork</span>

                    <span class="badge">Time Management</span>

                    <span class="badge">Data Visualization</span>

                    <span class="badge">Presentation Skills</span>

                    <span class="badge">Problem Solving</span>

                    <span class="badge">Communication</span>

                </div>

            </div>

        </section>


    



        <section class="fade-in">

            <h2><span class="section-icon">🚀</span> Projects</h2>

            

            <div class="project-card">

                <h3>Stock Price Dashboard</h3>

                <p>Designed comprehensive dashboards to visualize stock trends, moving averages, and sector comparisons using Tableau. Created interactive visualizations that help users analyze market patterns and make informed investment decisions. Implemented data filtering and drill-down capabilities for detailed analysis.</p>

                <div class="project-tech">Technologies: Tableau, Data Visualization, Financial Analysis</div>

            
                  <a href="https://github.com/Jeffrina-V" target="_blank" rel="noopener noreferrer" class="github-link">

                    <svg fill="currentColor" viewBox="0 0 24 24"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>

                    View on GitHub

                </a>

            </div>



            

            <div class="project-card">

                <h3>Library Data Visualization</h3>

                <p>Built comprehensive dashboards to analyze library usage patterns, borrowing trends, and overdue returns. Implemented data-driven insights to improve library management and user experience. Utilized Python for data processing and Tableau for creating interactive visual reports.</p>

                <div class="project-tech">Technologies: Python, Tableau, Data Analysis, Dashboard Design</div>

        
                <a href="https://github.com/Jeffrina-V" target="_blank" rel="noopener noreferrer" class="github-link">
             <svg fill="currentColor" viewBox="0 0 24 24"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>

                    View on GitHub

                </a>

            </div>

        </section>
                <section class="fade-in">

            <h2><span class="section-icon">🎓</span> Education</h2>



    <div class="education-card">

                <h3>Undergraduate Degree - Bachelor of Science (B.Sc.)</h3>

                <div class="education-details"><strong>Computer Science with Data Analytics</strong></div>

                <div class="education-details"><strong>Sankara College of Science and Commerce</strong></div>

                <div class="education-details">Currently Pursuing</div>

                <div class="education-details" style="margin-top: 8px; color: #555; font-style: italic;">An Autonomous Institution | NAAC A+ Grade</div>

                <span class="percentage">CGPA: 90%</span>

                <div style="margin-top: 15px;">

                    <span class="badge">Computer Science</span>

                    <span class="badge">Data Analytics</span>

                    <span class="badge">Mathematics Topper</span>

                </div>

            </div>





        


            <div class="education-card">

                <h3>Higher Secondary Certificate (HSC)</h3>

                <div class="education-details"><strong>Immaculate Matric Higher Secondary School</strong></div>

                <div class="education-details">2023 - 2024</div>

                <span class="percentage">81%</span>

            </div>



            <div class="education-card">

                <h3>Secondary School Leaving Certificate (SSLC)</h3>

                <div class="education-details"><strong>Immaculate Matric Higher Secondary School</strong></div>

                <div class="education-details">2021 - 2022</div>

                <span class="percentage">88%</span>

            </div>

        </section>



        <section class="fade-in">

            <h2><span class="section-icon">🏆</span> Certifications & Achievements</h2>

            

            <div class="certificate-card" style="border-color: #d4af37; background: linear-gradient(135deg, #fffef7 0%, #fff9e6 100%);">

                <h3>🏆 Subject Topper Award - Mathematics</h3>

                <div class="education-details"><strong>Sankara College of Science & Commerce</strong></div>

                <div class="education-details">Department of Mathematics</div>

                <div class="education-details" style="margin-top: 5px;">Academic Year 2024-25</div>

                <div style="margin-top: 15px; padding: 15px; background: white; border-radius: 8px; border-left: 4px solid #d4af37;">

                    <p style="color: #555; line-height: 1.8; margin-bottom: 10px;"><strong>Achievement:</strong> Secured Highest Mark in Mathematics in the Comprehensive External Examinations</p>

                    <p style="color: #0f2027; font-size: 1.1em; font-weight: bold;">Subject: Discrete Mathematics for Data Analytics</p>

                    <p style="color: #d4af37; font-size: 1.3em; font-weight: bold; margin-top: 10px;">Mark Scored: 97/100</p>

                </div>

                <div style="margin-top: 15px;">

                    <span class="badge">Academic Excellence</span>

                    <span class="badge">Mathematics Topper</span>

                    <span class="badge">97 Marks</span>

                    <span class="badge">Data Analytics</span>

                </div>

            </div>



     <div class="certificate-card">

                <h3>Data Analyst Internship Certificate</h3>

                <div class="education-details"><strong>InnoByte Services, New Delhi</strong></div>

                <div class="education-details">August 2025</div>

                <div class="education-details" style="margin-top: 10px; color: #0f2027; font-weight: 600;">Certificate ID: IS/AI/F7103</div>

                <p style="margin-top: 15px; color: #555;">Successfully completed internship demonstrating exceptional dedication, professionalism, and competence in data analysis. Contributed significantly to department success through independent work and team collaboration.</p>

                <div style="margin-top: 15px;">

                    <span class="badge">Data Analysis</span>

                    <span class="badge">Professional Development</span>

                    <span class="badge">Industry Experience</span>

                </div>

            </div>

        </section>



        <section class="fade-in">

            <h2><span class="section-icon">🎓</span> Workshops & Professional Training</h2>

            

            <div class="workshop-card">

                <h3>Data Analyst 30 Days Masterclass</h3>

                <div class="education-details"><strong>Novi Tech Pvt. Ltd</strong></div>

                <div class="education-details">2025</div>

                <p style="margin-top: 15px; color: #555; line-height: 1.8;">Completed intensive 30-day professional training program focused on advanced data analytics techniques, industry best practices, and hands-on project experience. Gained expertise in data visualization, statistical analysis, and business intelligence tools through practical assignments and real-world case studies.</p>

                <div style="margin-top: 15px;">

                    <span class="badge">Data Analytics</span>

                    <span class="badge">Professional Training</span>

                    <span class="badge">Industry Skills</span>

                    <span class="badge">Hands-on Projects</span>

                </div>

            </div>



            <div class="workshop-card">

                <h3>Flutter Development Program</h3>

                <div class="education-details"><strong>Sankara College of Science & Commerce</strong></div>

                <div class="education-details">Department of Computer Science with Data Analytics</div>

                <div class="education-details" style="margin-top: 5px;">February 24-26, 2025</div>

                <p style="margin-top: 15px; color: #555; line-height: 1.8;">Successfully completed comprehensive Flutter Development Program gaining practical skills in developing cross-platform mobile applications using Flutter and Dart, with expertise in UI design, state management, and seamless app deployment.</p>

                <div style="margin-top: 15px;">

                    <span class="badge">Flutter Development</span>

                    <span class="badge">Mobile App Development</span>

                    <span class="badge">Cross-Platform</span>

                    <span class="badge">UI/UX Design</span>

                    <span class="badge">Dart Programming</span>

                </div>

            </div>



            <div class="workshop-card">

                <h3>IoT Display - National Science Day</h3>

                <div class="education-details"><strong>Sankara College of Science & Commerce</strong></div>

                <div class="education-details">Department of Computer Science with Data Analytics</div>

                <div class="education-details" style="margin-top: 5px;">February 28, 2025</div>

                <p style="margin-top: 15px; color: #555; line-height: 1.8;">Participated in IoT Display event at National Science Day, demonstrating knowledge in Internet of Things technologies and practical applications. Engaged in hands-on demonstrations and technical presentations showcasing IoT sensors, connectivity, and real-world implementations.</p>

                <div style="margin-top: 15px;">

                    <span class="badge">IoT Technology</span>

                    <span class="badge">National Science Day</span>

                    <span class="badge">Technical Demonstration</span>

                    <span class="badge">Hardware Integration</span>

                </div>

            </div>

        </section>



        <section class="fade-in">

            <h2><span class="section-icon">🌐</span> Languages</h2>

            <div class="languages-grid">

                <div class="language-item">

                    <div class="language-name">English</div>

                    <div class="language-level">Read / Write / Speak</div>

                </div>

                <div class="language-item">

                    <div class="language-name">Tamil</div>

                    <div class="language-level">Read / Write / Speak</div>

                </div>

                <div class="language-item">

                    <div class="language-name">French</div>

                    <div class="language-level">Read / Write</div>

                </div>

                <div class="language-item">

                    <div class="language-name">Hindi</div>

                    <div class="language-level">Read / Write</div>

                </div>

            </div>

        </section>
        <section class="fade-in">
            <h2><span class="section-icon">🎨</span> Hobbies & Interests</h2>

            <div class="hobby-grid">

                <div class="hobby-card">

                    <div class="hobby-icon">📚</div>

                    <div class="hobby-title">Reading</div>

                    <p style="color: #666; margin-top: 8px; font-size: 0.9em;">Books, articles & literature</p>

                </div>

                <div class="hobby-card">

                    <div class="hobby-icon">💻</div>

                    <div class="hobby-title">Coding</div>

                    <p style="color: #666; margin-top: 8px; font-size: 0.9em;">Personal Projects & Challenges</p>

                </div>

                <div class="hobby-card">

                    <div class="hobby-icon">🎬</div>

                    <div class="hobby-title">Editing</div>

                    <p style="color: #666; margin-top: 8px; font-size: 0.9em;">Video & photo editing</p>

                </div>

                <div class="hobby-card">

                    <div class="hobby-icon">🎓</div>

                    <div class="hobby-title">Learning</div>

                    <p style="color: #666; margin-top: 8px; font-size: 0.9em;">Online Courses & Workshops</p>

                </div>

            </div>

        </section>



       <section class="fade-in">

            <h2><span class="section-icon">📞</span> Get In Touch</h2>

            <div class="contact-info">

                <div class="contact-item">

                    <h3>📧 Email</h3>

                    <a href="mailto:jeffrinaviviliya@gmail.com">jeffrinaviviliya@gmail.com</a>

                </div>

                <div class="contact-item">

                    <h3>📱 Phone</h3>

                    <a href="tel:+918838540526">+91 88385 40526</a>

                </div>

                <div class="contact-item">

                    <h3>📍 Location</h3>

                    <p>Coimbatore, Tamil Nadu</p>

                    <p style="font-size: 0.9em; opacity: 0.8; margin-top: 5px;">India</p>

                </div>

            </div>

        </section>



        <footer>

            <p style="font-size: 1.2em; margin-bottom: 10px;">

                <strong>Jeffrina V</strong>  Portfolio

            </p>

            <p>&copy; 2025 All Rights Reserved</p>

            <p style="margin-top: 10px;">

                Built with <span class="footer-heart">❤️</span> using HTML, CSS & JavaScript

            </p>

            <p style="margin-top: 15px; font-size: 0.9em; opacity: 0.8;">

                Open for Opportunities | Let's Connect!

            </p>

        </footer>

    </div>



    <div class="scroll-top" id="scrollTop" onclick="scrollToTop()">

        ↑

    </div>



    <script>

        const observerOptions = {

            threshold: 0.1,

            rootMargin: '0px 0px -50px 0px'

        };



        const observer = new IntersectionObserver((entries) => {

            entries.forEach(entry => {

                if (entry.isIntersecting) {

                    entry.target.style.opacity = '1';

                    entry.target.style.transform = 'translateY(0)';

                }

            });

        }, observerOptions);



        document.querySelectorAll('.fade-in').forEach(el => {

            observer.observe(el);

        });



        document.querySelectorAll('.social-btn').forEach(btn => {

            btn.addEventListener('click', function(e) {

                this.style.transform = 'scale(0.95)';

                setTimeout(() => {

                    this.style.transform = '';

                }, 150);

            });

        });



        const skillCards = document.querySelectorAll('.skill-card');

        skillCards.forEach((card, index) => {

            card.style.animationDelay = `${index * 0.15}s`;

        });



        const scrollTopBtn = document.getElementById('scrollTop');



        window.addEventListener('scroll', () => {

            if (window.pageYOffset > 300) {

                scrollTopBtn.classList.add('visible');

            } else {

                scrollTopBtn.classList.remove('visible');

            }

        });



        function scrollToTop() {

            window.scrollTo({

                top: 0,

                behavior: 'smooth'

            });

        }



        document.querySelectorAll('a[href^="#"]').forEach(anchor => {

            anchor.addEventListener('click', function (e) {

                e.preventDefault();

                const target = document.querySelector(this.getAttribute('href'));

                if (target) {

                    target.scrollIntoView({

                        behavior: 'smooth',

                        block: 'start'

                    });

                }

            });

        });



        window.addEventListener('load', () => {

            document.body.style.opacity = '1';

        });



        document.querySelectorAll('.skill-card, .project-card, .education-card, .certificate-card, .workshop-card').forEach(card => {

            card.addEventListener('mouseenter', function() {

                this.style.transition = 'all 0.3s ease';

            });

        });

    console.log('%c👋 Welcome to Jeffrina V\'s Portfolio!', 'color: #0f2027; font-size: 20px; font-weight: bold;');

        console.log('%c📧 Contact: jeffrinaviviliya@gmail.com', 'color: #d4af37; font-size: 14px;');

        console.log('%c🔗 LinkedIn: https://www.linkedin.com/in/jeffrina-v-39a0aa354', 'color: #203a43; font-size: 14px;');



        const currentYear = new Date().getFullYear();

        const footerText = document.querySelector('footer p:nth-child(2)');

        if (footerText) {

            footerText.textContent = `© ${currentYear} All Rights Reserved`;

        }

    </script>

    </body>

    </html>


