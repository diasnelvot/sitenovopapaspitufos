<!DOCTYPE html>
<html lang="pt-BR" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Papa's Pitufos | Haute Cuisine & Mixologia</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        royalDark: {
                            950: '#030712',
                            900: '#0B132B',
                            800: '#1C2541',
                            700: '#2A365B'
                        },
                        champagne: {
                            100: '#FAF8F5',
                            200: '#F3EDE2',
                            300: '#E7DC8A',
                            400: '#D2C1A0'
                        },
                        goldAccent: {
                            300: '#F7E7A9',
                            400: '#E5C158',
                            500: '#D4AF37',
                            600: '#B89228'
                        },
                        sapphire: {
                            300: '#93C5FD',
                            400: '#60A5FA',
                            500: '#2563EB',
                            600: '#1D4ED8',
                            800: '#1E3A8A',
                            900: '#0F172A'
                        }
                    },
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                        serif: ['Cinzel', 'Playfair Display', 'serif']
                    }
                }
            }
        }
    </script>
    <!-- FontAwesome 6.5 -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700;800;900&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: #030712;
            color: #F3EDE2;
            overflow-x: hidden;
        }

        /* Custom Subtle Scrollbar */
        ::-webkit-scrollbar {
            width: 6px;
            height: 6px;
        }
        ::-webkit-scrollbar-track {
            background: #030712;
        }
        ::-webkit-scrollbar-thumb {
            background: #2563EB;
            border-radius: 9999px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #D4AF37;
        }

        /* Luxury Glass & Surface Effects */
        .glass-panel {
            background: rgba(11, 19, 43, 0.88);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(37, 99, 235, 0.25);
        }
        .glass-card {
            background: rgba(28, 37, 65, 0.55);
            backdrop-filter: blur(14px);
            border: 1px solid rgba(212, 175, 55, 0.15);
            transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .glass-card:hover {
            transform: translateY(-4px);
            border-color: rgba(212, 175, 55, 0.45);
            box-shadow: 0 20px 40px -20px rgba(15, 23, 42, 0.9);
        }

        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }

        /* Smooth View Fade Transition */
        .page-view {
            animation: fadeIn 0.45s cubic-bezier(0.16, 1, 0.3, 1) forwards;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(10px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Glow effects */
        .gold-glow {
            box-shadow: 0 0 25px rgba(212, 175, 55, 0.2);
        }
        .sapphire-glow {
            box-shadow: 0 0 30px rgba(37, 99, 235, 0.25);
        }
    </style>
</head>
<body class="min-h-screen flex flex-col justify-between selection:bg-sapphire-500 selection:text-white bg-royalDark-950">

    <!-- HEADER / NAVEGAÇÃO -->
    <header class="sticky top-0 z-40 glass-panel border-b border-sapphire-500/30 px-4 lg:px-12 py-4 transition-all">
        <div class="max-w-7xl mx-auto flex items-center justify-between">
            
            <!-- Logo Elegante -->
            <a href="javascript:void(0)" onclick="navigateTo('home')" class="flex items-center gap-3 group">
                <div class="w-11 h-11 rounded-full border border-goldAccent-500/40 flex items-center justify-center bg-royalDark-900 shadow-lg group-hover:border-sapphire-400 group-hover:scale-105 transition-all">
                    <i class="fa-solid fa-crown text-goldAccent-400 text-base"></i>
                </div>
                <div>
                    <h1 class="font-serif text-lg sm:text-xl font-bold tracking-widest text-white uppercase">
                        Papa's Pitufos
                    </h1>
                    <p class="text-[9px] text-sapphire-400 tracking-[0.25em] uppercase font-semibold">Oitava Nota Gastrobar</p>
                </div>
            </a>

            <!-- Menu de NAVEGAÇÃO -->
            <nav class="hidden md:flex items-center gap-1 bg-royalDark-950/90 p-1.5 rounded-full border border-sapphire-500/30 text-xs font-medium tracking-wide shadow-inner">
                <button onclick="navigateTo('home')" id="nav-home" class="nav-btn px-4 py-2 rounded-full text-gray-300 hover:text-white transition-all">
                    Início
                </button>
                <button onclick="navigateTo('menu')" id="nav-menu" class="nav-btn px-4 py-2 rounded-full text-gray-300 hover:text-white transition-all">
                    Cardápio
                </button>
                <button onclick="navigateTo('about')" id="nav-about" class="nav-btn px-4 py-2 rounded-full text-gray-300 hover:text-white transition-all">
                    A Alquimia
                </button>
                <button onclick="navigateTo('events')" id="nav-events" class="nav-btn px-4 py-2 rounded-full text-gray-300 hover:text-white transition-all">
                    Experiências
                </button>
                <button onclick="navigateTo('reservations')" id="nav-reservations" class="nav-btn px-4 py-2 rounded-full text-gray-300 hover:text-white transition-all">
                    Reservas VIP
                </button>
            </nav>

            <!-- Ações -->
            <div class="flex items-center gap-2 sm:gap-3">
                <button onclick="openAdminLogin()" title="Painel de Gestão VIP" class="p-2.5 rounded-full bg-royalDark-800 border border-sapphire-500/30 text-sapphire-400 hover:bg-sapphire-600 hover:text-white transition-all flex items-center gap-2 text-xs">
                    <i class="fa-solid fa-sliders"></i>
                    <span class="hidden sm:inline font-semibold">Painel</span>
                </button>

                <button onclick="toggleCartModal()" class="px-4 py-2.5 rounded-full bg-gradient-to-r from-sapphire-600 via-sapphire-700 to-sapphire-800 border border-goldAccent-500/30 text-white font-bold hover:shadow-lg hover:shadow-sapphire-500/30 transition-all active:scale-95 flex items-center gap-2 text-xs">
                    <i class="fa-solid fa-wine-glass text-goldAccent-400"></i>
                    <span class="hidden sm:inline">Pedido</span>
                    <span id="cart-badge-count" class="px-2 py-0.5 rounded-full bg-royalDark-950 text-goldAccent-400 text-[10px] font-black border border-goldAccent-500/40">0</span>
                </button>
            </div>
        </div>
    </header>

    <!-- CONTEÚDO DINÂMICO MULTIPÁGINAS -->
    <main class="relative z-10 flex-grow max-w-7xl w-full mx-auto px-4 sm:px-6 lg:px-8 py-8 sm:py-12">

        <!-- ================= PAGE 1: INÍCIO (HOME) ================= -->
        <div id="page-home" class="page-view space-y-24">
            <!-- Hero Banner Sofisticado -->
            <section class="relative min-h-[70vh] flex items-center justify-center py-8">
                <div class="grid lg:grid-cols-12 gap-12 items-center w-full">
                    
                    <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                        <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-sapphire-500/10 border border-sapphire-400/30 text-sapphire-400 text-xs font-semibold tracking-widest uppercase">
                            <i class="fa-solid fa-gem text-[10px] text-goldAccent-400"></i> Alta Gastronomia & Mixologia Pitufo
                        </div>
                        
                        <h1 class="text-4xl sm:text-6xl font-serif font-extrabold tracking-tight text-white leading-[1.15]">
                            Onde a Alquimia Encanta os Sentidos.
                        </h1>

                        <p class="text-gray-300 text-sm sm:text-base leading-relaxed max-w-xl mx-auto lg:mx-0 font-light">
                            Uma experiência gastronômica memorável. Ingredientes raros de origem certificada, preparos moleculares e coquetelaria exclusiva em um ambiente azul safira intimista e refinado.
                        </p>

                        <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-4">
                            <button onclick="navigateTo('menu')" class="w-full sm:w-auto px-8 py-4 rounded-full bg-sapphire-600 hover:bg-sapphire-500 border border-goldAccent-500/40 text-white font-bold text-xs tracking-wider uppercase transition-all shadow-lg shadow-sapphire-600/30 flex items-center justify-center gap-3">
                                <i class="fa-solid fa-utensils text-goldAccent-400"></i> Explorar Cardápio Gourmet
                            </button>
                            <button onclick="navigateTo('reservations')" class="w-full sm:w-auto px-8 py-4 rounded-full glass-card text-champagne-100 font-semibold text-xs tracking-wider uppercase hover:bg-royalDark-800 transition-all border border-sapphire-500/30 flex items-center justify-center gap-2">
                                <i class="fa-solid fa-calendar-check text-sapphire-400"></i> Reserva VIP
                            </button>
                        </div>
                    </div>

                    <!-- Imagem de Destaque -->
                    <div class="lg:col-span-5 flex justify-center">
                        <div class="relative glass-card rounded-3xl p-4 border border-sapphire-500/40 max-w-md w-full shadow-2xl sapphire-glow">
                            <div class="relative h-80 rounded-2xl overflow-hidden">
                                <img src="https://images.unsplash.com/photo-1544025162-d76694265947?auto=format&fit=crop&w=800&q=80" alt="Prato Destaque Haute Cuisine" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/800x600/0B132B/D4AF37?text=Alta+Gastronomia'">
                                <div class="absolute inset-0 bg-gradient-to-t from-royalDark-950/95 via-transparent to-transparent"></div>
                                <div class="absolute bottom-4 left-4 right-4 text-left">
                                    <span class="text-[10px] font-bold uppercase tracking-widest text-goldAccent-400">Criação Assinada</span>
                                    <h3 class="font-serif text-lg font-bold text-white">Tornedor Wagyu A5 ao Poivre Nobre</h3>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </section>

            <!-- Destaques do Cardápio -->
            <section class="space-y-8">
                <div class="flex items-end justify-between border-b border-royalDark-800 pb-4">
                    <div>
                        <span class="text-[10px] font-bold tracking-widest text-sapphire-400 uppercase">Seleção do Chef Executivo</span>
                        <h2 class="text-2xl sm:text-3xl font-serif font-bold text-white">Pratos Emblemáticos</h2>
                    </div>
                    <button onclick="navigateTo('menu')" class="text-xs text-goldAccent-400 font-semibold hover:underline flex items-center gap-1">
                        Ver Cardápio Completo <i class="fa-solid fa-chevron-right text-[10px]"></i>
                    </button>
                </div>

                <div id="home-featured-grid" class="grid grid-cols-1 md:grid-cols-3 gap-6">
                    <!-- JS Injected -->
                </div>
            </section>

            <!-- Avaliações & Reconhecimentos -->
            <section class="glass-panel rounded-3xl p-8 sm:p-12 text-center space-y-6 border border-sapphire-500/30 gold-glow">
                <span class="text-xs font-bold uppercase tracking-widest text-goldAccent-400">Crítica Gastronômica Internacional</span>
                <blockquote class="font-serif text-lg sm:text-2xl text-champagne-200 max-w-3xl mx-auto italic leading-relaxed">
                    "O Papa's Pitufos redefine a haute cuisine contemporânea com uma atmosfera azul safira inigualável, insumos raríssimos e harmonizações geniais."
                </blockquote>
                <p class="text-xs font-semibold text-sapphire-400 uppercase tracking-wider">— Guia Internacional de Gastronomia Fina</p>
            </section>
        </div>

        <!-- ================= PAGE 2: CARDÁPIO ================= -->
        <div id="page-menu" class="page-view hidden space-y-8">
            <div class="text-center space-y-2">
                <span class="text-xs font-bold uppercase tracking-widest text-goldAccent-400 bg-sapphire-500/20 px-4 py-1.5 rounded-full border border-goldAccent-500/30">
                    Menu Gastronômico Completo
                </span>
                <h2 class="text-3xl sm:text-5xl font-serif font-bold text-white">Alta Gastronomia & Mixologia</h2>
                <p class="text-gray-300 max-w-2xl mx-auto text-xs sm:text-sm font-light">
                    Uma curadoria de ingredientes nobres: Trufas de Alba, Caviar Beluga, Wagyu A5, frutos do mar selvagens e elixires artesanais exclusivos.
                </p>
            </div>

            <!-- Filtros e Busca -->
            <div class="glass-panel p-5 rounded-2xl space-y-4 border border-sapphire-500/30">
                <div class="flex items-center gap-3 overflow-x-auto no-scrollbar pb-1" id="category-tabs">
                    <!-- JS Injected -->
                </div>

                <div class="flex flex-col sm:flex-row items-center justify-between gap-4 pt-3 border-t border-royalDark-800">
                    <div class="relative w-full sm:w-80">
                        <i class="fa-solid fa-magnifying-glass absolute left-3.5 top-1/2 -translate-y-1/2 text-gray-400 text-xs"></i>
                        <input type="text" id="search-input" oninput="renderMenu()" placeholder="Procurar prato, ingrediente ou drink..." class="w-full bg-royalDark-950/80 border border-sapphire-500/30 rounded-full pl-9 pr-4 py-2 text-xs text-white focus:outline-none focus:border-goldAccent-400 transition-all">
                    </div>

                    <select id="sort-select" onchange="renderMenu()" class="w-full sm:w-auto bg-royalDark-950/80 border border-sapphire-500/30 text-xs text-gray-200 rounded-full px-4 py-2 focus:outline-none focus:border-goldAccent-400">
                        <option value="popular">Destaques da Casa</option>
                        <option value="price-asc">Menor Preço</option>
                        <option value="price-desc">Maior Preço</option>
                    </select>
                </div>
            </div>

            <!-- Grid do Menu -->
            <div id="menu-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- JS Injected -->
            </div>
        </div>

        <!-- ================= PAGE 3: SOBRE NÓS ================= -->
        <div id="page-about" class="page-view hidden space-y-12">
            <div class="text-center space-y-2">
                <span class="text-xs font-bold uppercase tracking-widest text-sapphire-400 bg-sapphire-500/10 px-4 py-1.5 rounded-full border border-sapphire-500/20">
                    História & Tradição Nobre
                </span>
                <h2 class="text-3xl sm:text-5xl font-serif font-bold text-white">Nossa Filosofia Gastronômica</h2>
            </div>

            <div class="grid lg:grid-cols-2 gap-12 items-center">
                <div class="relative">
                    <div class="aspect-video rounded-3xl overflow-hidden border border-sapphire-500/40 shadow-2xl">
                        <img src="https://images.unsplash.com/photo-1555396273-367ea4eb4db5?auto=format&fit=crop&w=800&q=80" alt="Ambiente do Restaurante" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/800x500/0B132B/D4AF37?text=Ambiente+Safira'">
                    </div>
                </div>

                <div class="space-y-6">
                    <h3 class="text-2xl font-serif font-bold text-white">Sabor, Técnica Moleculares & Pureza</h3>
                    <p class="text-gray-300 leading-relaxed text-xs sm:text-sm font-light">
                        Criado para exigentes apreciadores do bom viver, o Papa's Pitufos unifica o rigor clássico da culinária europeia com toques de vanguarda e mixologia autoral em um ambiente envolvente no tom azul safira imperial.
                    </p>
                    <div class="grid grid-cols-2 gap-4 pt-2">
                        <div class="glass-card p-4 rounded-2xl border-l-2 border-l-goldAccent-400">
                            <h4 class="font-bold text-white text-sm">Cozinha Autoral</h4>
                            <p class="text-[11px] text-gray-400 mt-1">Pratos assinados por mestres com foco em textura e profundidade.</p>
                        </div>
                        <div class="glass-card p-4 rounded-2xl border-l-2 border-l-sapphire-400">
                            <h4 class="font-bold text-white text-sm">Mixologia Safira</h4>
                            <p class="text-[11px] text-gray-400 mt-1">Coquetéis moleculares com botânicos selvagens e esferificações.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- ================= PAGE 4: EXPERIÊNCIAS ================= -->
        <div id="page-events" class="page-view hidden space-y-12">
            <div class="text-center space-y-2">
                <span class="text-xs font-bold uppercase tracking-widest text-goldAccent-400 bg-sapphire-500/20 px-4 py-1.5 rounded-full border border-goldAccent-500/30">
                    Eventos Privativos & Masterclasses
                </span>
                <h2 class="text-3xl sm:text-5xl font-serif font-bold text-white">Experiências Exclusivas</h2>
                <p class="text-gray-300 max-w-xl mx-auto text-xs sm:text-sm font-light">
                    Jantares harmonizados em múltiplos tempos, noites de degustação de Caviar & Champagne e eventos corporativos de alto padrão.
                </p>
            </div>

            <div class="grid md:grid-cols-3 gap-6">
                <div class="glass-card p-6 rounded-3xl border border-sapphire-500/30 space-y-4 hover:border-goldAccent-400/50 transition-all">
                    <div class="w-12 h-12 rounded-2xl bg-royalDark-950 border border-goldAccent-400/30 flex items-center justify-center text-goldAccent-400 text-lg">
                        <i class="fa-solid fa-wine-bottle"></i>
                    </div>
                    <h3 class="font-serif font-bold text-lg text-white">Degustação Imperial em 7 Tempos</h3>
                    <p class="text-xs text-gray-300 font-light leading-relaxed">
                        Uma jornada multissensorial por insumos raros harmonizados com Grandes Crus e safras especiais selecionadas pelo nosso sommelier.
                    </p>
                    <button onclick="navigateTo('reservations')" class="text-xs font-bold text-goldAccent-400 hover:underline">Consultar Calendário VIP →</button>
                </div>

                <div class="glass-card p-6 rounded-3xl border border-sapphire-500/30 space-y-4 hover:border-sapphire-400/50 transition-all">
                    <div class="w-12 h-12 rounded-2xl bg-royalDark-950 border border-sapphire-400/30 flex items-center justify-center text-sapphire-400 text-lg">
                        <i class="fa-solid fa-champagne-glasses"></i>
                    </div>
                    <h3 class="font-serif font-bold text-lg text-white">Salão Secreto Safira</h3>
                    <p class="text-xs text-gray-300 font-light leading-relaxed">
                        Espaço privativo equipado com sistema acústico e atendimento dedicado de garçons e mixologistas exclusivos para até 20 pessoas.
                    </p>
                    <button onclick="navigateTo('reservations')" class="text-xs font-bold text-sapphire-400 hover:underline">Solicitar Orçamento →</button>
                </div>

                <div class="glass-card p-6 rounded-3xl border border-sapphire-500/30 space-y-4 hover:border-goldAccent-400/50 transition-all">
                    <div class="w-12 h-12 rounded-2xl bg-royalDark-950 border border-goldAccent-400/30 flex items-center justify-center text-goldAccent-400 text-lg">
                        <i class="fa-solid fa-flask text-sapphire-400"></i>
                    </div>
                    <h3 class="font-serif font-bold text-lg text-white">Masterclass de Mixologia Molecular</h3>
                    <p class="text-xs text-gray-300 font-light leading-relaxed">
                        Aprenda as técnicas de clarificação, infusão sob pressão e esferificação diretamente com nosso chefe de bar.
                    </p>
                    <button onclick="navigateTo('reservations')" class="text-xs font-bold text-goldAccent-400 hover:underline">Ver Próximas Turmas →</button>
                </div>
            </div>
        </div>

        <!-- ================= PAGE 5: RESERVAS VIP ================= -->
        <div id="page-reservations" class="page-view hidden max-w-3xl mx-auto py-4">
            <div class="glass-panel p-8 sm:p-12 rounded-3xl border border-sapphire-500/40 space-y-6 shadow-2xl">
                <div class="text-center space-y-2">
                    <span class="text-xs font-bold uppercase tracking-widest text-goldAccent-400 bg-sapphire-500/20 px-4 py-1.5 rounded-full border border-goldAccent-500/30">
                        Atendimento Preferencial VIP
                    </span>
                    <h2 class="text-3xl font-serif font-bold text-white">Reserva de Mesas & Lounges</h2>
                    <p class="text-gray-300 text-xs font-light">Garanta o seu espaço em nosso salão azul safira ou lounges privativos.</p>
                </div>

                <form onsubmit="handleReservationSubmit(event)" class="space-y-4 pt-2">
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div>
                            <label class="text-[11px] font-bold text-gray-300 uppercase tracking-wider block mb-1">Nome Completo</label>
                            <input type="text" required placeholder="Seu nome completo" class="w-full bg-royalDark-950 border border-sapphire-500/30 rounded-xl px-4 py-3 text-xs text-white focus:outline-none focus:border-goldAccent-400 transition-all">
                        </div>
                        <div>
                            <label class="text-[11px] font-bold text-gray-300 uppercase tracking-wider block mb-1">Telefone / WhatsApp</label>
                            <input type="tel" required placeholder="(11) 99999-9999" class="w-full bg-royalDark-950 border border-sapphire-500/30 rounded-xl px-4 py-3 text-xs text-white focus:outline-none focus:border-goldAccent-400 transition-all">
                        </div>
                        <div>
                            <label class="text-[11px] font-bold text-gray-300 uppercase tracking-wider block mb-1">Data Desejada</label>
                            <input type="date" required class="w-full bg-royalDark-950 border border-sapphire-500/30 rounded-xl px-4 py-3 text-xs text-white focus:outline-none focus:border-goldAccent-400 transition-all">
                        </div>
                        <div>
                            <label class="text-[11px] font-bold text-gray-300 uppercase tracking-wider block mb-1">Ambiente Desejado</label>
                            <select required class="w-full bg-royalDark-950 border border-sapphire-500/30 rounded-xl px-4 py-3 text-xs text-white focus:outline-none focus:border-goldAccent-400 transition-all">
                                <option value="balcao">Balcão do Alquimista (1-2 Pessoas)</option>
                                <option value="salao">Mesa Salão Safira (2-4 Pessoas)</option>
                                <option value="lounge">Sofa Lounge Imperial (4-6 Pessoas)</option>
                                <option value="vip">Camarote Privativo VIP (6+ Pessoas)</option>
                            </select>
                        </div>
                    </div>

                    <button type="submit" class="w-full py-4 rounded-xl bg-gradient-to-r from-sapphire-600 via-sapphire-700 to-sapphire-800 border border-goldAccent-500/40 text-white font-bold text-xs tracking-wider uppercase transition-all shadow-md hover:shadow-sapphire-500/30 mt-4 active:scale-[0.99]">
                        Solicitar Confirmação de Reserva VIP
                    </button>
                </form>
            </div>
        </div>

    </main>

    <!-- FOOTER NOBRE -->
    <footer class="relative z-10 glass-panel border-t border-sapphire-500/30 py-8 text-center text-xs text-gray-400 mt-12">
        <div class="max-w-7xl mx-auto px-4 flex flex-col sm:flex-row items-center justify-between gap-4">
            <p>© 2026 Papa's Pitufos Haute Cuisine. Todos os direitos reservados.</p>
            <div class="flex items-center gap-4 text-gray-300">
                <a href="javascript:void(0)" onclick="navigateTo('home')" class="hover:text-goldAccent-400 transition-colors">Início</a>
                <a href="javascript:void(0)" onclick="navigateTo('menu')" class="hover:text-goldAccent-400 transition-colors">Cardápio</a>
                <a href="javascript:void(0)" onclick="navigateTo('events')" class="hover:text-goldAccent-400 transition-colors">Experiências</a>
                <a href="javascript:void(0)" onclick="navigateTo('reservations')" class="hover:text-goldAccent-400 transition-colors">Reservas</a>
            </div>
        </div>
    </footer>

    <!-- MODAL DE DETALHES DO ITEM -->
    <div id="item-modal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4 bg-royalDark-950/90 backdrop-blur-md">
        <div class="glass-panel w-full max-w-md rounded-3xl overflow-hidden border border-sapphire-500/50 shadow-2xl p-6 space-y-4">
            <div class="flex justify-between items-start">
                <div>
                    <span id="modal-tag" class="text-[9px] font-extrabold uppercase tracking-widest text-goldAccent-400"></span>
                    <h3 id="modal-title" class="font-serif text-xl font-bold text-white"></h3>
                </div>
                <button onclick="closeModal('item-modal')" class="text-gray-400 hover:text-white"><i class="fa-solid fa-xmark text-lg"></i></button>
            </div>
            <img id="modal-img" class="w-full h-48 object-cover rounded-2xl border border-sapphire-500/30" onerror="this.src='https://placehold.co/600x400/0B132B/D4AF37?text=Gastronomia'">
            <p id="modal-desc" class="text-xs text-gray-300 leading-relaxed font-light"></p>
            <div class="flex items-center justify-between pt-2">
                <span id="modal-price" class="text-xl font-bold text-goldAccent-400"></span>
                <button onclick="addModalItemToCart()" class="px-5 py-2.5 rounded-xl bg-sapphire-600 border border-goldAccent-500/40 text-white font-bold text-xs hover:bg-sapphire-500 transition-all shadow-md">
                    Adicionar ao Pedido
                </button>
            </div>
        </div>
    </div>

    <!-- SIDEBAR DO CARRINHO -->
    <div id="cart-sidebar" class="fixed inset-0 z-50 hidden">
        <div onclick="toggleCartModal()" class="absolute inset-0 bg-royalDark-950/80 backdrop-blur-sm"></div>
        <div class="absolute right-0 top-0 bottom-0 w-full max-w-sm glass-panel p-6 flex flex-col justify-between shadow-2xl border-l border-sapphire-500/40">
            <div class="flex items-center justify-between pb-4 border-b border-royalDark-800">
                <h3 class="font-serif text-lg font-bold text-white flex items-center gap-2">
                    <i class="fa-solid fa-wine-glass text-goldAccent-400"></i> Seu Pedido VIP
                </h3>
                <button onclick="toggleCartModal()" class="text-gray-400 hover:text-white"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div id="cart-items" class="flex-grow my-4 overflow-y-auto space-y-3 pr-1"></div>
            <div class="pt-4 border-t border-royalDark-800 space-y-3">
                <div class="flex justify-between text-sm font-bold text-white">
                    <span>Total do Pedido:</span>
                    <span id="cart-total-val" class="text-goldAccent-400 font-extrabold">R$ 0,00</span>
                </div>
                <button onclick="clearCart()" class="w-full py-3.5 rounded-full bg-sapphire-600 border border-goldAccent-500/40 hover:bg-sapphire-500 text-white font-bold text-xs tracking-wider uppercase transition-all shadow-md">
                    Confirmar & Enviar à Cozinha
                </button>
            </div>
        </div>
    </div>

    <!-- ACESSO RESTRITO AO PAINEL -->
    <div id="admin-login" class="fixed inset-0 z-[60] hidden flex items-center justify-center p-4 bg-royalDark-950/95 backdrop-blur-md">
        <div class="glass-panel w-full max-w-sm rounded-3xl p-7 border border-goldAccent-500/40 space-y-5 shadow-2xl">
            <div class="text-center space-y-2">
                <div class="mx-auto w-12 h-12 rounded-full flex items-center justify-center bg-sapphire-600/20 border border-goldAccent-500/40 text-goldAccent-400">
                    <i class="fa-solid fa-lock text-lg"></i>
                </div>
                <h3 class="font-serif text-xl font-bold text-white">Acesso Administrativo</h3>
                <p class="text-xs text-gray-400">Digite a senha para consultar os pedidos do restaurante.</p>
            </div>
            <form onsubmit="checkAdminPassword(event)" class="space-y-3">
                <input id="admin-password" type="password" required autocomplete="current-password"
                    placeholder="Senha do painel"
                    class="w-full bg-royalDark-950 border border-sapphire-500/30 rounded-xl px-4 py-3 text-sm text-white focus:outline-none focus:border-goldAccent-400">
                <p id="admin-login-error" class="hidden text-xs text-red-400">Senha incorreta. Tente novamente.</p>
                <button type="submit" class="w-full py-3 rounded-xl bg-sapphire-600 hover:bg-sapphire-500 text-white font-bold text-xs uppercase tracking-wider">Entrar</button>
                <button type="button" onclick="closeAdminLogin()" class="w-full py-2 text-xs text-gray-400 hover:text-white">Cancelar</button>
            </form>
        </div>
    </div>

    <!-- PAINEL VIP DE GESTÃO -->
    <div id="admin-panel" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4 bg-royalDark-950/90 backdrop-blur-md">
        <div class="glass-panel w-full max-w-xl rounded-3xl p-6 border border-sapphire-500/50 space-y-4 shadow-2xl">
            <div class="flex justify-between items-center pb-3 border-b border-royalDark-800">
                <h3 class="font-serif text-lg font-bold text-goldAccent-400 flex items-center gap-2">
                    <i class="fa-solid fa-sliders"></i> Painel de Gestão do Restaurante
                </h3>
                <button onclick="toggleAdminPanel()" class="text-gray-400 hover:text-white"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="grid grid-cols-2 gap-4 text-center">
                <div class="p-4 rounded-2xl bg-royalDark-950/80 border border-sapphire-500/30">
                    <span class="text-xs text-gray-400 uppercase font-semibold">Faturamento da Sessão</span>
                    <h4 id="admin-sales" class="text-2xl font-bold text-goldAccent-400 mt-1">R$ 0,00</h4>
                </div>
                <div class="p-4 rounded-2xl bg-royalDark-950/80 border border-sapphire-500/30">
                    <span class="text-xs text-gray-400 uppercase font-semibold">Pedidos Concluídos</span>
                    <h4 id="admin-count" class="text-2xl font-bold text-white mt-1">0</h4>
                </div>
            </div>
            <div class="flex flex-col sm:flex-row sm:items-center sm:justify-between gap-3">
                <div>
                    <h4 class="text-sm font-bold text-white">Resumo diário de pedidos</h4>
                    <p class="text-[11px] text-gray-400">Os registros ficam salvos neste navegador.</p>
                </div>
                <div class="flex items-center gap-2">
                    <input id="report-date" type="date" onchange="renderDailyReport()"
                        class="bg-royalDark-950 border border-sapphire-500/30 rounded-lg px-3 py-2 text-xs text-white">
                    <button onclick="exportDailyReport()" class="px-3 py-2 rounded-lg bg-sapphire-600 hover:bg-sapphire-500 text-white text-xs font-bold">
                        <i class="fa-solid fa-download mr-1"></i> Exportar CSV
                    </button>
                </div>
            </div>
            <div class="grid grid-cols-2 gap-3 text-center">
                <div class="p-3 rounded-xl bg-royalDark-950/80 border border-sapphire-500/30">
                    <span class="text-[10px] text-gray-400 uppercase font-semibold">Pedidos no dia</span>
                    <h4 id="admin-daily-count" class="text-xl font-bold text-white mt-1">0</h4>
                </div>
                <div class="p-3 rounded-xl bg-royalDark-950/80 border border-sapphire-500/30">
                    <span class="text-[10px] text-gray-400 uppercase font-semibold">Total do dia</span>
                    <h4 id="admin-daily-sales" class="text-xl font-bold text-goldAccent-400 mt-1">R$ 0,00</h4>
                </div>
            </div>
            <div class="overflow-x-auto max-h-64 overflow-y-auto rounded-xl border border-sapphire-500/20">
                <table class="w-full text-left text-xs">
                    <thead class="sticky top-0 bg-royalDark-900 text-goldAccent-400">
                        <tr>
                            <th class="p-3">Hora</th><th class="p-3">Pedido</th><th class="p-3">Itens</th><th class="p-3">Total</th>
                        </tr>
                    </thead>
                    <tbody id="admin-orders-table" class="divide-y divide-sapphire-500/10 text-gray-200">
                        <tr><td colspan="4" class="p-4 text-center text-gray-400">Nenhum pedido registrado neste dia.</td></tr>
                    </tbody>
                </table>
            </div>
            <div class="flex justify-end">
                <button onclick="clearDailyOrders()" class="px-3 py-2 rounded-lg border border-red-500/30 text-red-300 hover:bg-red-500/10 text-xs">
                    Limpar registros do dia
                </button>
            </div>
        </div>
    </div>

    <!-- TOAST NOTIFICATION -->
    <div id="toast" class="fixed bottom-6 right-6 z-50 hidden glass-panel px-5 py-3 rounded-2xl border border-goldAccent-400 text-xs font-semibold text-white shadow-xl"></div>

    <script>
        // EXPANDED GOURMET MENU DATA
        const MENU = [
            // GASTRONOMIA / ENTRADAS NOBRES & PRATOS PRINCIPAIS
            { id: 1, title: "Tornedor Wagyu A5 ao Poivre Nobre", cat: "eats", tag: "Especialidade do Chef", price: 185.00, img: "https://images.unsplash.com/photo-1544025162-d76694265947?auto=format&fit=crop&w=600&q=80", desc: "Corte nobre de Wagyu A5 selado na crosta de pimentas selecionadas, demiglace ao cognac e mousseline leve de batata trufada." },
            { id: 2, title: "Canapés de Caviar Beluga & Blinis", cat: "eats", tag: "Exclusivo", price: 210.00, img: "https://images.unsplash.com/photo-1534422298391-e4f8c172dddb?auto=format&fit=crop&w=600&q=80", desc: "Caviar Beluga sobre blinis aquecidos, creme de fraîche refinado, ciboulette picada e lascas de lâmina de ouro 24k." },
            { id: 3, title: "Bisque de Lagosta com Açafrão Real", cat: "eats", tag: "Culinária Francesa", price: 145.00, img: "https://images.unsplash.com/photo-1559847844-5315695dadae?auto=format&fit=crop&w=600&q=80", desc: "Sopa aveludada de lagosta grelhada com estigmas de açafrão do Irã, finalizada com emulsão de ervas finas e crostini de sourdough." },
            { id: 4, title: "Risoto de Cavaquinha & Trufas Negras", cat: "eats", tag: "Autoral", price: 165.00, img: "https://images.unsplash.com/photo-1633964913295-ceb43826e7c9?auto=format&fit=crop&w=600&q=80", desc: "Arroz arbóreo italiano com medalhões de cavaquinha, manteiga noisette e lâminas frescas de trufa negra de Alba." },
            { id: 5, title: "Ceviche de Robalo em Leite de Tigre Azul", cat: "eats", tag: "Mixologia Gastronômica", price: 88.00, img: "https://images.unsplash.com/photo-1535399831218-d5bd36d1a6b3?auto=format&fit=crop&w=600&q=80", desc: "Robalo selvagem marinado em infusão cítrica natural de flor de fada, abacate macerado, milho crocante e pimenta rosa." },
            { id: 6, title: "Tapas de Cogumelos Eringui Trufados", cat: "eats", tag: "Vegetariano Gourmet", price: 72.00, img: "https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=600&q=80", desc: "Cogumelos silvestres e eringui grelhados no azeite extravirgem trufado, servidos sobre broa artesanal tostada ao alho confit." },
            { id: 7, title: "Carpaccio de Polvo ao Molho Cítrico", cat: "eats", tag: "Frutos do Mar", price: 95.00, img: "https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=600&q=80", desc: "Lâminas ultrafinas de polvo grelhado, alcaparras crocantes, flor de sal e azeite verde de manjericão." },

            // MIXOLOGIA & ELIXIRES SAFIRA
            { id: 8, title: "Elixir Safira Dourado Pitufos", cat: "drinks", tag: "Assinatura da Casa", price: 58.00, img: "https://images.unsplash.com/photo-1514362545857-3bc16c4c7d1b?auto=format&fit=crop&w=600&q=80", desc: "Gin botânico safira, água tônica artesanal de flor de sabugueiro, licor de mirtilo e brilho comestível mineral." },
            { id: 9, title: "Smoked Bourbon Old Fashioned", cat: "drinks", tag: "Defumado na Mesa", price: 65.00, img: "https://images.unsplash.com/photo-1510812431401-41d2bd2722f3?auto=format&fit=crop&w=600&q=80", desc: "Bourbon maturado em carvalho, bitters aromáticos de especiarias e névoa defumada de madeira de macieira sob campânula." },
            { id: 10, title: "Smurfberry Royale Molecular", cat: "drinks", tag: "Molecular", price: 52.00, img: "https://images.unsplash.com/photo-1551024709-8f23befc6f87?auto=format&fit=crop&w=600&q=80", desc: "Vodka premium com infusão artesanal de amora silvestre, licor de cassis e esfera molecular expansiva de limão siciliano." },
            { id: 11, title: "Coquetel Lumina Botânico 24k", cat: "drinks", tag: "Premium", price: 68.00, img: "https://images.unsplash.com/photo-1536935338788-846bb9981813?auto=format&fit=crop&w=600&q=80", desc: "Tequila reposado, licor St. Germain, tônica artesanal e flocos flutuantes de ouro puro comestível." },
            { id: 12, title: "Infusão Mística de Ervas (Zero Álcool)", cat: "drinks", tag: "Mocktail", price: 38.00, img: "https://images.unsplash.com/photo-1556881286-fc6915169721?auto=format&fit=crop&w=600&q=80", desc: "Néctar de tangerina fresca, chá de borboleta azul, xarope caseiro de gengibre e espuma suave de capim-santo." },

            // SOBREMESAS AUTORAIS
            { id: 13, title: "Esfera Belgacom & Gelato de Baunilha Bourbon", cat: "desserts", tag: "Sobremesa Assinada", price: 55.00, img: "https://images.unsplash.com/photo-1579372786545-d24232daf58c?auto=format&fit=crop&w=600&q=80", desc: "Esfera de chocolate belga 70% recheada com gelato artesanal de baunilha Bourbon, servida com calda quente de avelã." },
            { id: 14, title: "Soufflé Quente de Pistache Siciliano", cat: "desserts", tag: "Culinária Doce", price: 52.00, img: "https://images.unsplash.com/photo-1606313564200-e75d5e30476c?auto=format&fit=crop&w=600&q=80", desc: "Soufflé aerado de pistache de Bronte, acompanhado de sorbet de limão e crocante de praliné." },
            { id: 15, title: "Velvet Azul Papa's Haute", cat: "desserts", tag: "Exclusivo", price: 46.00, img: "https://images.unsplash.com/photo-1588195538326-c5b1e9f80a1b?auto=format&fit=crop&w=600&q=80", desc: "Bolo aveludado de amêndoas com creme levemente cítrico de mascarpone e merengue italiano maçaricado." },
            { id: 16, title: "Mille-Feuille de Baunilha & Macadâmia", cat: "desserts", tag: "Clássico", price: 44.00, img: "https://images.unsplash.com/photo-1509440159596-0249088772ff?auto=format&fit=crop&w=600&q=80", desc: "Massa folhada caramelizada em camadas com mousseline de baunilha de Madagascar e macadâmias crocantes." }
        ];

        const CATS = [
            { id: "all", name: "Cardápio Completo" },
            { id: "eats", name: "Gastronomia & Entradas" },
            { id: "drinks", name: "Mixologia & Elixires" },
            { id: "desserts", name: "Sobremesas Haute" }
        ];

        let currentPage = "home";
        let activeCat = "all";
        let cart = [];
        let selectedItem = null;
        let totalSales = 0;
        let ordersCount = 0;

        // Roteamento de Páginas
        function navigateTo(pageId) {
            currentPage = pageId;
            const pages = ['home', 'menu', 'about', 'events', 'reservations'];
            
            pages.forEach(p => {
                const el = document.getElementById(`page-${p}`);
                if (el) {
                    if (p === pageId) {
                        el.classList.remove('hidden');
                    } else {
                        el.classList.add('hidden');
                    }
                }
            });

            updateNavigationUI();
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        function updateNavigationUI() {
            const pages = ['home', 'menu', 'about', 'events', 'reservations'];
            pages.forEach(p => {
                const btn = document.getElementById(`nav-${p}`);
                if (btn) {
                    if (p === currentPage) {
                        btn.className = "nav-btn px-4 py-2 rounded-full text-goldAccent-400 bg-sapphire-600/30 border border-goldAccent-500/40 font-bold transition-all shadow-md";
                    } else {
                        btn.className = "nav-btn px-4 py-2 rounded-full text-gray-300 hover:text-white transition-all";
                    }
                }
            });
        }

        function renderTabs() {
            document.getElementById('category-tabs').innerHTML = CATS.map(c => {
                const count = c.id === 'all' ? MENU.length : MENU.filter(i => i.cat === c.id).length;
                return `
                <button onclick="setCat('${c.id}')" class="px-4 py-2 rounded-full text-xs font-semibold transition-all whitespace-nowrap flex items-center gap-2 ${activeCat === c.id ? 'bg-sapphire-600 text-white font-bold shadow-md border border-goldAccent-500/40' : 'bg-royalDark-950/80 text-gray-300 hover:bg-royalDark-800'}">
                    <span>${c.name}</span>
                    <span class="px-1.5 py-0.5 rounded-full text-[10px] ${activeCat === c.id ? 'bg-royalDark-950 text-goldAccent-400 font-bold' : 'bg-royalDark-900 text-sapphire-400'}">${count}</span>
                </button>
            `}).join('');
        }

        function setCat(id) {
            activeCat = id;
            renderTabs();
            renderMenu();
        }

        function renderFeaturedHome() {
            const featured = [MENU[0], MENU[1], MENU[3], MENU[7], MENU[8], MENU[12]];
            document.getElementById('home-featured-grid').innerHTML = featured.map(i => `
                <div class="glass-card rounded-2xl overflow-hidden p-4 space-y-3 flex flex-col justify-between group border border-sapphire-500/20">
                    <div class="relative overflow-hidden rounded-xl h-48">
                        <img src="${i.img}" alt="${i.title}" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" onerror="this.src='https://placehold.co/600x400/0B132B/D4AF37?text=${encodeURIComponent(i.title)}'">
                        <span class="absolute top-2 left-2 px-2.5 py-1 rounded-full bg-royalDark-950/80 backdrop-blur-md text-[9px] font-bold text-goldAccent-400 border border-goldAccent-500/30 uppercase tracking-wider">${i.tag}</span>
                    </div>
                    <div class="space-y-1">
                        <h4 class="font-serif font-bold text-white text-base">${i.title}</h4>
                        <p class="text-xs text-gray-300 font-light line-clamp-2">${i.desc}</p>
                    </div>
                    <div class="flex items-center justify-between pt-2 border-t border-royalDark-800">
                        <span class="font-bold text-goldAccent-400 text-sm">R$ ${i.price.toFixed(2)}</span>
                        <div class="flex items-center gap-2">
                            <button onclick="addToCartDirect(${i.id})" class="p-2 rounded-lg bg-sapphire-600/30 text-goldAccent-400 hover:bg-sapphire-600 hover:text-white transition-all" title="Adicionar">
                                <i class="fa-solid fa-plus text-xs"></i>
                            </button>
                            <button onclick="openModal(${i.id})" class="px-3 py-1.5 rounded-lg bg-royalDark-950 text-gray-200 text-xs font-semibold hover:bg-royalDark-800 transition-all border border-sapphire-500/30">Detalhes</button>
                        </div>
                    </div>
                </div>
            `).join('');
        }

        function renderMenu() {
            const search = document.getElementById('search-input').value.toLowerCase();
            const sort = document.getElementById('sort-select').value;

            let items = MENU.filter(i => (activeCat === 'all' || i.cat === activeCat) && (i.title.toLowerCase().includes(search) || i.desc.toLowerCase().includes(search) || i.tag.toLowerCase().includes(search)));

            if (sort === 'price-asc') items.sort((a,b) => a.price - b.price);
            if (sort === 'price-desc') items.sort((a,b) => b.price - a.price);

            const grid = document.getElementById('menu-grid');
            if (items.length === 0) {
                grid.innerHTML = `
                    <div class="col-span-full text-center py-12 space-y-2 glass-card rounded-2xl">
                        <i class="fa-solid fa-utensils text-2xl text-gray-500"></i>
                        <p class="text-xs text-gray-400 font-semibold">Nenhum item gourmet encontrado para a pesquisa.</p>
                    </div>
                `;
                return;
            }

            grid.innerHTML = items.map(i => `
                <div class="glass-card rounded-2xl overflow-hidden p-4 space-y-3 flex flex-col justify-between group border border-sapphire-500/20">
                    <div class="relative overflow-hidden rounded-xl h-48">
                        <img src="${i.img}" alt="${i.title}" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" onerror="this.src='https://placehold.co/600x400/0B132B/D4AF37?text=${encodeURIComponent(i.title)}'">
                        <span class="absolute top-2 left-2 px-2.5 py-1 rounded-full bg-royalDark-950/80 backdrop-blur-md text-[9px] font-bold text-goldAccent-400 border border-goldAccent-500/30 uppercase tracking-wider">${i.tag}</span>
                    </div>
                    <div class="space-y-1">
                        <h4 class="font-serif font-bold text-white text-base">${i.title}</h4>
                        <p class="text-xs text-gray-300 font-light line-clamp-2">${i.desc}</p>
                    </div>
                    <div class="flex items-center justify-between pt-2 border-t border-royalDark-800">
                        <span class="font-bold text-goldAccent-400 text-base">R$ ${i.price.toFixed(2)}</span>
                        <div class="flex items-center gap-2">
                            <button onclick="addToCartDirect(${i.id})" class="px-3 py-1.5 rounded-full bg-sapphire-600 border border-goldAccent-500/30 text-white text-xs font-bold hover:bg-sapphire-500 transition-all flex items-center gap-1 shadow-sm">
                                <i class="fa-solid fa-plus text-[10px]"></i> Pedir
                            </button>
                            <button onclick="openModal(${i.id})" class="p-2 rounded-full bg-royalDark-950 text-gray-300 hover:bg-royalDark-800 transition-all border border-sapphire-500/20" title="Ver Detalhes">
                                <i class="fa-solid fa-eye text-xs"></i>
                            </button>
                        </div>
                    </div>
                </div>
            `).join('');
        }

        function closeModal(id) {
            const el = document.getElementById(id);
            if (el) el.classList.add('hidden');
        }

        function addToCartDirect(id) {
            const item = MENU.find(i => i.id === Number(id));
            if (!item) return;
            const existing = cart.find(c => c.id === item.id);
            if (existing) existing.qty += 1;
            else cart.push({ ...item, qty: 1 });
            updateCart();
            showToast(`${item.title} adicionado ao pedido!`);
        }

        function addModalItemToCart() {
            if (!selectedItem) return;
            addToCartDirect(selectedItem.id);
            closeModal('item-modal');
        }

        function changeCartQty(id, delta) {
            const item = cart.find(i => i.id === Number(id));
            if (!item) return;
            item.qty += delta;
            if (item.qty <= 0) cart = cart.filter(i => i.id !== Number(id));
            updateCart();
        }

        function toggleCartModal() {
            document.getElementById('cart-sidebar').classList.toggle('hidden');
            updateCart();
        }

        function updateCart() {
            const totalQty = cart.reduce((sum, item) => sum + item.qty, 0);
            document.getElementById('cart-badge-count').innerText = totalQty;
            const container = document.getElementById('cart-items');

            if (!cart.length) {
                container.innerHTML = `<div class="text-center py-12 space-y-2 text-gray-400">
                    <i class="fa-solid fa-wine-glass text-2xl text-sapphire-400"></i>
                    <p class="text-xs font-semibold">Seu pedido VIP está vazio.</p></div>`;
            } else {
                container.innerHTML = cart.map(item => `
                    <div class="flex items-center justify-between p-3 rounded-xl bg-royalDark-950 border border-sapphire-500/20 text-xs text-white">
                        <div class="space-y-0.5 max-w-[150px]">
                            <p class="font-bold">${item.title}</p>
                            <p class="text-goldAccent-400 font-bold text-[11px]">R$ ${(item.price * item.qty).toFixed(2).replace('.', ',')}</p>
                        </div>
                        <div class="flex items-center gap-2 bg-royalDark-900 px-2 py-1 rounded-lg border border-sapphire-500/30">
                            <button onclick="changeCartQty(${item.id}, -1)" class="text-gray-300 px-1 font-bold" aria-label="Diminuir">−</button>
                            <span class="text-xs font-bold text-goldAccent-400 w-4 text-center">${item.qty}</span>
                            <button onclick="changeCartQty(${item.id}, 1)" class="text-gray-300 px-1 font-bold" aria-label="Aumentar">+</button>
                        </div>
                    </div>`).join('');
            }
            const total = cart.reduce((sum, item) => sum + item.price * item.qty, 0);
            document.getElementById('cart-total-val').innerText = formatBRL(total);
        }

        function formatBRL(value) {
            return value.toLocaleString('pt-BR', { style: 'currency', currency: 'BRL' });
        }

        function localDateKey(date = new Date()) {
            const y = date.getFullYear();
            const m = String(date.getMonth() + 1).padStart(2, '0');
            const d = String(date.getDate()).padStart(2, '0');
            return `${y}-${m}-${d}`;
        }

        function getSavedOrders() {
            try { return JSON.parse(localStorage.getItem('papasPitufosOrders') || '[]'); }
            catch (error) { return []; }
        }

        function saveOrders(orders) {
            localStorage.setItem('papasPitufosOrders', JSON.stringify(orders));
        }

        function clearCart() {
            if (!cart.length) {
                showToast('Adicione pelo menos um item antes de confirmar.');
                return;
            }
            const orderItems = cart.map(item => ({
                id: item.id, title: item.title, price: item.price, qty: item.qty
            }));
            const total = orderItems.reduce((sum, item) => sum + item.price * item.qty, 0);
            const orders = getSavedOrders();
            orders.push({
                number: orders.length ? Math.max(...orders.map(o => o.number || 0)) + 1 : 1,
                date: localDateKey(),
                time: new Date().toLocaleTimeString('pt-BR', { hour: '2-digit', minute: '2-digit' }),
                items: orderItems,
                total
            });
            saveOrders(orders);
            totalSales += total;
            ordersCount += 1;
            cart = [];
            updateCart();
            closeModal('cart-sidebar');
            renderDailyReport();
            showToast('Pedido confirmado e enviado para a cozinha!');
        }

        function openAdminLogin() {
            document.getElementById('admin-password').value = '';
            document.getElementById('admin-login-error').classList.add('hidden');
            document.getElementById('admin-login').classList.remove('hidden');
            setTimeout(() => document.getElementById('admin-password').focus(), 50);
        }

        function closeAdminLogin() {
            document.getElementById('admin-login').classList.add('hidden');
        }

        function checkAdminPassword(event) {
            event.preventDefault();
            const ADMIN_PASSWORD = 'pitufos2026';
            const entered = document.getElementById('admin-password').value;
            if (entered !== ADMIN_PASSWORD) {
                document.getElementById('admin-login-error').classList.remove('hidden');
                return;
            }
            closeAdminLogin();
            document.getElementById('admin-panel').classList.remove('hidden');
            const orders = getSavedOrders();
            totalSales = orders.reduce((sum, order) => sum + order.total, 0);
            ordersCount = orders.length;
            document.getElementById('admin-sales').innerText = formatBRL(totalSales);
            document.getElementById('admin-count').innerText = ordersCount;
            const dateInput = document.getElementById('report-date');
            if (!dateInput.value) dateInput.value = localDateKey();
            renderDailyReport();
        }

        function toggleAdminPanel() {
            const panel = document.getElementById('admin-panel');
            if (panel.classList.contains('hidden')) openAdminLogin();
            else panel.classList.add('hidden');
        }

        function renderDailyReport() {
            const dateInput = document.getElementById('report-date');
            if (!dateInput) return;
            const chosenDate = dateInput.value || localDateKey();
            const orders = getSavedOrders().filter(order => order.date === chosenDate);
            const dailyTotal = orders.reduce((sum, order) => sum + order.total, 0);
            document.getElementById('admin-daily-count').innerText = orders.length;
            document.getElementById('admin-daily-sales').innerText = formatBRL(dailyTotal);
            const tbody = document.getElementById('admin-orders-table');

            if (!orders.length) {
                tbody.innerHTML = `<tr><td colspan="4" class="p-4 text-center text-gray-400">Nenhum pedido registrado neste dia.</td></tr>`;
                return;
            }

            tbody.innerHTML = orders.map(order => {
                const details = order.items.map(item => `${item.qty}× ${item.title}`).join(', ');
                return `<tr class="align-top">
                    <td class="p-3 whitespace-nowrap">${order.time}</td>
                    <td class="p-3">#${order.number}</td>
                    <td class="p-3 min-w-40">${details}</td>
                    <td class="p-3 whitespace-nowrap text-goldAccent-400 font-bold">${formatBRL(order.total)}</td>
                </tr>`;
            }).join('');
        }

        function exportDailyReport() {
            const chosenDate = document.getElementById('report-date').value || localDateKey();
            const orders = getSavedOrders().filter(order => order.date === chosenDate);
            if (!orders.length) {
                showToast('Não há pedidos nesta data para exportar.');
                return;
            }
            const rows = [['Pedido', 'Data', 'Hora', 'Itens', 'Total']];
            orders.forEach(order => {
                const items = order.items.map(item => `${item.qty}x ${item.title}`).join(' | ');
                rows.push([order.number, order.date, order.time, items, order.total.toFixed(2)]);
            });
            const csv = '\uFEFF' + rows.map(row => row.map(value => `"${String(value).replace(/"/g, '""')}"`).join(';')).join('\r\n');
            const blob = new Blob([csv], { type: 'text/csv;charset=utf-8;' });
            const url = URL.createObjectURL(blob);
            const link = document.createElement('a');
            link.href = url;
            link.download = `pedidos-papas-pitufos-${chosenDate}.csv`;
            document.body.appendChild(link);
            link.click();
            link.remove();
            URL.revokeObjectURL(url);
            showToast('Relatório CSV exportado!');
        }

        function clearDailyOrders() {
            const chosenDate = document.getElementById('report-date').value || localDateKey();
            saveOrders(getSavedOrders().filter(order => order.date !== chosenDate));
            const orders = getSavedOrders();
            totalSales = orders.reduce((sum, order) => sum + order.total, 0);
            ordersCount = orders.length;
            document.getElementById('admin-sales').innerText = formatBRL(totalSales);
            document.getElementById('admin-count').innerText = ordersCount;
            renderDailyReport();
            showToast('Registros do dia apagados.');
        }

        function handleReservationSubmit(event) {
            event.preventDefault();
            showToast('Solicitação de reserva registrada com sucesso! Entraremos em contato.');
            event.target.reset();
        }

        let toastTimeout;
        function showToast(message) {
            const toast = document.getElementById('toast');
            toast.innerText = message;
            toast.classList.remove('hidden');
            clearTimeout(toastTimeout);
            toastTimeout = setTimeout(() => toast.classList.add('hidden'), 3500);
        }

        function openModal(id) {
            selectedItem = MENU.find(item => item.id === Number(id));
            if (!selectedItem) return;
            document.getElementById('modal-tag').innerText = selectedItem.tag;
            document.getElementById('modal-title').innerText = selectedItem.title;
            document.getElementById('modal-img').src = selectedItem.img;
            document.getElementById('modal-desc').innerText = selectedItem.desc;
            document.getElementById('modal-price').innerText = formatBRL(selectedItem.price);
            document.getElementById('item-modal').classList.remove('hidden');
        }

        document.addEventListener('keydown', event => {
            if (event.key === 'Escape') {
                closeModal('item-modal');
                closeModal('cart-sidebar');
                closeAdminLogin();
                closeModal('admin-panel');
            }
        });

        window.addEventListener('DOMContentLoaded', () => {
            const search = document.getElementById('search-input');
            const sort = document.getElementById('sort-select');
            if (search) search.value = '';
            if (sort) sort.value = 'popular';
            renderTabs();
            renderFeaturedHome();
            renderMenu();
            updateNavigationUI();
            updateCart();
        });
    </script>
</body>
</html>
