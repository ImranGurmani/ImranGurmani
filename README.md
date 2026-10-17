<!DOCTYPE html>
<html lang="en" class="dark">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Imran Khan Gurmani | GitHub Profile & Brand Readme</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
  <!-- FontAwesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            obsidian: {
              950: '#050508',
              900: '#08080c',
              850: '#0d0e15',
              800: '#12131d',
              700: '#1b1c2a',
              border: '#27273a',
              borderGlow: 'rgba(250, 204, 21, 0.25)'
            },
            gold: {
              300: '#FFE249',
              400: '#FACC15',
              500: '#EAB308',
              600: '#CA8A04',
              glow: 'rgba(250, 204, 21, 0.15)'
            }
          },
          fontFamily: {
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
            mono: ['"JetBrains Mono"', 'monospace']
          },
          animation: {
            'glow-pulse': 'glowPulse 3s infinite alternate',
            'float-slow': 'float 5s ease-in-out infinite',
            'border-run': 'borderMove 4s linear infinite',
            'snake-pulse': 'snakeGlow 1.5s ease-in-out infinite'
          },
          keyframes: {
            glowPulse: {
              '0%': { boxShadow: '0 0 15px rgba(250, 204, 21, 0.15)' },
              '100%': { boxShadow: '0 0 35px rgba(250, 204, 21, 0.35)' }
            },
            float: {
              '0%, 100%': { transform: 'translateY(0px)' },
              '50%': { transform: 'translateY(-8px)' }
            },
            snakeGlow: {
              '0%, 100%': { filter: 'drop-shadow(0 0 4px #FACC15)' },
              '50%': { filter: 'drop-shadow(0 0 10px #FFE249)' }
            }
          }
        }
      }
    }
  </script>

  <style>
    /* Custom sleek scrollbar */
    ::-webkit-scrollbar {
      width: 7px;
      height: 7px;
    }
    ::-webkit-scrollbar-track {
      background: #08080c;
    }
    ::-webkit-scrollbar-thumb {
      background: #27273a;
      border-radius: 4px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: #FACC15;
    }

    /* Gradient Border utility */
    .neon-card {
      background: linear-gradient(180deg, rgba(18, 19, 29, 0.85) 0%, rgba(13, 14, 21, 0.95) 100%);
      border: 1px solid #27273a;
      transition: all 0.35s cubic-bezier(0.2, 0.8, 0.2, 1);
    }
    .neon-card:hover {
      border-color: rgba(250, 204, 21, 0.5);
      box-shadow: 0 12px 30px -8px rgba(250, 204, 21, 0.18);
      transform: translateY(-3px);
    }

    /* Gold gradient text */
    .text-gold-gradient {
      background: linear-gradient(135deg, #FFF08A 0%, #FACC15 50%, #CA8A04 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .badge-cyber {
      background: rgba(250, 204, 21, 0.06);
      border: 1px solid rgba(250, 204, 21, 0.22);
      color: #FACC15;
    }
    .badge-cyber:hover {
      background: rgba(250, 204, 21, 0.15);
      border-color: #FACC15;
      box-shadow: 0 0 14px rgba(250, 204, 21, 0.3);
    }

    /* Blinking Terminal Cursor */
    .cursor-blink {
      animation: blink 1s step-end infinite;
    }
    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }
  </style>
</head>

