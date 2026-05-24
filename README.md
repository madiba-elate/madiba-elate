<!DOCTYPE html>
<html lang="fr" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Madiba Elate | Architecte Logiciel & Chercheur IA</title>
    
    <!-- Intégration de Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts pour un look "Développeur / Cyber" -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@300;400;600&family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
    
    <!-- Icônes Lucide -->
    <script src="https://unpkg.com/lucide@latest"></script>

    <!-- Configuration Tailwind personnalisée -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        mono: ['Fira Code', 'monospace'],
                    },
                    colors: {
                        brand: {
                            dark: '#0f172a',
                            light: '#e2e8f0',
                            accent: '#38bdf8', // Bleu cyan tech
                            purple: '#8b5cf6'  // Touche IA/Maths
                        }
                    }
                }
            }
        }
    </script>

    <style>
        /* Effet de verre (Glassmorphism) pour les cartes */
        .glass-card {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s ease;
        }
        .glass-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px -10px rgba(56, 189, 248, 0.3);
            border-color: rgba(56, 189, 248, 0.5);
        }
        
        /* Animation du texte gradient */
        .text-gradient {
            background: linear-gradient(to right, #38bdf8, #8b5cf6);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="bg-brand-dark text-brand-light font-sans antialiased selection:bg-brand-accent selection:text-white relative min-h-screen">

    <!-- Canvas pour l'arrière-plan interactif (Particules/Réseau) -->
    <canvas id="bg-canvas" class="fixed inset-0 z-0 pointer-events-none opacity-30"></canvas>

    <!-- Conteneur principal -->
    <div class="relative z-10 max-w-5xl mx-auto px-6 py-16 md:py-24 space-y-24">

        <!-- HEADER / HERO SECTION -->
        <header class="space-y-6 text-center md:text-left">
            <div class="inline-block px-4 py-1.5 rounded-full border border-brand-accent/30 bg-brand-accent/10 text-brand-accent text-sm font-mono mb-4">
                <i data-lucide="terminal" class="inline w-4 h-4 mr-2 -mt-0.5"></i>
                Initialisation du système... Bienvenue.
            </div>
            <h1 class="text-4xl md:text-6xl font-extrabold tracking-tight">
                Salut, moi c'est <br class="md:hidden" />
                <span class="text-gradient">Albert Emmanuel Madiba Elate</span> 👋
            </h1>
            <p class="text-lg md:text-xl text-slate-400 leading-relaxed max-w-3xl">
                Je suis un jeune chercheur en informatique théorique, architecte logiciel et passionné d'intelligence artificielle basé à Douala, Cameroun. Tout en menant un parcours académique d'excellence en Première C au Lycée Joss, je consacre mon temps à concevoir des technologies de rupture et des infrastructures de bas niveau sous l'égide de mon laboratoire de R&D, <strong class="text-white">OmniGroup</strong> 
                <span class="italic text-brand-purple">(*Innovation as a vector of sovereignty*)</span>.
            </p>
        </header>

        <!-- PROJETS : OMNIGROUP -->
        <section class="space-y-8">
            <div class="flex items-center space-x-3 border-b border-slate-700 pb-4">
                <i data-lucide="building-2" class="w-8 h-8 text-brand-accent"></i>
                <h2 class="text-2xl md:text-3xl font-bold text-white">Le Projet d'une Vie : OmniGroup & R&D</h2>
            </div>
            <p class="text-slate-400">Je construis un écosystème technologique souverain astrophysique et informatique articulé autour de plusieurs piliers d'ingénierie profonde :</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Carte Genesis -->
                <div class="glass-card p-6 rounded-2xl">
                    <div class="flex items-center space-x-3 mb-4">
                        <div class="p-2 bg-blue-500/20 rounded-lg text-blue-400"><i data-lucide="code-2"></i></div>
                        <h3 class="text-xl font-bold text-white">Genesis Language</h3>
                    </div>
                    <p class="text-slate-400 text-sm leading-relaxed">Conception et développement d'un langage de programmation de bas niveau ultra-optimisé, unifié pour le web, le mobile et l'embarqué (avec un parser récursif haute-performance et AST robuste).</p>
                </div>
                
                <!-- Carte CodeFlow -->
                <div class="glass-card p-6 rounded-2xl">
                    <div class="flex items-center space-x-3 mb-4">
                        <div class="p-2 bg-purple-500/20 rounded-lg text-purple-400"><i data-lucide="cpu"></i></div>
                        <h3 class="text-xl font-bold text-white">CodeFlow IDE & Proton Ecosystem</h3>
                    </div>
                    <p class="text-slate-400 text-sm leading-relaxed">Création d'un environnement de développement intégré moderne et d'outils de productivité système pour développeurs.</p>
                </div>

                <!-- Carte Pangea AI -->
                <div class="glass-card p-6 rounded-2xl">
                    <div class="flex items-center space-x-3 mb-4">
                        <div class="p-2 bg-emerald-500/20 rounded-lg text-emerald-400"><i data-lucide="brain-circuit"></i></div>
                        <h3 class="text-xl font-bold text-white">Pangea AI</h3>
                    </div>
                    <p class="text-slate-400 text-sm leading-relaxed">Un grand modèle de langage (LLM) souverain conçu spécifiquement pour la préservation et le traitement des langues africaines.</p>
                </div>

                <!-- Carte Omni-Fleet -->
                <div class="glass-card p-6 rounded-2xl">
                    <div class="flex items-center space-x-3 mb-4">
                        <div class="p-2 bg-orange-500/20 rounded-lg text-orange-400"><i data-lucide="network"></i></div>
                        <h3 class="text-xl font-bold text-white">OMNI-FLEET-INFINITY</h3>
                    </div>
                    <p class="text-slate-400 text-sm leading-relaxed">Orchestration d'architectures d'automatisation résilientes, d'infrastructures cloud multi-services (Docker, Kubernetes) et d'agents IA autonomes (RAG, LangChain).</p>
                </div>
            </div>
        </section>

        <!-- STACK TECHNIQUE -->
        <section class="space-y-8">
            <div class="flex items-center space-x-3 border-b border-slate-700 pb-4">
                <i data-lucide="layers" class="w-8 h-8 text-brand-purple"></i>
                <h2 class="text-2xl md:text-3xl font-bold text-white">Stack Technique & Expertise</h2>
            </div>
            
            <div class="space-y-6">
                <!-- Ligne Langages -->
                <div class="bg-slate-800/50 p-4 rounded-xl border border-slate-700/50 flex flex-col md:flex-row md:items-center">
                    <div class="md:w-1/4 font-semibold text-slate-300 mb-3 md:mb-0">Langages</div>
                    <div class="flex flex-wrap gap-2 md:w-3/4">
                        <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
                        <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
                        <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++">
                        <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter">
                        <img src="https://img.shields.io/badge/Shell_Script-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white" alt="Bash">
                        <img src="https://img.shields.io/badge/SQL-4169E1?style=flat-square&logo=sqlite&logoColor=white" alt="SQL">
                    </div>
                </div>

                <!-- Ligne IA & Cloud -->
                <div class="bg-slate-800/50 p-4 rounded-xl border border-slate-700/50 flex flex-col md:flex-row md:items-center">
                    <div class="md:w-1/4 font-semibold text-slate-300 mb-3 md:mb-0">IA & Cloud</div>
                    <div class="flex flex-wrap gap-2 md:w-3/4">
                        <img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-FFD21E?style=flat-square" alt="Hugging Face">
                        <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=chainlink&logoColor=white" alt="LangChain">
                        <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
                    </div>
                </div>

                <!-- Ligne DB -->
                <div class="bg-slate-800/50 p-4 rounded-xl border border-slate-700/50 flex flex-col md:flex-row md:items-center">
                    <div class="md:w-1/4 font-semibold text-slate-300 mb-3 md:mb-0">Bases de données</div>
                    <div class="flex flex-wrap gap-2 md:w-3/4">
                        <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
                        <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis">
                    </div>
                </div>

                <!-- Ligne Systèmes -->
                <div class="bg-slate-800/50 p-4 rounded-xl border border-slate-700/50 flex flex-col md:flex-row md:items-center">
                    <div class="md:w-1/4 font-semibold text-slate-300 mb-3 md:mb-0">Systèmes</div>
                    <div class="flex flex-wrap gap-2 md:w-3/4">
                        <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">
                        <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
                        <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare">
                    </div>
                </div>
            </div>
        </section>

        <!-- OBJECTIFS & PHILOSOPHIE -->
        <section class="space-y-8">
            <div class="flex items-center space-x-3 border-b border-slate-700 pb-4">
                <i data-lucide="target" class="w-8 h-8 text-rose-400"></i>
                <h2 class="text-2xl md:text-3xl font-bold text-white">Objectifs & Philosophie</h2>
            </div>
            <ul class="space-y-4">
                <li class="flex items-start">
                    <i data-lucide="graduation-cap" class="w-6 h-6 text-brand-accent mr-3 flex-shrink-0 mt-1"></i>
                    <div>
                        <strong class="text-white text-lg">Ambition Académique :</strong>
                        <p class="text-slate-400">Préparation rigoureuse et active pour intégrer les universités d'élite mondiales (notamment le <strong class="text-white">MIT</strong> et l'Ivy League en <em class="text-brand-purple">Computer Science</em>).</p>
                    </div>
                </li>
                <li class="flex items-start">
                    <i data-lucide="globe-2" class="w-6 h-6 text-brand-accent mr-3 flex-shrink-0 mt-1"></i>
                    <div>
                        <strong class="text-white text-lg">Impact & Souveraineté :</strong>
                        <p class="text-slate-400">Utiliser la technologie comme un levier d'émancipation sociale et financière en Afrique à travers des micro-SaaS d'inclusion financière (FinTech, tontines numériques, gestion d'actifs).</p>
                    </div>
                </li>
                <li class="flex items-start">
                    <i data-lucide="compass" class="w-6 h-6 text-brand-accent mr-3 flex-shrink-0 mt-1"></i>
                    <div>
                        <strong class="text-white text-lg">Discipline de Vie :</strong>
                        <p class="text-slate-400">Rigoureuse organisation du travail (<em class="text-brand-accent">Zero Desktop</em>, triptyque d'apprentissage <em class="text-brand-purple">Imperium, Lab, Academia</em>), végétarisme et exploration linguistique (français, anglais C2, russe, latin, italien, japonais).</p>
                    </div>
                </li>
            </ul>
        </section>

        <!-- STATS GITHUB -->
        <section class="space-y-8">
            <div class="flex items-center space-x-3 border-b border-slate-700 pb-4">
                <i data-lucide="bar-chart-3" class="w-8 h-8 text-emerald-400"></i>
                <h2 class="text-2xl md:text-3xl font-bold text-white">Statistiques d'Activité GitHub</h2>
            </div>
            <blockquote class="border-l-4 border-brand-accent pl-4 italic text-slate-300 py-2 bg-slate-800/30 rounded-r-lg">
                « La rigueur scientifique n'attend pas le nombre des années. Le code n'est qu'un outil ; le but final est l'impact humain et la conscience de notre souveraineté. »
            </blockquote>
            
            <p class="text-sm text-slate-500 italic text-center">
                (Les statistiques d'activité ci-dessous s'initialiseront automatiquement dès la publication de tes premiers commits sur tes différents dépôts R&D).
            </p>

            <div class="flex flex-col md:flex-row justify-center items-center gap-4">
                <!-- On garde les balises img dynamiques du readme -->
                <img src="https://github-readme-stats.vercel.app/api?username=madiba-elate&show_icons=true&theme=tokyonight&count_private=true&hide_border=true" alt="Statistiques de Madiba" class="w-full md:w-[48%] rounded-xl shadow-lg border border-slate-700/50" onerror="this.style.display='none'" />
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=madiba-elate&layout=compact&theme=tokyonight&hide_border=true" alt="Langages les plus utilisés" class="w-full md:w-[48%] rounded-xl shadow-lg border border-slate-700/50" onerror="this.style.display='none'" />
            </div>
        </section>

        <!-- FOOTER / CONTACT -->
        <footer class="pt-12 pb-8 text-center border-t border-slate-800">
            <h2 class="text-2xl font-bold text-white mb-6">🌐 Restons connectés</h2>
            <div class="flex flex-wrap justify-center gap-4">
                <a href="https://omnigroup.great-site.net" target="_blank" class="flex items-center px-6 py-3 bg-slate-800 hover:bg-brand-accent/20 border border-slate-700 hover:border-brand-accent text-white rounded-full transition-all duration-300 shadow-lg">
                    <i data-lucide="globe" class="w-5 h-5 mr-2 text-brand-accent"></i>
                    omnigroup.tech
                </a>
                <a href="https://huggingface.co/madiba-elate" target="_blank" class="flex items-center px-6 py-3 bg-slate-800 hover:bg-yellow-500/20 border border-slate-700 hover:border-yellow-500 text-white rounded-full transition-all duration-300 shadow-lg">
                    <i data-lucide="smile" class="w-5 h-5 mr-2 text-yellow-500"></i>
                    Hugging Face
                </a>
                <a href="https://www.linkedin.com/in/madiba-elate" target="_blank" class="flex items-center px-6 py-3 bg-slate-800 hover:bg-blue-500/20 border border-slate-700 hover:border-blue-500 text-white rounded-full transition-all duration-300 shadow-lg">
                    <i data-lucide="linkedin" class="w-5 h-5 mr-2 text-blue-500"></i>
                    LinkedIn
                </a>
            </div>
            <p class="mt-12 text-sm text-slate-600 font-mono">
                © 2026 OmniGroup / Albert Emmanuel Madiba Elate. All rights reserved.
            </p>
        </footer>

    </div>

    <!-- Initialisation des icônes -->
    <script>
        lucide.createIcons();
    </script>

    <!-- Animation Canvas (Particules style Neural Network / Topologie) -->
    <script>
        const canvas = document.getElementById('bg-canvas');
        const ctx = canvas.getContext('2d');
        
        let width, height;
        let particles = [];
        
        function resize() {
            width = canvas.width = window.innerWidth;
            height = canvas.height = window.innerHeight;
        }
        
        window.addEventListener('resize', resize);
        resize();

        class Particle {
            constructor() {
                this.x = Math.random() * width;
                this.y = Math.random() * height;
                this.vx = (Math.random() - 0.5) * 0.5;
                this.vy = (Math.random() - 0.5) * 0.5;
                this.radius = Math.random() * 2;
            }
            
            update() {
                this.x += this.vx;
                this.y += this.vy;
                
                if (this.x < 0 || this.x > width) this.vx = -this.vx;
                if (this.y < 0 || this.y > height) this.vy = -this.vy;
            }
            
            draw() {
                ctx.beginPath();
                ctx.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
                ctx.fillStyle = '#38bdf8'; // Couleur cyan
                ctx.fill();
            }
        }

        // Créer les particules
        for (let i = 0; i < 80; i++) {
            particles.push(new Particle());
        }

        function animate() {
            ctx.clearRect(0, 0, width, height);
            
            for (let i = 0; i < particles.length; i++) {
                particles[i].update();
                particles[i].draw();
                
                // Dessiner les lignes entre les particules proches
                for (let j = i + 1; j < particles.length; j++) {
                    const dx = particles[i].x - particles[j].x;
                    const dy = particles[i].y - particles[j].y;
                    const distance = Math.sqrt(dx * dx + dy * dy);
                    
                    if (distance < 120) {
                        ctx.beginPath();
                        ctx.moveTo(particles[i].x, particles[i].y);
                        ctx.lineTo(particles[j].x, particles[j].y);
                        ctx.strokeStyle = `rgba(56, 189, 248, ${0.2 - distance/600})`;
                        ctx.stroke();
                    }
                }
            }
            
            requestAnimationFrame(animate);
        }
        
        animate();
    </script>
</body>
</html>
