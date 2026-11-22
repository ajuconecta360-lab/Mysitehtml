<!DOCTYPE html>
<html lang="pt-BR" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Cílios de Boneca | Alongamento de Cílios & Estética em Aracaju</title>
  <meta name="description" content="Realce sua beleza natural com alongamento de cílios, lash lifting e design de sobrancelhas na Aruana, Aracaju - SE. Conheça nosso studio em Tour Virtual 360°." />
  
  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,500&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
  
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- Lucide Icons -->
  <script src="https://unpkg.com/lucide@latest"></script>

  <!-- Three.js para visualização 360° interativa -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>

  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            nude: '#FAF6F2',
            rose: '#E8C5B8',
            champagne: '#C59B6D',
            coffee: '#3A2A24',
            coffeeLight: '#5C463D',
          },
          fontFamily: {
            serif: ['"Playfair Display"', 'serif'],
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
          }
        }
      }
    }
  </script>

  <style>
    body {
      background-color: #FAF6F2;
      color: #3A2A24;
      font-family: 'Plus Jakarta Sans', sans-serif;
    }
    h1, h2, h3, .font-serif {
      font-family: 'Playfair Display', serif;
    }
    .glass-nav {
      background: rgba(250, 246, 242, 0.92);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
    }
    .tour-container {
      position: relative;
      width: 100%;
      aspect-ratio: 16 / 9;
      min-height: 360px;
      border-radius: 1.5rem;
      overflow: hidden;
      box-shadow: 0 20px 45px -15px rgba(58, 42, 36, 0.18);
      border: 1px solid rgba(197, 155, 109, 0.35);
    }
    #canvas360 {
      width: 100%;
      height: 100%;
      display: block;
      cursor: grab;
    }
    #canvas360:active {
      cursor: grabbing;
    }
  </style>
</head>
<body class="antialiased selection:bg-rose selection:text-coffee">

  <!-- Navbar -->
  <header class="fixed top-0 inset-x-0 z-50 glass-nav border-b border-champagne/20">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 h-20 flex items-center justify-between">
      <a href="#" class="flex items-center gap-2.5">
        <span class="w-9 h-9 rounded-full bg-coffee text-nude flex items-center justify-center font-serif text-lg font-semibold">CB</span>
        <div>
          <span class="font-serif text-xl font-bold tracking-tight text-coffee block leading-none">Cílios de Boneca</span>
          <span class="text-[11px] uppercase tracking-[0.2em] text-champagne font-semibold">Studio & Estética</span>
        </div>
      </a>

      <!-- Desktop Menu -->
      <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-coffee/85">
        <a href="#procedimentos" class="hover:text-champagne transition">Procedimentos</a>
        <a href="#tour-360" class="hover:text-champagne transition flex items-center gap-1.5">
          <i data-lucide="compass" class="w-4 h-4 text-champagne"></i> Tour 360°
        </a>
        <a href="#avaliacoes" class="hover:text-champagne transition">Avaliações</a>
        <a href="#localizacao" class="hover:text-champagne transition">Localização</a>
      </nav>

      <div class="hidden md:flex items-center gap-3">
        <a href="#agendar" class="bg-coffee text-nude hover:bg-coffeeLight px-5 py-2.5 rounded-full text-sm font-semibold transition shadow-sm">
          Agendar Horário
        </a>
      </div>

      <!-- Mobile Menu Button -->
      <button id="mobileMenuBtn" class="md:hidden p-2 text-coffee rounded-lg hover:bg-rose/30" aria-label="Abrir menu">
        <i data-lucide="menu" class="w-6 h-6"></i>
      </button>
    </div>

    <!-- Mobile Dropdown -->
    <div id="mobileMenu" class="hidden md:hidden bg-nude border-b border-champagne/20 px-4 pt-2 pb-6 space-y-3">
      <a href="#procedimentos" class="block py-2 text-coffee font-medium border-b border-champagne/10">Procedimentos</a>
      <a href="#tour-360" class="block py-2 text-coffee font-medium border-b border-champagne/10">Tour Virtual 360°</a>
      <a href="#avaliacoes" class="block py-2 text-coffee font-medium border-b border-champagne/10">Avaliações 5.0 ★</a>
      <a href="#localizacao" class="block py-2 text-coffee font-medium border-b border-champagne/10">Onde Estamos</a>
      <a href="#agendar" class="block text-center bg-coffee text-nude py-3 rounded-full font-semibold mt-4">Agendar pelo WhatsApp</a>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="pt-32 pb-20 md:pt-40 md:pb-28 px-4 sm:px-6 relative overflow-hidden">
    <div class="absolute top-20 right-0 w-96 h-96 bg-rose/35 rounded-full blur-3xl -z-10"></div>
    <div class="absolute bottom-0 left-0 w-80 h-80 bg-champagne/15 rounded-full blur-3xl -z-10"></div>

    <div class="max-w-6xl mx-auto grid md:grid-cols-12 gap-12 items-center">
      <div class="md:col-span-7 space-y-6">
        <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-rose/40 border border-champagne/30 text-xs font-semibold text-coffee">
          <span class="text-champagne">★★★★★</span> Nota 5.0 no Google • Aruana, Aracaju - SE
        </div>

        <h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold text-coffee leading-[1.12]">
          O olhar marcante que você merece, com <span class="italic text-champagne font-normal">leveza e naturalidade.</span>
        </h1>

        <p class="text-base sm:text-lg text-coffee/80 max-w-xl leading-relaxed">
          Especialistas em extensão de cílios, lash lifting e design de sobrancelhas. Técnicas personalizadas para realçar a simetria do seu rosto sem pesar nos fios naturais.
        </p>

        <div class="flex flex-col sm:flex-row gap-4 pt-2">
          <a href="#agendar" class="inline-flex items-center justify-center gap-2 bg-coffee text-nude hover:bg-coffeeLight px-7 py-4 rounded-full font-semibold text-sm sm:text-base transition shadow-lg shadow-coffee/15">
            <i data-lucide="calendar-heart" class="w-5 h-5 text-rose"></i>
            Agendar Avaliação no WhatsApp
          </a>
          <a href="#tour-360" class="inline-flex items-center justify-center gap-2 bg-white/80 hover:bg-white text-coffee border border-champagne/40 px-7 py-4 rounded-full font-semibold text-sm sm:text-base transition">
            <i data-lucide="view" class="w-5 h-5 text-champagne"></i>
            Conhecer Studio em 360°
          </a>
        </div>

        <div class="grid grid-cols-3 gap-4 pt-6 border-t border-champagne/20 max-w-lg">
          <div>
            <p class="font-serif text-2xl font-bold text-coffee">100%</p>
            <p class="text-xs text-coffee/70">Fios isolados e seguros</p>
          </div>
          <div>
            <p class="font-serif text-2xl font-bold text-coffee">5.0 ★</p>
            <p class="text-xs text-coffee/70">Satisfação máxima</p>
          </div>
          <div>
            <p class="font-serif text-2xl font-bold text-coffee">Aruana</p>
            