<body class="bg-obsidian-950 text-zinc-300 font-sans antialiased min-h-screen relative overflow-x-hidden selection:bg-gold-400 selection:text-black">

  <!-- Interactive Constellation Canvas Background -->
  <canvas id="particleCanvas" class="fixed inset-0 pointer-events-none z-0 opacity-70"></canvas>

  <!-- Ambient Golden Blurs -->
  <div class="fixed -top-40 -left-40 w-96 h-96 bg-gold-400/10 rounded-full blur-[140px] pointer-events-none z-0"></div>
  <div class="fixed top-1/2 -right-40 w-[450px] h-[450px] bg-amber-500/10 rounded-full blur-[160px] pointer-events-none z-0"></div>
  <div class="fixed -bottom-40 left-1/3 w-96 h-96 bg-yellow-300/5 rounded-full blur-[150px] pointer-events-none z-0"></div>

  <!-- Main Wrapper -->
  <div class="relative z-10 flex flex-col min-h-screen">

    <!-- Top Floating Cyber Navigation -->
    <header class="sticky top-4 z-40 max-w-6xl w-[94%] mx-auto backdrop-blur-xl bg-obsidian-900/80 border border-obsidian-border rounded-2xl px-5 py-3.5 shadow-2xl flex items-center justify-between">
      <div class="flex items-center space-x-3.5">
        <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-gold-400 to-amber-600 p-[1.5px] flex items-center justify-center shadow-lg shadow-gold-500/20">
          <div class="w-full h-full bg-obsidian-900 rounded-[10px] flex items-center justify-center font-mono font-black text-gold-400 text-sm">
            JG
          </div>
        </div>
        <div>
          <div class="flex items-center gap-2">
            <span class="text-white font-extrabold tracking-tight text-sm md:text-base">Imran Khan Gurmani</span>
            <span class="text-[10px] bg-gold-400/15 text-gold-400 border border-gold-400/30 px-2 py-0.5 rounded-full font-mono font-semibold">imrangurmani.shop</span>
          </div>
          <p class="text-[11px] text-zinc-400 font-mono hidden sm:block">github.com/imrangurmani (Jigar Gurmani)</p>
        </div>
      </div>

      <!-- Action Buttons -->
      <div class="flex items-center space-x-3">
        <button onclick="openReadmeModal()" class="group relative px-4 py-2 rounded-xl text-xs font-bold text-black bg-gradient-to-r from-gold-300 via-gold-400 to-amber-500 hover:brightness-110 transition-all shadow-lg shadow-gold-500/25 flex items-center gap-2">
          <i class="fa-solid fa-code text-xs"></i>
          <span>Get GitHub Readme</span>
          <i class="fa-solid fa-arrow-right text-[10px] group-hover:translate-x-1 transition-transform"></i>
        </button>
      </div>
    </header>

    <!-- Main Content Grid Container -->
    <main class="max-w-6xl w-[94%] mx-auto py-8 space-y-10">

      <!-- ================= 1. HERO SECTION & LIVE TYPING ================= -->
      <section class="neon-card rounded-3xl p-6 sm:p-10 relative overflow-hidden border border-obsidian-border">
        <!-- Neon Accent Top Bar -->
        <div class="absolute top-0 left-0 right-0 h-[2px] bg-gradient-to-r from-transparent via-gold-400 to-transparent"></div>

        <div class="flex flex-col lg:flex-row items-center justify-between gap-8">
          
          <!-- Left Text Block -->
          <div class="flex-1 space-y-5 text-center lg:text-left">
            <!-- Collab Pill -->
            <div class="inline-flex items-center gap-2.5 px-3.5 py-1.5 rounded-full bg-obsidian-800 border border-obsidian-border text-xs font-mono">
              <span class="relative flex h-2.5 w-2.5">
                <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
                <span class="relative inline-flex rounded-full h-2.5 w-2.5 bg-emerald-500"></span>
              </span>
              <span class="text-zinc-200 font-medium">Open to Collab & SaaS Ventures</span>
              <span class="text-zinc-500">|</span>
              <span class="text-gold-400 font-semibold"><i class="fa-solid fa-location-dot mr-1"></i>Kot Addu, Pakistan</span>
            </div>

            <!-- Main Heading with Luxury Gold Gradient -->
            <h1 class="text-3xl sm:text-4xl md:text-5xl lg:text-6xl font-black tracking-tight text-white leading-tight">
              Crafting Scalable Code & <br class="hidden sm:block">
              <span class="text-gold-gradient">Intelligent Digital Systems.</span>
            </h1>

            <!-- Animated Typewriter Display -->
            <div class="bg-obsidian-900/90 border border-obsidian-border rounded-xl p-3.5 max-w-xl font-mono text-sm flex items-center gap-2 text-zinc-300">
              <span class="text-gold-400 font-bold">$</span>
              <span class="text-zinc-500">run dev --role</span>
              <span id="typewriter" class="text-white font-semibold"></span>
              <span class="text-gold-400 font-bold cursor-blink">▋</span>
            </div>

            <!-- Description matching imrangurmani.shop -->
            <p class="text-zinc-400 text-sm md:text-base leading-relaxed max-w-2xl">
              I am <strong class="text-white">Imran Khan Gurmani</strong>, also recognized as <span class="text-gold-400 font-semibold">Jigar Gurmani</span>. A Full-Stack Web Developer and Digital Entrepreneur engineering mission-critical SaaS, automated high-throughput APIs, voice synthesis systems, and ed-tech platforms.
            </p>

            <!-- Social Action Badges -->
            <div class="flex flex-wrap items-center justify-center lg:justify-start gap-3 pt-2">
              <a href="https://imrangurmani.shop" target="_blank" class="px-4 py-2 rounded-xl bg-obsidian-800 hover:bg-obsidian-700 border border-obsidian-border text-xs font-mono text-zinc-200 flex items-center gap-2 transition hover:border-gold-400/40">
                <i class="fa-solid fa-globe text-gold-400"></i> imrangurmani.shop
              </a>
              <a href="mailto:contact@imrangurmani.shop" class="px-4 py-2 rounded-xl bg-obsidian-800 hover:bg-obsidian-700 border border-obsidian-border text-xs font-mono text-zinc-200 flex items-center gap-2 transition hover:border-gold-400/40">
                <i class="fa-solid fa-envelope text-gold-400"></i> Direct Inquiry
              </a>
              <a href="https://github.com" target="_blank" class="px-4 py-2 rounded-xl bg-obsidian-800 hover:bg-obsidian-700 border border-obsidian-border text-xs font-mono text-zinc-200 flex items-center gap-2 transition hover:border-gold-400/40">
                <i class="fa-brands fa-github text-gold-400"></i> GitHub Profile
              </a>
            </div>
          </div>

          <!-- Right: Glowing Cyber Avatar Card -->
          <div class="flex-shrink-0 relative group">
            <div class="absolute -inset-1 bg-gradient-to-r from-gold-400 via-amber-500 to-yellow-300 rounded-3xl blur-xl opacity-30 group-hover:opacity-75 transition duration-1000 group-hover:duration-200 animate-glow-pulse"></div>
            
            <div class="relative w-72 sm:w-80 bg-obsidian-900 border border-obsidian-border rounded-3xl p-6 text-center space-y-4 shadow-2xl">
              <div class="relative mx-auto w-28 h-28 rounded-2xl bg-gradient-to-tr from-gold-400 to-amber-600 p-1">
                <div class="w-full h-full bg-obsidian-950 rounded-[14px] flex flex-col items-center justify-center overflow-hidden relative">
                  <i class="fa-solid fa-terminal text-4xl text-gold-400/80 mb-1"></i>
                  <span class="text-xs font-mono font-bold tracking-widest text-zinc-400">JIGAR</span>
                  <div class="absolute bottom-0 inset-x-0 h-1 bg-gradient-to-r from-gold-400 to-amber-500"></div>
                </div>
                <div class="absolute -bottom-2 -right-2 bg-obsidian-900 border border-gold-400/50 text-gold-400 text-[10px] font-mono px-2 py-0.5 rounded-full shadow-lg">
                  LVL. 99
                </div>
              </div>

              <div>
                <h3 class="text-lg font-bold text-white">Imran Khan Gurmani</h3>
                <p class="text-xs text-gold-400 font-mono mt-0.5">@imrangurmani</p>
                <div class="mt-2 text-xs text-zinc-400">
                  <span>Kot Addu, Punjab, PK</span> 🇵🇰
                </div>
              </div>

              <!-- Quick spec indicators -->
              <div class="pt-3 border-t border-obsidian-border/80 grid grid-cols-2 gap-2 text-left font-mono text-[11px]">
                <div class="bg-obsidian-850 p-2 rounded-lg border border-obsidian-border">
                  <span class="text-zinc-500 block text-[9px] uppercase">Experience</span>
                  <span class="text-white font-bold">5+ Years</span>
                </div>
                <div class="bg-obsidian-850 p-2 rounded-lg border border-obsidian-border">
                  <span class="text-zinc-500 block text-[9px] uppercase">Architecture</span>
                  <span class="text-gold-400 font-bold">Full-Stack</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- ================= 2. ANIMATED STATS COUNTERS ================= -->
      <section class="grid grid-cols-2 md:grid-cols-4 gap-4">
        <!-- Stat 1 -->
        <div class="neon-card rounded-2xl p-5 text-center relative overflow-hidden">
          <div class="text-2xl sm:text-3xl lg:text-4xl font-extrabold text-gold-gradient font-mono counter" data-target="50">0</div>
          <span class="text-xs sm:text-sm font-semibold text-white block mt-1">Projects Completed</span>
          <span class="text-[11px] text-zinc-500 font-mono mt-0.5 block">SaaS, APIs & Portals</span>
        </div>
        <!-- Stat 2 -->
        <div class="neon-card rounded-2xl p-5 text-center relative overflow-hidden">
          <div class="text-2xl sm:text-3xl lg:text-4xl font-extrabold text-white font-mono counter" data-target="30">0</div>
          <span class="text-xs sm:text-sm font-semibold text-gold-400 block mt-1">Happy Global Clients</span>
          <span class="text-[11px] text-zinc-500 font-mono mt-0.5 block">100% Satisfaction Rate</span>
        </div>
        <!-- Stat 3 -->
        <div class="neon-card rounded-2xl p-5 text-center relative overflow-hidden">
          <div class="text-2xl sm:text-3xl lg:text-4xl font-extrabold text-gold-gradient font-mono">99.9%</div>
          <span class="text-xs sm:text-sm font-semibold text-white block mt-1">SaaS System Uptime</span>
          <span class="text-[11px] text-zinc-500 font-mono mt-0.5 block">High-Throughput Engines</span>
        </div>
        <!-- Stat 4 -->
        <div class="neon-card rounded-2xl p-5 text-center relative overflow-hidden">
          <div class="text-2xl sm:text-3xl lg:text-4xl font-extrabold text-white font-mono counter" data-target="100">0</div>
          <span class="text-xs sm:text-sm font-semibold text-gold-400 block mt-1">LMS Students Trained</span>
          <span class="text-[11px] text-zinc-500 font-mono mt-0.5 block">GenXEmpire Academy</span>
        </div>
      </section>

      <!-- ================= 3. ANIMATED GITHUB SNAKE SIMULATION & CONTRIBUTION MATRIX ================= -->
      <section class="neon-card rounded-3xl p-6 sm:p-8 space-y-6">
        <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4 border-b border-obsidian-border pb-4">
          <div>
            <div class="flex items-center gap-2">
              <i class="fa-solid fa-gamepad text-gold-400 text-lg"></i>
              <h2 class="text-lg sm:text-xl font-bold text-white tracking-tight">Interactive GitHub Contribution Matrix & Cyber Snake</h2>
            </div>
            <p class="text-xs text-zinc-400 font-mono mt-1">Simulating real GitHub contributions in brand yellow-gold palette</p>
          </div>
          <div class="flex items-center space-x-2 text-xs font-mono bg-obsidian-900 border border-obsidian-border px-3 py-1.5 rounded-xl">
            <span class="text-zinc-500">Score:</span>
            <span id="snakeScore" class="text-gold-400 font-bold">1,842</span>
            <span class="text-zinc-600">|</span>
            <button onclick="resetSnakeGame()" class="text-zinc-400 hover:text-white transition flex items-center gap-1">
              <i class="fa-solid fa-rotate-right text-[10px]"></i> Restart
            </button>
          </div>
        </div>

        <!-- Snake Simulation Container -->
        <div class="relative bg-obsidian-950 border border-obsidian-border rounded-2xl p-4 overflow-hidden">
          <!-- Canvas for Snake Board -->
          <canvas id="snakeCanvas" class="w-full h-36 rounded-lg block"></canvas>

          <!-- Status overlay -->
          <div class="mt-3 flex flex-wrap items-center justify-between text-[11px] font-mono text-zinc-400 gap-2">
            <div class="flex items-center gap-2">
              <span>Less</span>
              <span class="w-2.5 h-2.5 rounded-sm bg-[#161b22]"></span>
              <span class="w-2.5 h-2.5 rounded-sm bg-[#3a3512]"></span>
              <span class="w-2.5 h-2.5 rounded-sm bg-[#786616]"></span>
              <span class="w-2.5 h-2.5 rounded-sm bg-[#ca9f10]"></span>
              <span class="w-2.5 h-2.5 rounded-sm bg-[#facc15] shadow-sm shadow-gold-400/50"></span>
              <span>More Active</span>
            </div>
            <div class="flex items-center gap-2">
              <span class="text-gold-400 font-semibold">● Yellow Snake Eating Commits</span>
            </div>
          </div>
        </div>

        <!-- Live Telemetry Badges -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
          <!-- Card A -->
          <div class="bg-obsidian-900/70 border border-obsidian-border rounded-xl p-4 flex items-center justify-between">
            <div>
              <p class="text-[11px] font-mono text-zinc-500 uppercase">Longest Streak</p>
              <h4 class="text-xl font-bold text-white mt-0.5">289 Days</h4>
              <p class="text-[10px] text-emerald-400 font-mono mt-1"><i class="fa-solid fa-arrow-trend-up mr-1"></i>Consistent daily pusher</p>
            </div>
            <div class="w-10 h-10 rounded-xl bg-gold-400/10 border border-gold-400/30 flex items-center justify-center text-gold-400">
              <i class="fa-solid fa-fire text-lg"></i>
            </div>
          </div>
          <!-- Card B -->
          <div class="bg-obsidian-900/70 border border-obsidian-border rounded-xl p-4 flex items-center justify-between">
            <div>
              <p class="text-[11px] font-mono text-zinc-500 uppercase">Total Commits (2025-2026)</p>
              <h4 class="text-xl font-bold text-gold-gradient mt-0.5">3,120+</h4>
              <p class="text-[10px] text-zinc-400 font-mono mt-1">SaaS & Open-Source Repos</p>
            </div>
            <div class="w-10 h-10 rounded-xl bg-amber-500/10 border border-amber-500/30 flex items-center justify-center text-amber-400">
              <i class="fa-solid fa-code-commit text-lg"></i>
            </div>
          </div>
          <!-- Card C -->
          <div class="bg-obsidian-900/70 border border-obsidian-border rounded-xl p-4 flex items-center justify-between">
            <div>
              <p class="text-[11px] font-mono text-zinc-500 uppercase">Production Status</p>
              <h4 class="text-xl font-bold text-white mt-0.5">5 Key Ventures</h4>
              <p class="text-[10px] text-gold-400 font-mono mt-1">Live in Market</p>
            </div>
            <div class="w-10 h-10 rounded-xl bg-gold-300/10 border border-gold-300/30 flex items-center justify-center text-gold-300">
              <i class="fa-solid fa-network-wired text-lg"></i>
            </div>
          </div>
        </div>
      </section>

      <!-- ================= 4. SHOWCASE GRID OF FLAGSHIP VENTURES ================= -->
      <section class="space-y-6">
        <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-2 border-b border-obsidian-border pb-4">
          <div>
            <div class="flex items-center gap-2">
              <i class="fa-solid fa-cubes-stacked text-gold-400 text-lg"></i>
              <h2 class="text-2xl font-bold text-white tracking-tight">Flagship Ventures & Systems</h2>
            </div>
            <p class="text-xs text-zinc-400 font-mono mt-1">Real platforms conceptualized, engineered, and operated by Imran Khan Gurmani</p>
          </div>
          <span class="text-xs font-mono text-gold-400 bg-gold-400/10 border border-gold-400/20 px-3 py-1 rounded-full">
            Production Grade
          </span>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5">

          <!-- 1. SynVoice.io -->
          <div class="neon-card rounded-2xl p-6 flex flex-col justify-between group">
            <div class="space-y-3">
              <div class="flex items-center justify-between">
                <div class="w-10 h-10 rounded-xl bg-purple-500/10 border border-purple-500/30 flex items-center justify-center text-purple-400">
                  <i class="fa-solid fa-microphone-lines text-lg"></i>
                </div>
                <span class="text-[10px] font-mono bg-purple-950/60 text-purple-300 border border-purple-800 px-2 py-0.5 rounded-full">AI Audio SaaS</span>
              </div>
              <h3 class="text-xl font-bold text-white group-hover:text-gold-400 transition-colors flex items-center gap-2">
                SynVoice.io <i class="fa-solid fa-arrow-up-right-from-square text-xs opacity-60"></i>
              </h3>
              <p class="text-xs text-zinc-400 leading-relaxed">
                Next-Gen AI Voice Cloning & Speech Synthesis Platform. Multi-engine voice studio with XTTS-v2 & StyleTTS 2, custom voice training, automated credit subscriptions, and lightning-fast audio generation.
              </p>
            </div>
            <div class="mt-5 pt-4 border-t border-obsidian-border/70 space-y-3">
              <div class="flex flex-wrap gap-1.5 font-mono text-[10px]">
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Python</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">XTTS-v2</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Astro JS</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Tailwind</span>
              </div>
              <div class="flex items-center justify-between text-xs text-zinc-400 font-mono">
                <span>Status: <span class="text-emerald-400">Live Studio</span></span>
                <span class="text-gold-400 font-semibold">Tier 1 Voice Model</span>
              </div>
            </div>
          </div>

          <!-- 2. GeoSMM.pk -->
          <div class="neon-card rounded-2xl p-6 flex flex-col justify-between group">
            <div class="space-y-3">
              <div class="flex items-center justify-between">
                <div class="w-10 h-10 rounded-xl bg-blue-500/10 border border-blue-500/30 flex items-center justify-center text-blue-400">
                  <i class="fa-solid fa-bolt text-lg"></i>
                </div>
                <span class="text-[10px] font-mono bg-blue-950/60 text-blue-300 border border-blue-800 px-2 py-0.5 rounded-full">High-Load API</span>
              </div>
              <h3 class="text-xl font-bold text-white group-hover:text-gold-400 transition-colors flex items-center gap-2">
                GeoSMM.pk <i class="fa-solid fa-arrow-up-right-from-square text-xs opacity-60"></i>
              </h3>
              <p class="text-xs text-zinc-400 leading-relaxed">
                Automated High-Scale Social Media Marketing Services Panel & API Gateway. Handles millions of background API transactions, failover balancing, automated payment webhooks, and real-time order completion tracking.
              </p>
            </div>
            <div class="mt-5 pt-4 border-t border-obsidian-border/70 space-y-3">
              <div class="flex flex-wrap gap-1.5 font-mono text-[10px]">
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">PHP 8.2</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">MySQL High-Perf</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">REST Webhooks</span>
              </div>
              <div class="flex items-center justify-between text-xs text-zinc-400 font-mono">
                <span>Scale: <span class="text-gold-400">500k+ API calls/mo</span></span>
                <span class="text-emerald-400">99.9% Uptime</span>
              </div>
            </div>
          </div>

          <!-- 3. GenXEmpire.com -->
          <div class="neon-card rounded-2xl p-6 flex flex-col justify-between group">
            <div class="space-y-3">
              <div class="flex items-center justify-between">
                <div class="w-10 h-10 rounded-xl bg-emerald-500/10 border border-emerald-500/30 flex items-center justify-center text-emerald-400">
                  <i class="fa-solid fa-graduation-cap text-lg"></i>
                </div>
                <span class="text-[10px] font-mono bg-emerald-950/60 text-emerald-300 border border-emerald-800 px-2 py-0.5 rounded-full">EdTech & Academy</span>
              </div>
              <h3 class="text-xl font-bold text-white group-hover:text-gold-400 transition-colors flex items-center gap-2">
                GenXEmpire.com <i class="fa-solid fa-arrow-up-right-from-square text-xs opacity-60"></i>
              </h3>
              <p class="text-xs text-zinc-400 leading-relaxed">
                AI Automation Academy & LMS platform mentoring students in modern software engineering, AI tooling, and monetizable freelance skills with automated enrollment and payment verify gates.
              </p>
            </div>
            <div class="mt-5 pt-4 border-t border-obsidian-border/70 space-y-3">
              <div class="flex flex-wrap gap-1.5 font-mono text-[10px]">
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">LMS System</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Astro JS</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Tailwind</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Member Vault</span>
              </div>
              <div class="flex items-center justify-between text-xs text-zinc-400 font-mono">
                <span>Community: <span class="text-emerald-400 font-bold">100+ Active</span></span>
                <span class="text-zinc-400">Course Engine</span>
              </div>
            </div>
          </div>

          <!-- 4. MicroSmartLoan.in -->
          <div class="neon-card rounded-2xl p-6 flex flex-col justify-between group">
            <div class="space-y-3">
              <div class="flex items-center justify-between">
                <div class="w-10 h-10 rounded-xl bg-amber-500/10 border border-amber-500/30 flex items-center justify-center text-amber-400">
                  <i class="fa-solid fa-hand-holding-dollar text-lg"></i>
                </div>
                <span class="text-[10px] font-mono bg-amber-950/60 text-amber-300 border border-amber-800 px-2 py-0.5 rounded-full">FinTech CRM</span>
              </div>
              <h3 class="text-xl font-bold text-white group-hover:text-gold-400 transition-colors flex items-center gap-2">
                MicroSmartLoan.in <i class="fa-solid fa-arrow-up-right-from-square text-xs opacity-60"></i>
              </h3>
              <p class="text-xs text-zinc-400 leading-relaxed">
                Complete Loan Management CRM and micro-finance administration dashboard. Features dynamic eligibility calculation, automated installment schedules, KYC uploads, and disbursement auditing.
              </p>
            </div>
            <div class="mt-5 pt-4 border-t border-obsidian-border/70 space-y-3">
              <div class="flex flex-wrap gap-1.5 font-mono text-[10px]">
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">PHP & MySQL</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Financial Math</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Secure Auth</span>
              </div>
              <div class="flex items-center justify-between text-xs text-zinc-400 font-mono">
                <span>Security: <span class="text-amber-400 font-bold">Role-Based RBAC</span></span>
                <span class="text-zinc-400">Live Client CRM</span>
              </div>
            </div>
          </div>

          <!-- 5. RenZoify Agency -->
          <div class="neon-card rounded-2xl p-6 flex flex-col justify-between group md:col-span-2 lg:col-span-2">
            <div class="space-y-3">
              <div class="flex items-center justify-between">
                <div class="w-10 h-10 rounded-xl bg-gold-400/10 border border-gold-400/30 flex items-center justify-center text-gold-400">
                  <i class="fa-solid fa-laptop-code text-lg"></i>
                </div>
                <span class="text-[10px] font-mono bg-gold-950/60 text-gold-300 border border-gold-800 px-2 py-0.5 rounded-full">Bespoke Tech Agency</span>
              </div>
              <h3 class="text-xl font-bold text-white group-hover:text-gold-400 transition-colors flex items-center gap-2">
                RenZoify <i class="fa-solid fa-arrow-up-right-from-square text-xs opacity-60"></i>
              </h3>
              <p class="text-xs text-zinc-400 leading-relaxed">
                A modern digital agency crafting bespoke software solutions, customized web portals, conversion-focused user interfaces, and automated business infrastructure for global brands and local leaders.
              </p>
            </div>
            <div class="mt-5 pt-4 border-t border-obsidian-border/70 space-y-3">
              <div class="flex flex-wrap gap-1.5 font-mono text-[10px]">
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Full-Stack Solutions</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Performance Tuning</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">Custom CMS</span>
                <span class="px-2 py-0.5 rounded bg-obsidian-800 text-zinc-300 border border-obsidian-border">SEO Infrastructure</span>
              </div>
              <div class="flex items-center justify-between text-xs text-zinc-400 font-mono">
                <span>Portfolio: <span class="text-gold-400 font-bold">30+ Delivered Projects</span></span>
                <span class="text-emerald-400">100% Client Endorsement</span>
              </div>
            </div>
          </div>

        </div>
      </section>

      <!-- ================= 5. INTERACTIVE TECH ARSENAL ================= -->
      <section class="neon-card rounded-3xl p-6 sm:p-8 space-y-6">
        <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-2 border-b border-obsidian-border pb-4">
          <div>
            <div class="flex items-center gap-2">
              <i class="fa-solid fa-microchip text-gold-400 text-lg"></i>
              <h2 class="text-xl font-bold text-white tracking-tight">Engineering Arsenal & Modern Stack</h2>
            </div>
            <p class="text-xs text-zinc-400 font-mono mt-1">Tools and frameworks powering Imran's daily workflows</p>
          </div>
          <span class="text-xs font-mono text-zinc-500">production_ready_stack.json</span>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-5">
          <!-- Column 1: Core Backend & Data -->
          <div class="bg-obsidian-900/60 border border-obsidian-border rounded-2xl p-5 space-y-3">
            <h4 class="text-xs font-mono font-bold uppercase tracking-wider text-gold-400 flex items-center gap-2">
              <i class="fa-solid fa-server"></i> Backend & Data
            </h4>
            <div class="flex flex-wrap gap-2 pt-1">
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-brands fa-php text-sm"></i> PHP 8.x</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-database text-xs"></i> MySQL / MariaDB</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-brands fa-node-js text-sm"></i> Node.js</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-bolt text-xs"></i> RESTful APIs</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-fire text-xs"></i> Supabase</span>
            </div>
          </div>

          <!-- Column 2: Frontend & Styling -->
          <div class="bg-obsidian-900/60 border border-obsidian-border rounded-2xl p-5 space-y-3">
            <h4 class="text-xs font-mono font-bold uppercase tracking-wider text-amber-400 flex items-center gap-2">
              <i class="fa-solid fa-code"></i> Frontend & UI Systems
            </h4>
            <div class="flex flex-wrap gap-2 pt-1">
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-rocket text-xs"></i> Astro JS</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-wind text-xs"></i> Tailwind CSS</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-brands fa-js text-sm"></i> JavaScript (ESNext)</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-brands fa-html5 text-sm"></i> Semantic HTML5</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-mobile-screen text-xs"></i> Responsive UI</span>
            </div>
          </div>

          <!-- Column 3: AI, Agents & Cloud -->
          <div class="bg-obsidian-900/60 border border-obsidian-border rounded-2xl p-5 space-y-3">
            <h4 class="text-xs font-mono font-bold uppercase tracking-wider text-yellow-300 flex items-center gap-2">
              <i class="fa-solid fa-brain"></i> AI, Speech & Tooling
            </h4>
            <div class="flex flex-wrap gap-2 pt-1">
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-waveform-lines text-xs"></i> StyleTTS 2 / XTTS-v2</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-robot text-xs"></i> Cursor AI / Roo Code</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-network-wired text-xs"></i> Gemini & LLM APIs</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-solid fa-cloud text-xs"></i> Cloudflare</span>
              <span class="badge-cyber px-3 py-1.5 rounded-lg text-xs font-mono flex items-center gap-2"><i class="fa-brands fa-git-alt text-sm"></i> Git & Bash</span>
            </div>
          </div>
        </div>
      </section>

      <!-- ================= 6. BOTTOM CALL TO ACTION & MODAL TRIGGER ================= -->
      <section class="neon-card rounded-3xl p-8 sm:p-10 text-center relative overflow-hidden space-y-5">
        <div class="inline-block p-3 rounded-2xl bg-gold-400/10 border border-gold-400/30 text-gold-400 mb-2">
          <i class="fa-brands fa-github text-3xl"></i>
        </div>
        <h2 class="text-2xl sm:text-3xl font-black text-white">
          Ready to Upgrade Your GitHub Profile with this Style?
        </h2>
        <p class="text-zinc-400 text-sm max-w-xl mx-auto leading-relaxed">
          Grab the complete, professionally formulated Markdown code with custom shields, matching gold theme stats cards, and project tables ready to paste into your GitHub special repo (<code class="text-gold-400 font-mono">imrangurmani/imrangurmani</code>).
        </p>

        <div class="pt-3 flex flex-wrap items-center justify-center gap-4">
          <button onclick="openReadmeModal()" class="px-6 py-3 rounded-xl font-bold text-black bg-gradient-to-r from-gold-300 via-gold-400 to-amber-500 hover:brightness-110 shadow-lg shadow-gold-500/20 text-sm flex items-center gap-2 transition-all">
            <i class="fa-regular fa-copy text-sm"></i>
            <span>Copy Complete README.md</span>
          </button>
          <a href="https://imrangurmani.shop" target="_blank" class="px-6 py-3 rounded-xl font-mono text-zinc-300 bg-obsidian-850 hover:bg-obsidian-800 border border-obsidian-border text-sm flex items-center gap-2 transition-all">
            <i class="fa-solid fa-arrow-up-right-from-square text-xs text-gold-400"></i>
            <span>Visit imrangurmani.shop</span>
          </a>
        </div>
      </section>

      <!-- Footer Quote -->
      <footer class="text-center py-6 text-zinc-500 font-mono text-xs space-y-1">
        <p class="text-zinc-400">"Architecting resilient systems that power the next wave of web innovation."</p>
        <p>© 2026 Imran Khan Gurmani (Jigar Gurmani). Kot Addu, Pakistan.</p>
      </footer>

    </main>

  </div>

  <!-- ================= README MARKDOWN MODAL ================= -->
  <div id="readmeModal" class="fixed inset-0 z-50 bg-black/85 backdrop-blur-md hidden flex items-center justify-center p-4">
    <div class="bg-obsidian-900 border border-obsidian-border rounded-2xl w-full max-w-4xl max-h-[90vh] flex flex-col shadow-2xl overflow-hidden">
      
      <!-- Modal Header -->
      <div class="px-6 py-4 bg-obsidian-950 border-b border-obsidian-border flex items-center justify-between">
        <div class="flex items-center space-x-3">
          <i class="fa-brands fa-markdown text-gold-400 text-xl"></i>
          <div>
            <h3 class="text-white font-bold text-sm sm:text-base">Custom Gold-Cyber README.md</h3>
            <p class="text-[11px] text-zinc-400 font-mono">Optimized for imrangurmani / imrangurmani</p>
          </div>
        </div>
        <div class="flex items-center space-x-2">
          <button id="modalCopyBtn" onclick="copyMarkdownText()" class="px-4 py-1.5 rounded-lg bg-gold-400 hover:bg-gold-300 text-black font-bold text-xs flex items-center gap-2 transition">
            <i class="fa-solid fa-copy"></i>
            <span id="copyBtnLabel">Copy All Code</span>
          </button>
          <button onclick="closeReadmeModal()" class="w-8 h-8 rounded-lg bg-obsidian-800 hover:bg-obsidian-700 text-zinc-400 hover:text-white flex items-center justify-center transition">
            <i class="fa-solid fa-xmark text-sm"></i>
          </button>
        </div>
      </div>

      <!-- Modal Body -->
      <div class="p-4 sm:p-6 flex-1 overflow-auto bg-[#050508]">
        <textarea id="markdownArea" readonly class="w-full h-96 bg-transparent text-zinc-300 font-mono text-xs focus:outline-none resize-none leading-relaxed selection:bg-gold-400 selection:text-black"></textarea>
      </div>

      <!-- Modal Footer -->
      <div class="px-6 py-3 bg-obsidian-950 border-t border-obsidian-border flex items-center justify-between text-xs text-zinc-400 font-mono">
        <span>💡 Instructions: Go to GitHub → Create repo named <strong class="text-gold-400">imrangurmani</strong> → Paste into README.md</span>
        <button onclick="closeReadmeModal()" class="text-zinc-400 hover:text-white underline">Close</button>
      </div>
    </div>
  </div>

  <!-- Notification Toast -->
  <div id="toast" class="fixed bottom-6 right-6 z-50 transform translate-y-20 opacity-0 transition-all duration-300 pointer-events-none flex items-center gap-2.5 bg-gold-400 text-black px-4 py-3 rounded-xl shadow-2xl font-semibold text-xs border border-gold-300">
    <i class="fa-solid fa-circle-check text-base"></i>
    <span>README.md copied! Ready to paste into GitHub.</span>
  </div>

  <!-- ================= JAVASCRIPT ================= -->
  <script>
    // 1. Constellation Particle Canvas
    const canvas = document.getElementById('particleCanvas');
    const ctx = canvas.getContext('2d');
    let particles = [];
    const particleCount = 45;

    function resizeCanvas() {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    }
    window.addEventListener('resize', resizeCanvas);
    resizeCanvas();

    class Particle {
      constructor() {
        this.x = Math.random() * canvas.width;
        this.y = Math.random() * canvas.height;
        this.vx = (Math.random() - 0.5) * 0.45;
        this.vy = (Math.random() - 0.5) * 0.45;
        this.radius = Math.random() * 1.6 + 0.6;
      }
      update() {
        this.x += this.vx;
        this.y += this.vy;
        if (this.x < 0 || this.x > canvas.width) this.vx *= -1;
        if (this.y < 0 || this.y > canvas.height) this.vy *= -1;
      }
      draw() {
        ctx.beginPath();
        ctx.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
        ctx.fillStyle = '#FACC15';
        ctx.shadowBlur = 8;
        ctx.shadowColor = '#FACC15';
        ctx.fill();
      }
    }

    for (let i = 0; i < particleCount; i++) {
      particles.push(new Particle());
    }

    function animateParticles() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      for (let i = 0; i < particles.length; i++) {
        particles[i].update();
        particles[i].draw();

        // Connect nearest nodes
        for (let j = i + 1; j < particles.length; j++) {
          const dx = particles[i].x - particles[j].x;
          const dy = particles[i].y - particles[j].y;
          const dist = Math.sqrt(dx * dx + dy * dy);
          if (dist < 110) {
            ctx.beginPath();
            ctx.moveTo(particles[i].x, particles[i].y);
            ctx.lineTo(particles[j].x, particles[j].y);
            ctx.strokeStyle = `rgba(250, 204, 21, ${0.15 * (1 - dist / 110)})`;
            ctx.lineWidth = 0.6;
            ctx.stroke();
          }
        }
      }
      requestAnimationFrame(animateParticles);
    }
    animateParticles();

    // 2. Typewriter Effect
    const typewriterPhrases = [
      "Building High-Impact SaaS Platforms",
      "Custom PHP & Full-Stack Architect",
      "AI Automation & Speech Tech Pioneer",
      "Founder of GeoSMM, SynVoice & GenXEmpire",
      "Designing for imrangurmani.shop"
    ];
    let phraseIndex = 0;
    let charIndex = 0;
    let isDeleting = false;
    const typewriterEl = document.getElementById("typewriter");

    function typeLoop() {
      const current = typewriterPhrases[phraseIndex];
      if (isDeleting) {
        typewriterEl.textContent = current.substring(0, charIndex - 1);
        charIndex--;
      } else {
        typewriterEl.textContent = current.substring(0, charIndex + 1);
        charIndex++;
      }

      let speed = isDeleting ? 30 : 70;

      if (!isDeleting && charIndex === current.length) {
        speed = 2200;
        isDeleting = true;
      } else if (isDeleting && charIndex === 0) {
        isDeleting = false;
        phraseIndex = (phraseIndex + 1) % typewriterPhrases.length;
        speed = 500;
      }
      setTimeout(typeLoop, speed);
    }
    typeLoop();

    // 3. Counter Animation on viewport
    const counters = document.querySelectorAll('.counter');
    let hasCounted = false;

    function runCounters() {
      if (hasCounted) return;
      counters.forEach(counter => {
        const target = +counter.getAttribute('data-target');
        let count = 0;
        const step = Math.ceil(target / 40);
        const timer = setInterval(() => {
          count += step;
          if (count >= target) {
            counter.innerText = target + "+";
            clearInterval(timer);
          } else {
            counter.innerText = count;
          }
        }, 35);
      });
      hasCounted = true;
    }
    window.addEventListener('load', runCounters);

    // 4. Interactive GitHub Snake Simulator (Golden Theme)
    const sCanvas = document.getElementById('snakeCanvas');
    const sCtx = sCanvas.getContext('2d');
    let sCols = 48;
    let sRows = 7;
    let cellW = 0;
    let cellH = 0;
    let gridColors = [];
    let snake = [
      {x: 6, y: 3},
      {x: 5, y: 3},
      {x: 4, y: 3},
      {x: 3, y: 3}
    ];
    let dir = {x: 1, y: 0};
    let score = 1842;
    let snakeInterval = null;

    function setupSnakeGrid() {
      const rect = sCanvas.getBoundingClientRect();
      sCanvas.width = rect.width * window.devicePixelRatio;
      sCanvas.height = 144 * window.devicePixelRatio;
      sCtx.scale(window.devicePixelRatio, window.devicePixelRatio);

      cellW = rect.width / sCols;
      cellH = 144 / sRows;

      // Seed contribution intensity palette matching imrangurmani.shop
      const shades = [
        '#12131d', // empty
        '#27273a',
        '#574712',
        '#8f7212',
        '#c99d0e',
        '#facc15'  // peak gold commit
      ];

      gridColors = [];
      for (let c = 0; c < sCols; c++) {
        gridColors[c] = [];
        for (let r = 0; r < sRows; r++) {
          const rand = Math.random();
          let shadeIdx = 0;
          if (rand > 0.88) shadeIdx = 5;
          else if (rand > 0.70) shadeIdx = 4;
          else if (rand > 0.50) shadeIdx = 3;
          else if (rand > 0.30) shadeIdx = 2;
          else if (rand > 0.15) shadeIdx = 1;
          gridColors[c][r] = shades[shadeIdx];
        }
      }
    }

    function drawSnakeGrid() {
      const rect = sCanvas.getBoundingClientRect();
      sCtx.clearRect(0, 0, rect.width, 144);

      // Draw commit tiles
      for (let c = 0; c < sCols; c++) {
        for (let r = 0; r < sRows; r++) {
          sCtx.fillStyle = gridColors[c][r];
          sCtx.beginPath();
          sCtx.roundRect(c * cellW + 1.5, r * cellH + 1.5, cellW - 3, cellH - 3, 2);
          sCtx.fill();
        }
      }

      // Draw Snake Body
      for (let i = 0; i < snake.length; i++) {
        const seg = snake[i];
        if (i === 0) {
          // Head
          sCtx.fillStyle = '#FFE249';
          sCtx.shadowBlur = 12;
          sCtx.shadowColor = '#FACC15';
        } else {
          sCtx.fillStyle = '#FACC15';
          sCtx.shadowBlur = 4;
          sCtx.shadowColor = '#CA8A04';
        }
        sCtx.beginPath();
        sCtx.roundRect(seg.x * cellW + 1.5, seg.y * cellH + 1.5, cellW - 3, cellH - 3, 3);
        sCtx.fill();
      }
      sCtx.shadowBlur = 0;
    }

    function stepSnake() {
      // Pick random next turn towards high-commit tiles
      if (Math.random() < 0.22) {
        const turns = [
          {x: 0, y: -1},
          {x: 0, y: 1},
          {x: 1, y: 0},
          {x: -1, y: 0}
        ];
        const valid = turns.filter(t => !(t.x === -dir.x && t.y === -dir.y));
        dir = valid[Math.floor(Math.random() * valid.length)];
      }

      let newHead = {
        x: (snake[0].x + dir.x + sCols) % sCols,
        y: (snake[0].y + dir.y + sRows) % sRows
      };

      snake.unshift(newHead);
      // "Eats" commits and dims the tile
      gridColors[newHead.x][newHead.y] = '#27273a';
      snake.pop();

      score += 1;
      document.getElementById('snakeScore').innerText = score.toLocaleString();
      drawSnakeGrid();
    }

    function startSnakeGame() {
      setupSnakeGrid();
      drawSnakeGrid();
      if (snakeInterval) clearInterval(snakeInterval);
      snakeInterval = setInterval(stepSnake, 130);
    }

    function resetSnakeGame() {
      snake = [
        {x: 6, y: 3},
        {x: 5, y: 3},
        {x: 4, y: 3},
        {x: 3, y: 3}
      ];
      dir = {x: 1, y: 0};
      startSnakeGame();
    }

    window.addEventListener('resize', () => {
      setupSnakeGrid();
      drawSnakeGrid();
    });
    startSnakeGame();

    // 5. Raw GitHub README Markdown Template
    const customizedReadmeMarkdown = `<!-- ======================================================== -->
<!-- Imran Khan Gurmani (Jigar Gurmani) - GitHub Profile README -->
<!-- Palette: Obsidian Dark (#08080C) + Luxury Neon Gold (#FACC15) -->
<!-- Generated for: https://imrangurmani.shop -->
<!-- ======================================================== -->

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=08080c&height=220&section=header&text=Imran%20Khan%20Gurmani&fontSize=42&fontColor=FACC15&fontAlignY=40&desc=Full-Stack%20Architect%20%7C%20AI%20Ventures%20%7C%20Digital%20Entrepreneur&descColor=A1A1AA&descAlignY=62" width="100%" />
</div>

<p align="center">
  <a href="https://imrangurmani.shop"><img src="https://img.shields.io/badge/Portfolio-imrangurmani.shop-FACC15?style=for-the-badge&logo=google-chrome&logoColor=000&labelColor=08080c" alt="Portfolio" /></a>
  <a href="mailto:contact@imrangurmani.shop"><img src="https://img.shields.io/badge/Email-Get_in_Touch-FFE249?style=for-the-badge&logo=gmail&logoColor=000&labelColor=08080c" alt="Email" /></a>
  <a href="https://github.com/imrangurmani"><img src="https://img.shields.io/badge/Location-Kot%20Addu%2C%20Pakistan-FACC15?style=for-the-badge&logo=location-dot&logoColor=FACC15&labelColor=08080c" alt="Location" /></a>
</p>

<p align="center">
  <strong>"Crafting scalable code, mission-critical SaaS, and next-generation speech tech."</strong><br>
  Known across the developer web as <em>Jigar Gurmani</em>
</p>

---

### ⚡ Operational Telemetry & Metrics

- 🚀 **Projects Completed:** 50+ Production web apps, SaaS panels & APIs.
- 🤝 **Client Success:** 30+ Happy clients worldwide with 100% satisfaction.
- ⚡ **SaaS Uptime:** 99.9% uptime track record across high-volume platforms.
- 🎓 **GenXEmpire:** Trained 100+ students in full-stack engineering & AI workflows.
- 📍 **Base:** Kot Addu, Punjab, Pakistan.

---

### 🛸 Flagship Ventures & Ecosystem

| Platform | Core Domain | Technology Stack |
| :--- | :--- | :--- |
| **[SynVoice.io](https://synvoice.io)** | AI Voice Cloning & Speech Synthesis Platform | Python, XTTS-v2, StyleTTS 2, Astro JS, Tailwind |
| **[GeoSMM.pk](https://geosmm.pk)** | High-Traffic SMM Automation & Reseller API Gateway | PHP 8.2, MySQL High-Perf, Webhooks, Cron Queues |
| **[GenXEmpire.com](https://genxempire.com)** | AI Automation Academy & LMS Community | Astro JS, Tailwind CSS, Member Gating, Payments |
| **[MicroSmartLoan.in](https://microsmartloan.in)** | Complete Loan Management CRM & Installment Tracker | PHP, MySQL, Financial Math Engine, RBAC |
| **[RenZoify](https://renzoify.com)** | Bespoke Software Development & Web Agency | Full-Stack Modern Web, Custom CMS, UI/UX |

---

### 🛠️ Tech Arsenal & Stack

\`\`\`yaml
Languages:     PHP (8.x), JavaScript (ES6+), Python, SQL, HTML5/CSS3
Frameworks:    Astro JS, Node.js, Express, Tailwind CSS
Databases:     MySQL, MariaDB, Supabase, Redis
AI / Speech:   XTTS-v2, StyleTTS 2, Gemini API, ChatGPT / OpenAI APIs
Tooling:       Cursor AI, Roo Code, VS Code, Git/GitHub, Cloudflare, Linux Bash
\`\`\`

---

### 📊 GitHub Activity & Golden Telemetry

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=imrangurmani&show_icons=true&title_color=FACC15&text_color=D4D4D8&icon_color=FACC15&bg_color=08080c&border_color=27273a&hide_border=false" width="49%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=imrangurmani&theme=dark&background=08080c&border=27273a&stroke=FACC15&ring=FACC15&fire=FACC15&currStreakNum=FACC15&sideNums=EAB308&currStreakLabel=FACC15&dates=A1A1AA" width="49%" />
</div>

<br>

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=imrangurmani&layout=compact&title_color=FACC15&text_color=D4D4D8&bg_color=08080c&border_color=27273a&hide_border=false" />
</div>

---

### 🐍 GitHub Contribution Snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/imrangurmani/imrangurmani/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/imrangurmani/imrangurmani/output/github-contribution-grid-snake.svg">
  <img alt="github contribution grid snake" src="https://raw.githubusercontent.com/imrangurmani/imrangurmani/output/github-contribution-grid-snake.svg">
</picture>

---

<p align="center">
  <em>Designed with pride for <strong>Imran Khan Gurmani (Jigar Gurmani)</strong> • <a href="https://imrangurmani.shop">imrangurmani.shop</a></em>
</p>
`;

    // 6. Modal Functions
    const modal = document.getElementById("readmeModal");
    const markdownArea = document.getElementById("markdownArea");
    const toast = document.getElementById("toast");
    const copyBtnLabel = document.getElementById("copyBtnLabel");

    markdownArea.value = customizedReadmeMarkdown;

    function openReadmeModal() {
      modal.classList.remove("hidden");
    }

    function closeReadmeModal() {
      modal.classList.add("hidden");
    }

    modal.addEventListener("click", (e) => {
      if (e.target === modal) closeReadmeModal();
    });

    function showToastNotification() {
      toast.classList.remove("translate-y-20", "opacity-0");
      setTimeout(() => {
        toast.classList.add("translate-y-20", "opacity-0");
      }, 3500);
    }

    function copyMarkdownText() {
      const tempTextArea = document.createElement("textarea");
      tempTextArea.value = customizedReadmeMarkdown;
      document.body.appendChild(tempTextArea);
      tempTextArea.select();
      try {
        document.execCommand('copy');
        showToastNotification();
        copyBtnLabel.textContent = "Copied!";
        setTimeout(() => {
          copyBtnLabel.textContent = "Copy All Code";
        }, 2500);
      } catch (err) {
        console.error("Copy failed", err);
      }
      document.body.removeChild(tempTextArea);
    }
  </script>
</body>
</html>
