<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Md Meherab Hossen | MERN Stack Developer</title>
    <!-- Google Fonts & Font Awesome -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Animate on Scroll (AOS) -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: #0a0f1f;
            color: #eef2ff;
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* Custom gradient & glass effects */
        .glass-card {
            background: rgba(18, 25, 45, 0.7);
            backdrop-filter: blur(12px);
            border-radius: 2rem;
            border: 1px solid rgba(255, 255, 255, 0.08);
            box-shadow: 0 20px 35px -12px rgba(0, 0, 0, 0.4);
        }

        .neon-border {
            transition: all 0.3s ease;
            border-image: none;
        }

        .neon-border:hover {
            border-color: #f70000;
            box-shadow: 0 0 18px rgba(247, 0, 0, 0.3);
        }

        /* banner image container */
        .banner-wrapper {
            width: 100%;
            border-radius: 2rem;
            overflow: hidden;
            margin-bottom: 1.5rem;
            box-shadow: 0 25px 40px -12px rgba(0, 0, 0, 0.5);
            transition: transform 0.4s ease;
        }
        .banner-wrapper img {
            width: 100%;
            display: block;
            object-fit: cover;
            transition: transform 0.6s cubic-bezier(0.2, 0.9, 0.4, 1.1);
        }
        .banner-wrapper:hover img {
            transform: scale(1.02);
        }

        /* typing cursor effect */
        .typing-highlight {
            background: linear-gradient(120deg, #f70000, #ff5e5e);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            font-weight: 700;
        }

        /* profile image / avatar side */
        .avatar-decor {
            background: linear-gradient(135deg, #f70000, #b91c1c);
            padding: 3px;
            border-radius: 50%;
            display: inline-block;
        }

        .avatar-decor img {
            border-radius: 50%;
            width: 100%;
            height: 100%;
            object-fit: cover;
            background: #0a0f1f;
        }

        /* skill icons hover */
        .skill-icon {
            transition: all 0.25s ease;
            filter: drop-shadow(0 4px 6px rgba(0,0,0,0.3));
        }
        .skill-icon:hover {
            transform: translateY(-8px) scale(1.08);
            filter: drop-shadow(0 12px 15px rgba(247,0,0,0.3));
        }

        /* social links */
        .social-link {
            background: rgba(255,255,255,0.05);
            transition: all 0.25s;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            border-radius: 40px;
            padding: 0.6rem 1.2rem;
            gap: 0.6rem;
            backdrop-filter: blur(4px);
        }
        .social-link:hover {
            background: #f70000;
            color: white !important;
            transform: translateY(-3px);
        }
        .social-link i {
            font-size: 1.3rem;
        }

        /* stats cards */
        .stat-card {
            background: rgba(12, 18, 34, 0.8);
            border-radius: 1.5rem;
            padding: 1rem;
            transition: all 0.3s;
            border: 1px solid rgba(247, 0, 0, 0.2);
        }
        .stat-card:hover {
            border-color: #f70000;
            transform: scale(1.02);
        }

        /* button */
        .btn-primary {
            background: linear-gradient(95deg, #f70000, #b91c1c);
            border: none;
            padding: 0.7rem 1.8rem;
            border-radius: 40px;
            font-weight: 600;
            transition: 0.2s;
            color: white;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }
        .btn-primary:hover {
            transform: scale(1.03);
            box-shadow: 0 10px 20px -5px #f7000080;
            background: linear-gradient(95deg, #ff1a1a, #d10000);
        }

        /* scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #101624;
        }
        ::-webkit-scrollbar-thumb {
            background: #f70000;
            border-radius: 10px;
        }

        /* responsive */
        @media (max-width: 768px) {
            .glass-card {
                padding: 1.5rem !important;
            }
            .social-link span {
                display: none;
            }
            .social-link {
                padding: 0.7rem;
            }
            .social-link i {
                margin: 0;
            }
        }
        .gradient-text {
            background: linear-gradient(130deg, #ffffff, #ffb3b3);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
        }
    </style>

</head>
<body>

    <!-- particle / decorative background (simple) -->
    <div style="position: fixed; top:0; left:0; width:100%; height:100%; background: radial-gradient(circle at 20% 40%, #1a1f2f, #070b14); z-index:-2;"></div>
    <div style="position: fixed; top:0; left:0; width:100%; height:100%; background-image: radial-gradient(rgba(247,0,0,0.08) 1px, transparent 1px); background-size: 35px 35px; z-index:-1;"></div>

    <div class="container" style="max-width: 1300px; margin: 0 auto; padding: 2rem 1.5rem 4rem;">

        <!-- Banner Image from GitHub -->
        <div data-aos="fade-down" data-aos-duration="800" class="banner-wrapper">
            <img src="https://github.com/MAHIR-DEVES/MAHIR-DEVES/blob/main/github%20banner.png?raw=true" alt="GitHub Banner" onerror="this.src='https://placehold.co/1200x400/1a1f2f/f70000?text=MD+MEHERAB+HOSSEN'">
        </div>

        <!-- Header with profile section -->
        <div class="glass-card" style="padding: 2rem 2rem 1.8rem; margin-bottom: 2rem;" data-aos="fade-up">
            <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; gap: 1.5rem;">
                <div style="display: flex; align-items: center; gap: 1.2rem; flex-wrap: wrap;">
                    <div class="avatar-decor" style="width: 85px; height: 85px;">
                        <img src="https://avatars.githubusercontent.com/u/MAHIR-DEVES?size=100" alt="Md Meherab Hossen" onerror="this.src='https://ui-avatars.com/api/?background=f70000&color=fff&name=MD+Meherab'">
                    </div>
                    <div>
                        <h1 style="font-size: 2rem; font-weight: 800; letter-spacing: -0.02em;">Md Meherab Hossen</h1>
                        <div style="display: flex; gap: 0.5rem; flex-wrap: wrap; margin-top: 0.4rem;">
                            <span class="glass-card" style="padding: 0.25rem 0.9rem; font-size: 0.85rem; background: rgba(247,0,0,0.2); border-radius: 40px;"><i class="fas fa-map-marker-alt" style="color:#f70000;"></i> Rajshahi, Bangladesh</span>
                            <span class="glass-card" style="padding: 0.25rem 0.9rem; font-size: 0.85rem;"><i class="fas fa-code"></i> MERN Stack Developer</span>
                        </div>
                    </div>
                </div>
                <div>
                    <a href="#contact" class="btn-primary"><i class="fas fa-paper-plane"></i> Contact Me</a>
                </div>
            </div>
            <div style="margin-top: 1.2rem;">
                <div class="typing-highlight" style="font-size: 1.2rem; font-weight: 500;">
                    <i class="fas fa-terminal"></i>
                    <span id="typed-text"></span><span class="cursor" style="color:#f70000;">|</span>
                </div>
                <p style="margin-top: 1rem; line-height: 1.5; opacity: 0.85;">🚀 Passionate frontend & MERN developer crafting modern web experiences. I love building scalable applications with React, Node.js, and cloud technologies. Always curious, always coding.</p>
            </div>
        </div>

        <!-- Stats & Visitor Counter Row -->
        <div style="display: flex; flex-wrap: wrap; gap: 1.5rem; justify-content: space-between; margin-bottom: 2rem;" data-aos="fade-up" data-aos-delay="100">
            <div class="stat-card" style="flex: 1; min-width: 150px;">
                <div style="display: flex; align-items: center; gap: 0.8rem;">
                    <i class="fas fa-eye" style="font-size: 2rem; color:#f70000;"></i>
                    <div>
                        <div style="font-size: 0.8rem; text-transform: uppercase; letter-spacing: 1px;">Profile Views</div>
                        <div style="font-size: 1.8rem; font-weight: 700;" id="viewCount">1,284</div>
                    </div>
                </div>
            </div>
            <div class="stat-card" style="flex: 1; min-width: 150px;">
                <div style="display: flex; align-items: center; gap: 0.8rem;">
                    <i class="fab fa-github" style="font-size: 2rem; color:#f70000;"></i>
                    <div>
                        <div style="font-size: 0.8rem;">GitHub Repos</div>
                        <div style="font-size: 1.6rem; font-weight: 700;">12+</div>
                    </div>
                </div>
            </div>
            <div class="stat-card" style="flex: 1; min-width: 150px;">
                <div style="display: flex; align-items: center; gap: 0.8rem;">
                    <i class="fas fa-code-branch" style="font-size: 2rem; color:#f70000;"></i>
                    <div>
                        <div style="font-size: 0.8rem;">Projects</div>
                        <div style="font-size: 1.6rem; font-weight: 700;">20+</div>
                    </div>
                </div>
            </div>
            <div class="stat-card" style="flex: 1; min-width: 150px;">
                <div style="display: flex; align-items: center; gap: 0.8rem;">
                    <i class="fas fa-coffee" style="font-size: 2rem; color:#f70000;"></i>
                    <div>
                        <div style="font-size: 0.8rem;">Fun fact</div>
                        <div style="font-size: 1rem; font-weight: 500;">i am funny 😍</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Connect with me & Social + contact info row -->
        <div class="glass-card" style="padding: 1.8rem; margin-bottom: 2rem;" data-aos="fade-right">
            <h3 style="font-size: 1.6rem; margin-bottom: 1.2rem; display: flex; align-items: center; gap: 0.5rem;"><i class="fas fa-share-alt" style="color:#f70000;"></i> Connect with me</h3>
            <div style="display: flex; flex-wrap: wrap; gap: 1rem; justify-content: flex-start;">
                <a href="https://x.com/mdmeher25341474" target="_blank" class="social-link" style="color: white; text-decoration: none;">
                    <i class="fab fa-twitter"></i><span>Twitter</span>
                </a>
                <a href="https://www.linkedin.com/in/md-meherab-07565a26b/" target="_blank" class="social-link" style="color: white; text-decoration: none;">
                    <i class="fab fa-linkedin-in"></i><span>LinkedIn</span>
                </a>
                <a href="https://www.facebook.com/profile.php?id=61583916434295" target="_blank" class="social-link" style="color: white; text-decoration: none;">
                    <i class="fab fa-facebook-f"></i><span>Facebook</span>
                </a>
                <a href="https://www.instagram.com/mdmeherab41/" target="_blank" class="social-link" style="color: white; text-decoration: none;">
                    <i class="fab fa-instagram"></i><span>Instagram</span>
                </a>
                <div class="social-link" style="background: transparent; border: 1px solid rgba(247,0,0,0.5);">
                    <i class="fas fa-envelope"></i><span>mdmeherab657@gmail.com</span>
                </div>
            </div>
        </div>

        <!-- Languages and Tools section - modern grid -->
        <div data-aos="fade-up" style="margin-bottom: 2rem;">
            <h3 style="font-size: 1.7rem; margin-bottom: 1.2rem;"><i class="fas fa-cogs"></i> Tech Stack & Tools</h3>
            <div class="glass-card" style="padding: 2rem;">
                <div style="display: flex; flex-wrap: wrap; gap: 1.8rem; justify-content: center; align-items: center;">
                    <!-- icons with tooltips / modern representation -->
                    <div class="skill-icon" title="JavaScript"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="48" height="48"/></div>
                    <div class="skill-icon" title="TypeScript"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" width="48" height="48"/></div>
                    <div class="skill-icon" title="React"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original-wordmark.svg" width="52" height="52"/></div>
                    <div class="skill-icon" title="Next.js"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original-wordmark.svg" width="52" height="52" style="filter: brightness(0) invert(1);"/></div>
                    <div class="skill-icon" title="Node.js"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original-wordmark.svg" width="52" height="52"/></div>
                    <div class="skill-icon" title="MongoDB"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original-wordmark.svg" width="52" height="52"/></div>
                    <div class="skill-icon" title="MySQL"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original-wordmark.svg" width="52" height="52"/></div>
                    <div class="skill-icon" title="PostgreSQL"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original-wordmark.svg" width="52" height="52"/></div>
                    <div class="skill-icon" title="Prisma"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/prisma/prisma-original.svg" width="48" height="48"/></div>
                    <div class="skill-icon" title="Docker"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original-wordmark.svg" width="52" height="52"/></div>
                    <div class="skill-icon" title="AWS"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" width="52" height="52"/></div>
                    <div class="skill-icon" title="GoLang"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/go/go-original-wordmark.svg" width="52" height="52"/></div>
                    <div class="skill-icon" title="Redux"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redux/redux-original.svg" width="48" height="48"/></div>
                    <div class="skill-icon" title="Postman"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postman/postman-original.svg" width="48" height="48"/></div>
                </div>
                <div style="margin-top: 1.5rem; text-align: center; font-size: 0.85rem; opacity: 0.7;">MERN | Next.js | TypeScript | Cloud Native</div>
            </div>
        </div>

        <!-- GitHub Stats Section with 3 columns (modern layout) -->
        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 1.8rem; margin-bottom: 2rem;" data-aos="zoom-in-up">
            <div class="glass-card" style="padding: 1.5rem; text-align: center;">
                <h4><i class="fas fa-chart-line"></i> Top Languages</h4>
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mahir-deves&show_icons=true&theme=radical&layout=compact&hide_border=true&bg_color=0a0f1f&title_color=f70000&text_color=ffffff" alt="Top Langs" style="width: 100%; border-radius: 16px; margin-top: 0.6rem;">
            </div>
            <div class="glass-card" style="padding: 1.5rem; text-align: center;">
                <h4><i class="fab fa-github-alt"></i> GitHub Stats</h4>
                <img src="https://github-readme-stats.vercel.app/api?username=mahir-deves&show_icons=true&theme=radical&hide_border=true&bg_color=0a0f1f&icon_color=f70000&title_color=f70000&text_color=dddddd" alt="GitHub Stats" style="width: 100%; border-radius: 16px;">
            </div>
            <div class="glass-card" style="padding: 1.5rem; text-align: center;">
                <h4><i class="fas fa-fire"></i> Contribution Streak</h4>
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=mahir-deves&theme=dark&hide_border=true&background=0a0f1f&stroke=f70000&ring=f70000&fire=f70000&currStreakLabel=f70000" alt="Streak Stats" style="width: 100%; border-radius: 16px;">
            </div>
        </div>

        <!-- Fun fact + extra quote -->
        <div class="glass-card" style="padding: 1.5rem 2rem; background: linear-gradient(145deg, #0f1428, #090c18); margin-bottom: 2rem; text-align: center;" data-aos="flip-up">
            <i class="fas fa-laptop-code" style="font-size: 2rem; color:#f70000;"></i>
            <p style="margin-top: 0.5rem; font-style: italic; font-size: 1.1rem;">"Code is like humor. When you have to explain it, it’s bad." – but my code? 🔥 Clean & modern.</p>
            <div style="margin-top: 0.6rem;"><span class="badge" style="background:#f7000022; padding: 0.3rem 1rem; border-radius: 40px;">⚡ Fun fact: i am funny 😍 & I love to merge creativity with logic.</span></div>
        </div>

        <!-- Contact / email section -->
        <div id="contact" class="glass-card" style="padding: 2rem; text-align: center;" data-aos="fade-up">
            <h3><i class="fas fa-envelope-open-text"></i> Let's work together</h3>
            <p style="margin: 0.8rem 0;">📫 Reach out for collaborations or just a chat :)</p>
            <a href="mailto:mdmeherab657@gamil.com" class="btn-primary" style="background: #b91c1c; margin-top: 0.5rem;"><i class="fas fa-paper-plane"></i> mdmeherab657@gmail.com</a>
            <div style="margin-top: 1rem; font-size: 0.8rem;">⭐ Open for freelance & full-time opportunities</div>
        </div>

        <footer style="margin-top: 3rem; text-align: center; font-size: 0.75rem; opacity: 0.6;">
            <p>© 2025 Md Meherab Hossen — MERN Stack Developer from Rajshahi, Bangladesh</p>
        </footer>
    </div>

    <!-- AOS & Typing effect JS -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true, offset: 20 });

        // Typing effect for dynamic text
        const phrases = [
            "A passionate frontend developer!",
            "I'm a MERN Stack Developer",
            "From Rajshahi, Bangladesh"
        ];
        let phraseIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        const typedTextSpan = document.getElementById("typed-text");

        function typeEffect() {
            const currentPhrase = phrases[phraseIndex];
            if (isDeleting) {
                typedTextSpan.innerText = currentPhrase.substring(0, charIndex - 1);
                charIndex--;
                if (charIndex === 0) {
                    isDeleting = false;
                    phraseIndex = (phraseIndex + 1) % phrases.length;
                }
            } else {
                typedTextSpan.innerText = currentPhrase.substring(0, charIndex + 1);
                charIndex++;
                if (charIndex === currentPhrase.length) {
                    isDeleting = true;
                    setTimeout(() => {}, 1500);
                }
            }
            const speed = isDeleting ? 60 : 100;
            setTimeout(typeEffect, speed);
        }
        typeEffect();

        // Simulate visitor counter (just for design flare - increments randomly on load, but smooth)
        let viewEl = document.getElementById('viewCount');
        let currentViews = 1284;
        const increment = Math.floor(Math.random() * 35) + 1;
        let targetViews = currentViews + increment;
        let step = 1;
        function updateCounter() {
            if (currentViews < targetViews) {
                currentViews += step;
                viewEl.innerText = currentViews.toLocaleString();
                setTimeout(updateCounter, 20);
            } else {
                viewEl.innerText = targetViews.toLocaleString();
            }
        }
        updateCounter();

        // Adding a little hover effect for stats and skill icons (already via CSS)
        // Also fix any broken image fallback for banner if raw github fails
        const bannerImg = document.querySelector('.banner-wrapper img');
        if(bannerImg) {
            bannerImg.addEventListener('error', function() {
                this.src = 'https://placehold.co/1200x400/1a1f2f/f70000?text=MD+MEHERAB+HOSSEN+%7C+MERN+DEV';
            });
        }
        const avatarImg = document.querySelector('.avatar-decor img');
        if(avatarImg) {
            avatarImg.addEventListener('error', function() {
                this.src = 'https://ui-avatars.com/api/?background=f70000&color=fff&name=MD+Meherab&size=100';
            });
        }
    </script>

</body>
</html>
