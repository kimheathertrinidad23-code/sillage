<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SILLAGE — Botanical & Artisanal Perfumery</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Cormorant Garamond (Editorial Serif) & Plus Jakarta Sans (Clean Sans-Serif) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&family=Plus+Jakarta+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        alabaster: '#FAF9F6',
                        stone: '#F2EFE9',
                        charcoal: '#1C1C1C',
                        muted: '#5E5B57',
                        taupe: '#8C7A6B',
                        taupeLight: '#D8CFC6',
                        borderSubtle: '#E6E2DA'
                    },
                    fontFamily: {
                        serif: ['"Cormorant Garamond"', 'Georgia', 'serif'],
                        sans: ['"Plus Jakarta Sans"', '-apple-system', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom subtle scrollbar & editorial refinements */
        body {
            background-color: #FAF9F6;
            color: #1C1C1C;
            font-family: 'Plus Jakarta Sans', sans-serif;
            -webkit-font-smoothing: antialiased;
        }
        .font-editorial {
            font-family: 'Cormorant Garamond', Georgia, serif;
        }
        /* Smooth fade-in animation for filtered items */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(8px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .animate-fade-in {
            animation: fadeIn 0.45s cubic-bezier(0.16, 1, 0.3, 1) forwards;
        }
        /* Glass bottle reflection shimmer */
        .bottle-glass {
            background: linear-gradient(135deg, rgba(255,255,255,0.65) 0%, rgba(242,239,233,0.3) 50%, rgba(140,122,107,0.08) 100%);
            backdrop-filter: blur(8px);
        }
    </style>
</head>
<body class="bg-alabaster text-charcoal selection:bg-taupe selection:text-alabaster">

    <!-- ================= NAVIGATION BAR ================= -->
    <header class="sticky top-0 z-40 bg-alabaster/90 backdrop-blur-md border-b border-borderSubtle transition-all">
        <div class="max-w-7xl mx-auto px-6 sm:px-10 h-20 flex items-center justify-between">
            <!-- Brand Wordmark -->
            <a href="#" class="font-editorial text-2xl sm:text-3xl tracking-[0.22em] font-medium text-charcoal uppercase">
                Sillage
            </a>

            <!-- Desktop Category Links -->
            <nav class="hidden md:flex items-center space-x-8 text-xs uppercase tracking-[0.16em] text-muted">
                <a href="#collection" onclick="selectGenderCategory('All Perfumes', false)" class="hover:text-charcoal transition-colors">All Perfumes</a>
                <a href="#collection" onclick="selectGenderCategory('For Him', true)" class="hover:text-charcoal transition-colors">For Him</a>
                <a href="#collection" onclick="selectGenderCategory('For Her', true)" class="hover:text-charcoal transition-colors">For Her</a>
            </nav>

            <!-- Action Triggers: Scent Guide & Direct Messenger Contact -->
            <div class="flex items-center space-x-4 sm:space-x-6">
                <button onclick="toggleGuideModal(true)" class="text-xs uppercase tracking-[0.15em] text-muted hover:text-charcoal transition-colors py-2">
                    Scent Guide
                </button>
                <a href="#contact" class="inline-flex items-center space-x-2 border border-charcoal/20 hover:border-charcoal px-4 py-2 rounded-full text-xs uppercase tracking-[0.14em] text-charcoal transition-all">
                    <span>Contact Me</span>
                </a>
            </div>
        </div>
    </header>

    <!-- ================= EDITORIAL HERO SECTION ================= -->
    <section class="relative overflow-hidden border-b border-borderSubtle">
        <div class="max-w-7xl mx-auto px-6 sm:px-10 py-20 sm:py-28 lg:py-32">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-8 items-center">
                
                <!-- Left Editorial Copy -->
                <div class="lg:col-span-7 space-y-8">
                    <div class="inline-flex items-center space-x-3 text-xs uppercase tracking-[0.2em] text-taupe">
                        <span class="w-8 h-[1px] bg-taupe"></span>
                        <span>Curated Fragrance Menu — For Him &amp; For Her</span>
                    </div>
                    
                    <h1 class="font-editorial text-4xl sm:text-6xl lg:text-[4.25rem] leading-[1.08] font-normal text-charcoal">
                        Iconic <br>
                        <span class="italic text-taupe">perfume menu</span> &amp; notes.
                    </h1>
                    
                    <p class="max-w-xl text-sm sm:text-base leading-relaxed text-muted font-light">
                        Explore twelve signature fragrances curated For Him and For Her. Filter by scent character—Woody, Powdery, Citrus, Fresh, Floral, or Amber / Spicy—and inspect the 3-bar intensity rating of every individual note.
                    </p>
                    
                    <div class="pt-2 flex flex-wrap items-center gap-6">
                        <a href="#collection" class="inline-flex items-center justify-center px-8 py-4 bg-charcoal text-alabaster text-xs uppercase tracking-[0.18em] rounded-full hover:bg-taupe transition-colors duration-300">
                            Browse Popular Menu
                        </a>
                        <a href="#contact" class="text-xs uppercase tracking-[0.16em] text-charcoal border-b border-charcoal/30 hover:border-charcoal pb-1 transition-colors">
                            Message Aries Pelo
                        </a>
                    </div>
                </div>
                            <text x="120" y="182" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="6.5" letter-spacing="1.5" fill="#5E5B57" stroke="none">HIM &amp; HER EDIT</text>
                            <text x="120" y="194" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="5.5" letter-spacing="1.2" fill="#8C7A6B" stroke="none">INTENSITY 1 — 5</text>
                            <text x="120" y="206" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-size="5" letter-spacing="1" fill="#5E5B57" stroke="none">50 ML / 100 ML</text>
                        </svg>
                        <span class="mt-3 text-[10px] uppercase tracking-[0.22em] text-taupe">Popular Collection</span>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- ================= PERFUME MENU & PRODUCT SHOWCASE ================= -->
    <main id="collection" class="max-w-7xl mx-auto px-6 sm:px-10 py-20 sm:py-24">
        
        <!-- Section Header & Two-Tier Interactive Filter Controls -->
        <div class="relative pb-10 border-b border-borderSubtle">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-8">
                <div class="space-y-2">
                    <span class="text-xs uppercase tracking-[0.2em] text-taupe">The Popular Menu</span>
                    <h2 class="font-editorial text-3xl sm:text-5xl font-normal text-charcoal">Iconic Fragrances</h2>
                </div>

                <!-- Primary Selection: All / For Him / For Her + Scent Profile Pop-Up Trigger -->
                <div class="flex flex-wrap items-center gap-2.5 sm:gap-3">
                    <div id="gender-tabs" class="inline-flex items-center p-1.5 rounded-full bg-stone/90 border border-borderSubtle" role="tablist" aria-label="Select All Perfumes, For Him, or For Her">
                        <!-- Rendered dynamically via JS -->
                    </div>

                    <!-- Scent Profile Pop-Up Trigger Button -->
                    <button 
                        id="scent-popup-trigger"
                        type="button"
                        onclick="toggleScentPopup()"
                        aria-expanded="false"
                        aria-controls="scent-profile-popup"
                        class="inline-flex items-center space-x-2.5 px-5 py-3 rounded-full border border-charcoal/25 bg-alabaster hover:border-charcoal text-xs uppercase tracking-[0.14em] text-charcoal transition-all shadow-sm"
                    >
                        <svg class="w-3.5 h-3.5 text-taupe" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M3 6h18M7 12h10M10 18h4" />
                        </svg>
                        <span id="scent-trigger-label">Scent Notes: All Scents</span>
                        <svg id="scent-trigger-chevron" class="w-3.5 h-3.5 text-muted transition-transform duration-200" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" />
                        </svg>
                    </button>
                </div>
            </div>

            <!-- Interactive Scent Profile Pop-Up Panel (Woody, Powdery, Citrus, Fresh, Floral, Amber / Spicy) -->
            <div 
                id="scent-profile-popup" 
                class="hidden mt-6 p-6 sm:p-7 rounded-2xl bg-white border border-taupe/40 shadow-[0_18px_45px_rgba(28,28,28,0.08)] animate-fade-in"
                role="region"
                aria-label="Scent Profile Pop-Up Filter"
            >
                <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-3 pb-4 mb-5 border-b border-borderSubtle">
                    <div>
                        <span class="block text-[10px] uppercase tracking-[0.2em] text-taupe font-medium">Olfactory Character Filter</span>
                        <h3 id="scent-popup-heading" class="font-editorial text-2xl text-charcoal">
                            Refine All Perfumes by Scent Note
                        </h3>
                    </div>
                    <div class="flex items-center gap-4">
                        <button 
                            type="button" 
                            onclick="resetAllFilters()" 
                            class="text-[11px] uppercase tracking-[0.14em] text-taupe hover:text-charcoal underline underline-offset-4 transition-colors"
                        >
                            Reset Filters
                        </button>
                        <button 
                            type="button" 
                            onclick="toggleScentPopup(false)" 
                            aria-label="Close scent profile filter"
                            class="w-8 h-8 rounded-full border border-borderSubtle flex items-center justify-center text-muted hover:text-charcoal hover:border-charcoal transition-colors"
                        >
                            &times;
                        </button>
                    </div>
                </div>

                <!-- Scent Profile Pills Grid -->
                <div id="scent-profile-options" class="flex flex-wrap items-center gap-2.5">
                    <!-- Populated dynamically via JS -->
                </div>
            </div>
        </div>

        <!-- Dual Scale Legend Bar (3-Bar Note Strength + 5-Dot Overall Scent Strength) & Filter Summary -->
        <div class="flex flex-col xl:flex-row xl:items-center justify-between py-5 text-xs text-muted border-b border-borderSubtle/60 gap-4">
            <div class="flex flex-wrap items-center gap-x-6 gap-y-2.5">
                <!-- 3-Bar Note Strength Legend -->
                <div class="flex flex-wrap items-center gap-x-3 gap-y-1">
                    <span class="uppercase tracking-[0.14em] text-[10px] text-charcoal font-medium">Note Strength (3-Bar):</span>
                    <span class="inline-flex items-center gap-1.5">
                        <span class="inline-flex items-end gap-0.5 h-2.5">
                            <span class="w-1 h-1.5 rounded-xs bg-taupe"></span>
                            <span class="w-1 h-2 rounded-xs bg-borderSubtle"></span>
                            <span class="w-1 h-2.5 rounded-xs bg-borderSubtle"></span>
                        </span>
                        <span>1 = Mild</span>
                    </span>
                    <span class="inline-flex items-center gap-1.5">
                        <span class="inline-flex items-end gap-0.5 h-2.5">
                            <span class="w-1 h-1.5 rounded-xs bg-taupe"></span>
                            <span class="w-1 h-2 rounded-xs bg-taupe"></span>
                            <span class="w-1 h-2.5 rounded-xs bg-borderSubtle"></span>
                        </span>
                        <span>2 = Moderate</span>
                    </span>
                    <span class="inline-flex items-center gap-1.5">
                        <span class="inline-flex items-end gap-0.5 h-2.5">
                            <span class="w-1 h-1.5 rounded-xs bg-taupe"></span>
                            <span class="w-1 h-2 rounded-xs bg-taupe"></span>
                            <span class="w-1 h-2.5 rounded-xs bg-taupe"></span>
                        </span>
                        <span>3 = Strong</span>
                    </span>
                </div>

                <span class="hidden sm:inline text-borderSubtle">|</span>

                <!-- 5-Dot Overall Scent Strength Legend -->
                <div class="flex flex-wrap items-center gap-x-3 gap-y-1">
                    <span class="uppercase tracking-[0.14em] text-[10px] text-charcoal font-medium">Overall Scent (5-Dot):</span>
                    <span class="inline-flex items-center gap-1.5">
                        <span class="inline-flex gap-1">
                            <span class="w-2 h-2 rounded-full bg-charcoal"></span>
                            <span class="w-2 h-2 rounded-full border border-charcoal/30"></span>
                            <span class="w-2 h-2 rounded-full border border-charcoal/30"></span>
                            <span class="w-2 h-2 rounded-full border border-charcoal/30"></span>
                            <span class="w-2 h-2 rounded-full border border-charcoal/30"></span>
                        </span>
                        <span>1 = Super Mild</span>
                    </span>
                    <span class="inline-flex items-center gap-1.5">
                        <span class="inline-flex gap-1">
                            <span class="w-2 h-2 rounded-full bg-charcoal"></span>
                            <span class="w-2 h-2 rounded-full bg-charcoal"></span>
                            <span class="w-2 h-2 rounded-full bg-charcoal"></span>
                            <span class="w-2 h-2 rounded-full bg-charcoal"></span>
                            <span class="w-2 h-2 rounded-full bg-charcoal"></span>
                        </span>
                        <span>5 = Strongest</span>
                    </span>
                </div>
            </div>

            <div class="flex items-center gap-3 shrink-0">
                <span id="active-filter-summary" class="text-charcoal font-medium">Showing All Perfumes (12 Fragrances)</span>
                <span class="text-borderSubtle">&bull;</span>
                <span>Click card for full pyramid</span>
            </div>
        </div>

        <!-- Product Showcase Grid -->
        <div id="perfume-grid" class="mt-12 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-x-8 gap-y-12">
            <!-- Perfume cards rendered dynamically via JS -->
        </div>

        <!-- Empty State -->
        <div id="empty-filter-state" class="hidden py-20 text-center space-y-4">
            <p class="font-editorial text-3xl text-charcoal">No fragrances match this exact combination.</p>
            <p class="text-xs sm:text-sm text-muted max-w-md mx-auto">Try switching to another olfactory note or view all curated selections.</p>
            <button onclick="resetAllFilters()" class="mt-2 px-6 py-3 rounded-full bg-charcoal text-alabaster text-xs uppercase tracking-[0.16em] hover:bg-taupe transition-colors">
                Show All Perfumes
            </button>
        </div>

    </main>

    <!-- ================= CONTACT ME & FOOTER ================= -->
    <footer id="contact" class="border-t border-borderSubtle bg-stone/60">
        <div class="max-w-7xl mx-auto px-6 sm:px-10 py-20 sm:py-24">
            <div class="max-w-3xl mx-auto text-center space-y-6">
                <span class="inline-block text-xs uppercase tracking-[0.22em] text-taupe">Direct Fragrance Inquiry</span>
                <h2 class="font-editorial text-4xl sm:text-5xl text-charcoal font-normal">
                    Contact Me
                </h2>
                <p class="text-xs sm:text-sm text-muted leading-relaxed max-w-xl mx-auto font-light">
                    Have a question about bottle availability, scent recommendations For Him or For Her, or personalized consultations? Reach out directly to <strong class="font-medium text-charcoal">Aries Pelo</strong> via Facebook Messenger.
                </p>
                <div class="pt-4">
                    <a 
                        href="https://www.facebook.com/ariesgian.pelo.71" 
                        target="_blank" 
                        rel="noopener noreferrer"
                        class="inline-flex items-center justify-center space-x-3 px-8 py-4 rounded-full bg-charcoal text-alabaster text-xs uppercase tracking-[0.18em] hover:bg-taupe transition-colors duration-300 shadow-sm"
                    >
                        <svg class="w-4 h-4 fill-current" viewBox="0 0 24 24" aria-hidden="true">
                            <path d="M12 2C6.477 2 2 6.145 2 11.258c0 2.91 1.453 5.503 3.727 7.197V22l3.405-1.869c.909.252 1.871.387 2.868.387 5.523 0 10-4.145 10-9.258S17.523 2 12 2zm1.006 12.467l-2.547-2.717-4.969 2.717 5.466-5.802 2.609 2.717 4.907-2.717-5.466 5.802z"/>
                        </svg>
                        <span>Message Aries Pelo on Messenger</span>
                    </a>
                </div>
                <p class="text-[11px] text-muted pt-1">
                    Direct Facebook Profile &amp; Messenger: <a href="https://www.facebook.com/ariesgian.pelo.71" target="_blank" rel="noopener noreferrer" class="underline hover:text-charcoal">facebook.com/ariesgian.pelo.71</a>
                </p>
            </div>

            <!-- Minimal Footer Bottom Line -->
            <div class="mt-16 pt-8 border-t border-borderSubtle flex flex-col sm:flex-row items-center justify-between text-xs text-muted gap-4">
                <a href="#" class="font-editorial text-xl tracking-[0.2em] uppercase text-charcoal">Sillage</a>
                <p>&copy; 2026 SILLAGE Fragrance Showcase &mdash; Curated Brochure for Aries Pelo.</p>
            </div>
        </div>
    </footer>

    <!-- ================= FRAGRANCE DETAIL MODAL ================= -->
    <div id="detail-modal" class="fixed inset-0 z-50 hidden items-center justify-center p-4 sm:p-6 bg-charcoal/50 backdrop-blur-sm">
        <div class="bg-alabaster border border-borderSubtle rounded-2xl max-w-2xl w-full max-h-[90vh] overflow-y-auto p-6 sm:p-10 relative shadow-2xl animate-fade-in">
            <button onclick="closeDetailModal()" aria-label="Close modal" class="absolute top-6 right-6 w-9 h-9 rounded-full border border-borderSubtle flex items-center justify-center text-muted hover:text-charcoal hover:border-charcoal transition-colors">
                &times;
            </button>
            <div id="detail-modal-content">
                <!-- Populated dynamically -->
            </div>
        </div>
    </div>

    <!-- ================= SCENT GUIDE MODAL ================= -->
    <div id="guide-modal" class="fixed inset-0 z-50 hidden items-center justify-center p-4 sm:p-6 bg-charcoal/50 backdrop-blur-sm">
        <div class="bg-alabaster border border-borderSubtle rounded-2xl max-w-xl w-full p-8 sm:p-10 relative shadow-2xl animate-fade-in">
            <button onclick="toggleGuideModal(false)" aria-label="Close guide" class="absolute top-6 right-6 w-9 h-9 rounded-full border border-borderSubtle flex items-center justify-center text-muted hover:text-charcoal hover:border-charcoal transition-colors">
                &times;
            </button>
            <span class="text-xs uppercase tracking-[0.2em] text-taupe">Olfactory Architecture</span>
            <h3 class="font-editorial text-3xl text-charcoal mt-1 mb-6">How to Read Our Menu</h3>
            
            <div class="space-y-5 text-sm text-muted leading-relaxed">
                <div>
                    <h4 class="font-editorial text-xl text-charcoal mb-1.5">3-Bar Individual Note Intensity</h4>
                    <p class="text-xs"><strong class="text-charcoal">1/3 Bars (Mild):</strong> Subtle, airy nuance that lends brightness or softness without dominating.</p>
                    <p class="text-xs"><strong class="text-charcoal">2/3 Bars (Moderate):</strong> Balanced, clearly perceptible character that anchors the heart or opening.</p>
                    <p class="text-xs"><strong class="text-charcoal">3/3 Bars (Strong):</strong> Dominant signature note driving the fragrance's identity and trail.</p>
                </div>
                <div class="border-t border-borderSubtle pt-5 space-y-1.5">
                    <h4 class="font-editorial text-xl text-charcoal">5-Dot Overall Scent Strength Scale</h4>
                    <p class="text-xs"><strong class="text-charcoal">1/5 — Super Mild:</strong> Whisper-light skin scent, ideal for warm weather and close quarters.</p>
                    <p class="text-xs"><strong class="text-charcoal">2/5 — Mild / Fresh:</strong> Clean, airy projection with refreshing citrus and floral clarity.</p>
                    <p class="text-xs"><strong class="text-charcoal">3/5 — Balanced / Soft:</strong> Refined, powdery or floral trail with moderate, graceful presence.</p>
                    <p class="text-xs"><strong class="text-charcoal">4/5 — Bold &amp; Distinct:</strong> Noticeable, well-rounded trail lasting through the day and evening.</p>
                    <p class="text-xs"><strong class="text-charcoal">5/5 — Strongest:</strong> Commanding sillage and intense projection engineered for maximum longevity.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- ================= APPLICATION LOGIC ================= -->
    <script>
        // Exact 12 Requested Perfumes: 6 For Him & 6 For Her (Each with 3-Bar Note Ratings & 5-Dot Overall Strength)
        const perfumes = [
            // ==================== FOR HIM (6) ====================
            {
                id: 'dior-sauvage',
                number: '01',
                gender: 'For Him',
                brand: 'Christian Dior',
                name: 'Dior Sauvage',
                scentTags: ['Fresh', 'Citrus', 'Woody'],
                concentration: 'Eau de Parfum',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 135, '100ml': 175 },
                image: 'https://images.unsplash.com/photo-1594035910387-fea47794261f?auto=format&fit=crop&w=900&q=85',
                accentColor: '#1E293B',
                tagline: 'Crisp Calabrian bergamot unleashed over Sichuan pepper and radiant ambroxan.',
                story: 'Inspired by wide-open desert skies at twilight, Dior Sauvage balances juicy, sun-drenched Calabrian bergamot with the crackling warmth of Sichuan pepper and a noble, woody ambroxan trail.',
                notePyramid: [
                    { tier: 'Top', name: 'Calabrian Bergamot', bars: 3, level: 'Strong' },
                    { tier: 'Heart', name: 'Sichuan Pepper', bars: 3, level: 'Strong' },
                    { tier: 'Base', name: 'Ambroxan', bars: 3, level: 'Strong' }
                ],
                mood: 'Magnetic, Crisp & Commanding',
                strength: 5,
                strengthLabel: 'Strongest'
            },
            {
                id: 'bleu-de-chanel',
                number: '02',
                gender: 'For Him',
                brand: 'Chanel',
                name: 'Bleu de Chanel',
                scentTags: ['Woody', 'Citrus', 'Fresh'],
                concentration: 'Eau de Parfum',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 140, '100ml': 180 },
                image: 'https://images.unsplash.com/photo-1523293182086-7651a899d37f?auto=format&fit=crop&w=900&q=85',
                accentColor: '#0F172A',
                tagline: 'Sparkling lemon and grapefruit anchored by aromatic ginger and deep cedar-sandalwood.',
                story: 'A timeless expression of freedom and quiet sophistication. Bleu de Chanel opens with invigorating citrus zest before settling into an opulent, velvety accord of dry cedar and New Caledonian sandalwood.',
                notePyramid: [
                    { tier: 'Top', name: 'Lemon & Grapefruit', bars: 2, level: 'Moderate' },
                    { tier: 'Heart', name: 'Lavender & Ginger', bars: 2, level: 'Moderate' },
                    { tier: 'Base', name: 'Cedar & Sandalwood', bars: 3, level: 'Strong' }
                ],
                mood: 'Refined, Versatile & Timeless',
                strength: 4,
                strengthLabel: 'Bold & Distinct'
            },
            {
                id: 'versace-eros',
                number: '03',
                gender: 'For Him',
                brand: 'Versace',
                name: 'Versace Eros',
                scentTags: ['Fresh', 'Amber / Spicy', 'Woody'],
                concentration: 'Eau de Parfum',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 105, '100ml': 135 },
                image: 'https://images.unsplash.com/photo-1585386959984-a4155224a1ad?auto=format&fit=crop&w=900&q=85',
                accentColor: '#0E7490',
                tagline: 'Vibrant mint leaves and crisp green apple wrapped in creamy Madagascar vanilla.',
                story: 'Luminous freshness meets sensual warmth. Versace Eros opens with an electrifying burst of crushed mint and green apple before unfolding into smooth tonka bean and rich Madagascar vanilla.',
                notePyramid: [
                    { tier: 'Top', name: 'Mint & Green Apple', bars: 3, level: 'Strong' },
                    { tier: 'Heart', name: 'Tonka Bean & Geranium', bars: 3, level: 'Strong' },
                    { tier: 'Base', name: 'Madagascar Vanilla', bars: 3, level: 'Strong' }
                ],
                mood: 'Vibrant, Sensual & Youthful',
                strength: 5,
                strengthLabel: 'Strongest'
            },
            {
                id: 'creed-aventus',
                number: '04',
                gender: 'For Him',
                brand: 'Creed',
                name: 'Creed Aventus',
                scentTags: ['Woody', 'Citrus', 'Fresh'],
                concentration: 'Eau de Parfum',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 365, '100ml': 495 },
                image: 'https://images.unsplash.com/photo-1615634260167-c8cdede054de?auto=format&fit=crop&w=900&q=85',
                accentColor: '#1C1917',
                tagline: 'Sun-ripened pineapple and bergamot over smoky birch wood and rich oakmoss.',
                story: 'Celebrated worldwide as a modern niche benchmark, Creed Aventus blends crisp pineapple and Calabrian bergamot with a dry, smoky heart of birch and oakmoss.',
                notePyramid: [
                    { tier: 'Top', name: 'Bergamot & Pineapple', bars: 3, level: 'Strong' },
                    { tier: 'Heart', name: 'Pink Pepper & Jasmine', bars: 2, level: 'Moderate' },
                    { tier: 'Base', name: 'Smoky Birch & Oakmoss', bars: 3, level: 'Strong' }
                ],
                mood: 'Distinguished, Crisp & Iconic',
                strength: 4,
                strengthLabel: 'Bold & Distinct'
            },
            {
                id: 'paco-rabanne-1-million',
                number: '05',
                gender: 'For Him',
                brand: 'Rabanne',
                name: 'Paco Rabanne 1 Million',
                scentTags: ['Amber / Spicy', 'Woody'],
                concentration: 'Eau de Toilette',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 105, '100ml': 130 },
                image: 'https://images.unsplash.com/photo-1592945403244-b3fbafd7f539?auto=format&fit=crop&w=900&q=85',
                accentColor: '#92400E',
                tagline: 'Blood mandarin layered over woody cinnamon, rose, and burnished leathery amber.',
                story: 'Unapologetically bold and opulent, Paco Rabanne 1 Million pairs sparkling blood mandarin with an intoxicating heart of woody cinnamon and rose over supple leathery amber.',
                notePyramid: [
                    { tier: 'Top', name: 'Blood Mandarin', bars: 2, level: 'Moderate' },
                    { tier: 'Heart', name: 'Woody Cinnamon & Rose', bars: 3, level: 'Strong' },
                    { tier: 'Base', name: 'Leathery Amber', bars: 3, level: 'Strong' }
                ],
                mood: 'Opulent, Warm & Daring',
                strength: 5,
                strengthLabel: 'Strongest'
            },
            {
                id: 'jpg-le-male',
                number: '06',
                gender: 'For Him',
                brand: 'Jean Paul Gaultier',
                name: 'Jean Paul Gaultier Le Male',
                scentTags: ['Powdery', 'Fresh', 'Amber / Spicy'],
                concentration: 'Eau de Toilette',
                sizes: ['75ml', '125ml'],
                prices: { '75ml': 102, '125ml': 132 },
                image: 'https://images.unsplash.com/photo-1587017539504-67cfbddac569?auto=format&fit=crop&w=900&q=85',
                accentColor: '#1D4ED8',
                tagline: 'Crisp mint and barbershop lavender melting into powdery vanilla and warm tonka.',
                story: 'An iconic fougère contrast of cool mint and aromatic lavender against a comforting, powdery embrace of cinnamon, orange blossom, vanilla, and tonka bean.',
                notePyramid: [
                    { tier: 'Top', name: 'Mint & Lavender', bars: 3, level: 'Strong' },
                    { tier: 'Heart', name: 'Cinnamon & Orange Blossom', bars: 2, level: 'Moderate' },
                    { tier: 'Base', name: 'Vanilla & Tonka', bars: 3, level: 'Strong' }
                ],
                mood: 'Comforting, Iconic & Sensual',
                strength: 4,
                strengthLabel: 'Bold & Distinct'
            },

            // ==================== FOR HER (6) ====================
            {
                id: 'chloe-edp',
                number: '07',
                gender: 'For Her',
                brand: 'Chloé',
                name: 'Chloé Eau de Parfum',
                scentTags: ['Floral', 'Powdery', 'Fresh'],
                concentration: 'Eau de Parfum',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 115, '100ml': 150 },
                image: 'https://images.unsplash.com/photo-1588405748880-12d1d2a59f75?auto=format&fit=crop&w=900&q=85',
                accentColor: '#B45309',
                tagline: 'Airy pink peony and lychee unfolding into powdery Damask rose and warm cedarwood.',
                story: 'Effortlessly feminine and luminous, Chloé Eau de Parfum captures a fresh, powdery rose bouquet lifted by delicate lychee and grounded by smooth Virginian cedarwood and amber.',
                notePyramid: [
                    { tier: 'Top', name: 'Peony & Lychee', bars: 2, level: 'Moderate' },
                    { tier: 'Heart', name: 'Damask Rose & Magnolia', bars: 3, level: 'Strong' },
                    { tier: 'Base', name: 'Cedarwood & Amber', bars: 2, level: 'Moderate' }
                ],
                mood: 'Romantic, Powdery & Chic',
                strength: 3,
                strengthLabel: 'Balanced / Soft'
            },
            {
                id: 'pdm-delina',
                number: '08',
                gender: 'For Her',
                brand: 'Parfums de Marly',
                name: 'Parfums de Marly Delina',
                scentTags: ['Floral', 'Powdery', 'Fresh'],
                concentration: 'Eau de Parfum',
                sizes: ['30ml', '75ml'],
                prices: { '30ml': 235, '75ml': 375 },
                image: 'https://images.unsplash.com/photo-1590736969955-71cc94901144?auto=format&fit=crop&w=900&q=85',
                accentColor: '#BE185D',
                tagline: 'Tart lychee and rhubarb draped over opulent Turkish rose, cashmeran, and vanilla.',
                story: 'A modern haute-parfumerie masterpiece sculpted around Turkish rose, sparkling lychee, and crisp rhubarb, wrapped in velvety cashmeran wood and creamy vanilla.',
                notePyramid: [
                    { tier: 'Top', name: 'Lychee & Rhubarb', bars: 3, level: 'Strong' },
                    { tier: 'Heart', name: 'Turkish Rose & Peony', bars: 3, level: 'Strong' },
                    { tier: 'Base', name: 'Cashmeran & Vanilla', bars: 3, level: 'Strong' }
                ],
                mood: 'Opulent, Radiant & Captivating',
                strength: 5,
                strengthLabel: 'Strongest'
            },
            {
                id: 'marc-jacobs-daisy',
                number: '09',
                gender: 'For Her',
                brand: 'Marc Jacobs',
                name: 'Marc Jacobs Daisy',
                scentTags: ['Floral', 'Fresh', 'Citrus'],
                concentration: 'Eau de Toilette',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 104, '100ml': 137 },
                image: 'https://images.unsplash.com/photo-1616949755610-8c9bbc08f138?auto=format&fit=crop&w=900&q=85',
                accentColor: '#CA8A04',
                tagline: 'Sunlit wild strawberry and ruby grapefruit resting on sheer violet leaf and white woods.',
                story: 'Bright, charming, and effortlessly wearable, Marc Jacobs Daisy sparkles with wild berries and fresh violet petals over a whisper-light veil of white woods and soft musk.',
                notePyramid: [
                    { tier: 'Top', name: 'Wild Strawberry & Grapefruit', bars: 2, level: 'Moderate' },
                    { tier: 'Heart', name: 'Violet Leaf & Jasmine', bars: 2, level: 'Moderate' },
                    { tier: 'Base', name: 'White Woods & Musk', bars: 1, level: 'Mild' }
                ],
                mood: 'Sunny, Fresh & Effortless',
                strength: 2,
                strengthLabel: 'Mild / Fresh'
            },
            {
                id: 'lancome-la-vie-est-belle',
                number: '10',
                gender: 'For Her',
                brand: 'Lancôme',
                name: 'Lancôme La Vie Est Belle',
                scentTags: ['Powdery', 'Floral', 'Amber / Spicy'],
                concentration: 'Eau de Parfum',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 122, '100ml': 166 },
                image: 'https://images.unsplash.com/photo-1563170351-be82bc888aa4?auto=format&fit=crop&w=900&q=85',
                accentColor: '#9D174D',
                tagline: 'Noble Iris Pallida and jasmine enveloped in warm spun praline and deep patchouli.',
                story: 'A radiant signature of joy built around the rare powdery elegance of Iris Pallida, brightened by pear and blackcurrant and sweetened with warm praline and Indonesian patchouli.',
                notePyramid: [
                    { tier: 'Top', name: 'Blackcurrant & Pear', bars: 2, level: 'Moderate' },
                    { tier: 'Heart', name: 'Iris Pallida & Jasmine', bars: 3, level: 'Strong' },
                    { tier: 'Base', name: 'Praline & Patchouli', bars: 3, level: 'Strong' }
                ],
                mood: 'Luminous, Velvety & Enveloping',
                strength: 5,
                strengthLabel: 'Strongest'
            },
            {
                id: 'burberry-goddess',
                number: '11',
                gender: 'For Her',
                brand: 'Burberry',
                name: 'Burberry Goddess',
                scentTags: ['Amber / Spicy', 'Powdery'],
                concentration: 'Eau de Parfum',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 135, '100ml': 168 },
                image: 'https://images.unsplash.com/photo-1595425970377-c9703cf48b6d?auto=format&fit=crop&w=900&q=85',
                accentColor: '#A16207',
                tagline: 'A luminous trio of woody vanilla infusion, rich vanilla caviar, and dark vanilla absolute.',
                story: 'Centered on a unique gourmand-aromatic harmony, Burberry Goddess illuminates a triple-vanilla architecture with a crisp opening touch of radiant Provence lavender.',
                notePyramid: [
                    { tier: 'Top', name: 'Vanilla Infusion & Lavender', bars: 2, level: 'Moderate' },
                    { tier: 'Heart', name: 'Vanilla Caviar', bars: 3, level: 'Strong' },
                    { tier: 'Base', name: 'Vanilla Absolute', bars: 3, level: 'Strong' }
                ],
                mood: 'Warm, Golden & Confident',
                strength: 4,
                strengthLabel: 'Bold & Distinct'
            },
            {
                id: 'jo-malone-english-pear',
                number: '12',
                gender: 'For Her',
                brand: 'Jo Malone London',
                name: 'Jo Malone English Pear & Freesia',
                scentTags: ['Fresh', 'Floral', 'Citrus'],
                concentration: 'Cologne',
                sizes: ['50ml', '100ml'],
                prices: { '50ml': 115, '100ml': 165 },
                image: 'https://images.unsplash.com/photo-1541643600914-78b084683601?auto=format&fit=crop&w=900&q=85',
                accentColor: '#78716C',
                tagline: 'Just-ripe King William pear wrapped in cool white freesias and sheer patchouli-amber.',
                story: 'The essence of autumn orchards in soft morning light—delicate, crisp pear nectar meets cool white freesia blossoms over a subtle, understated veil of patchouli and amber.',
                notePyramid: [
                    { tier: 'Top', name: 'King William Pear', bars: 2, level: 'Moderate' },
                    { tier: 'Heart', name: 'White Freesia', bars: 2, level: 'Moderate' },
                    { tier: 'Base', name: 'Patchouli & Amber', bars: 1, level: 'Mild' }
                ],
                mood: 'Delicate, Poetic & Whisper-Light',
                strength: 2,
                strengthLabel: 'Mild / Fresh'
            }
        ];

        // Application State
        let activeGender = 'All Perfumes'; // 'All Perfumes' | 'For Him' | 'For Her'
        let activeScent = 'All Scents';    // 'All Scents' | 'Woody' | 'Fresh' | 'Citrus' | 'Powdery' | 'Floral' | 'Amber / Spicy'
        let isScentPopupOpen = false;

        // Track selected volume per perfume ID (defaults to each perfume's first available size)
        const selectedVolumes = {};
        perfumes.forEach(p => {
            selectedVolumes[p.id] = p.sizes[0];
        });

        const genderCategories = ['All Perfumes', 'For Him', 'For Her'];
        const scentProfiles = [
            { id: 'All Scents', label: 'All Scents', desc: 'Complete spectrum' },
            { id: 'Woody', label: 'Woody', desc: 'Cedar, sandalwood, birch & oakmoss' },
            { id: 'Fresh', label: 'Fresh', desc: 'Crisp pear, mint, lychee & lavender' },
            { id: 'Citrus', label: 'Citrus', desc: 'Bergamot, grapefruit & lemon zest' },
            { id: 'Powdery', label: 'Powdery', desc: 'Iris Pallida, soft rose & vanilla' },
            { id: 'Floral', label: 'Floral', desc: 'Turkish rose, peony, freesia & jasmine' },
            { id: 'Amber / Spicy', label: 'Amber / Spicy', desc: 'Cinnamon, tonka, vanilla caviar & amber' }
        ];

        // Initialize Page
        document.addEventListener('DOMContentLoaded', () => {
            renderGenderTabs();
            renderScentProfileOptions();
            renderPerfumeGrid();
        });

        // Generate an ultra-clean, guaranteed-to-load luxury bottle SVG fallback if any external photo is offline
        function getFallbackBottleSvg(name, brand, accent = '#1C1C1C') {
            const safeName = name.replace(/&/g, '&amp;').replace(/'/g, '&apos;');
            const safeBrand = brand.replace(/&/g, '&amp;').replace(/'/g, '&apos;');
            const svg = `
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 450" width="600" height="450">
                    <defs>
                        <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
                            <stop offset="0%" stop-color="#F6F4EF"/>
                            <stop offset="100%" stop-color="#EAE5DC"/>
                        </linearGradient>
                        <linearGradient id="glass" x1="0" y1="0" x2="1" y2="0">
                            <stop offset="0%" stop-color="#FFFFFF" stop-opacity="0.85"/>
                            <stop offset="50%" stop-color="#FAF9F6" stop-opacity="0.55"/>
                            <stop offset="100%" stop-color="#D8CFC6" stop-opacity="0.65"/>
                        </linearGradient>
                    </defs>
                    <rect width="600" height="450" fill="url(#bg)"/>
                    <ellipse cx="300" cy="392" rx="115" ry="12" fill="#1C1C1C" opacity="0.08"/>
                    <rect x="266" y="76" width="68" height="44" rx="4" fill="${accent}"/>
                    <rect x="278" y="120" width="44" height="14" fill="#8C7A6B" opacity="0.6"/>
                    <rect x="218" y="134" width="164" height="248" rx="14" fill="url(#glass)" stroke="#1C1C1C" stroke-opacity="0.22" stroke-width="1.5"/>
                    <rect x="228" y="144" width="144" height="228" rx="9" fill="none" stroke="#8C7A6B" stroke-opacity="0.35" stroke-width="1"/>
                    <line x1="300" y1="134" x2="300" y2="368" stroke="#8C7A6B" stroke-opacity="0.4" stroke-width="1.2"/>
                    <rect x="242" y="196" width="116" height="128" rx="4" fill="#FAF9F6" stroke="#E6E2DA" stroke-width="1"/>
                    <text x="300" y="226" text-anchor="middle" font-family="Georgia, serif" font-size="11" letter-spacing="2.5" fill="#8C7A6B">${safeBrand.toUpperCase()}</text>
                    <line x1="268" y1="238" x2="332" y2="238" stroke="#D8CFC6" stroke-width="1"/>
                    <text x="300" y="264" text-anchor="middle" font-family="Georgia, serif" font-size="14" fill="#1C1C1C">${safeName}</text>
                    <text x="300" y="298" text-anchor="middle" font-family="sans-serif" font-size="8.5" letter-spacing="2" fill="#5E5B57">SIGNATURE SCENT</text>
                </svg>
            `.trim();
            return 'data:image/svg+xml;charset=UTF-8,' + encodeURIComponent(svg);
        }

        // Render Primary Gender Selection Pills (All Perfumes / For Him / For Her)
        function renderGenderTabs() {
            const container = document.getElementById('gender-tabs');
            container.innerHTML = genderCategories.map(cat => {
                const isActive = activeGender === cat;
                const count = cat === 'All Perfumes'
                    ? perfumes.length
                    : perfumes.filter(p => p.gender === cat).length;

                return `
                    <button 
                        type="button"
                        role="tab"
                        aria-selected="${isActive}"
                        onclick="selectGenderCategory('${cat}', true)"
                        class="px-5 py-2.5 rounded-full text-xs uppercase tracking-[0.15em] transition-all duration-300 flex items-center space-x-2 ${
                            isActive 
                            ? 'bg-charcoal text-alabaster font-medium shadow-sm' 
                            : 'text-muted hover:text-charcoal'
                        }"
                    >
                        <span>${cat}</span>
                        <span class="text-[10px] ${isActive ? 'text-taupeLight' : 'text-muted/70'}">(${count})</span>
                    </button>
                `;
            }).join('');
        }

        // Render Scent Profile Options inside the Pop-Up Panel
        function renderScentProfileOptions() {
            const container = document.getElementById('scent-profile-options');
            container.innerHTML = scentProfiles.map(profile => {
                const isActive = activeScent === profile.id;
                const matchCount = perfumes.filter(p => {
                    const genderMatch = activeGender === 'All Perfumes' || p.gender === activeGender;
                    const scentMatch = profile.id === 'All Scents' || p.scentTags.includes(profile.id);
                    return genderMatch && scentMatch;
                }).length;

                return `
                    <button
                        type="button"
                        onclick="selectScentProfile('${profile.id}')"
                        class="group text-left px-4 py-3 rounded-xl border transition-all duration-200 flex flex-col justify-between min-w-[145px] ${
                            isActive
                            ? 'bg-charcoal text-alabaster border-charcoal shadow-sm'
                            : 'bg-alabaster/70 hover:bg-stone text-charcoal border-borderSubtle hover:border-taupe'
                        }"
                    >
                        <div class="flex items-center justify-between gap-3 w-full">
                            <span class="text-xs uppercase tracking-[0.14em] font-medium">${profile.label}</span>
                            <span class="text-[10px] px-2 py-0.5 rounded-full ${
                                isActive ? 'bg-alabaster/15 text-alabaster' : 'bg-stone text-muted'
                            }">${matchCount}</span>
                        </div>
                        <span class="text-[11px] mt-1 font-light ${isActive ? 'text-taupeLight' : 'text-muted'}">
                            ${profile.desc}
                        </span>
                    </button>
                `;
            }).join('');

            // Update Pop-Up Heading & Trigger Label
            const heading = document.getElementById('scent-popup-heading');
            if (heading) {
                heading.textContent = activeGender === 'All Perfumes'
                    ? 'Refine All Perfumes by Scent Note'
                    : `Refine "${activeGender}" Selection by Scent Note`;
            }

            const triggerLabel = document.getElementById('scent-trigger-label');
            const triggerBtn = document.getElementById('scent-popup-trigger');
            if (triggerLabel && triggerBtn) {
                triggerLabel.textContent = activeScent === 'All Scents' ? 'Scent Notes: All Scents' : `Scent: ${activeScent}`;
                if (activeScent !== 'All Scents') {
                    triggerBtn.classList.add('border-taupe', 'bg-stone/70');
                } else {
                    triggerBtn.classList.remove('border-taupe', 'bg-stone/70');
                }
            }
        }

        // Handle Gender Tab Selection (automatically pops open the scent note filter for For Him / For Her)
        function selectGenderCategory(gender, autoOpenPopup = true) {
            activeGender = gender;
            renderGenderTabs();
            renderScentProfileOptions();
            renderPerfumeGrid();

            if (autoOpenPopup && (gender === 'For Him' || gender === 'For Her')) {
                toggleScentPopup(true);
            }
        }

        // Toggle Scent Profile Pop-Up Panel
        function toggleScentPopup(forceState) {
            const popup = document.getElementById('scent-profile-popup');
            const trigger = document.getElementById('scent-popup-trigger');
            const chevron = document.getElementById('scent-trigger-chevron');

            isScentPopupOpen = typeof forceState === 'boolean' ? forceState : !isScentPopupOpen;

            if (isScentPopupOpen) {
                popup.classList.remove('hidden');
                trigger.setAttribute('aria-expanded', 'true');
                chevron.classList.add('rotate-180');
            } else {
                popup.classList.add('hidden');
                trigger.setAttribute('aria-expanded', 'false');
                chevron.classList.remove('rotate-180');
            }
        }

        // Select Scent Profile from Pop-Up
        function selectScentProfile(scentId) {
            activeScent = scentId;
            renderScentProfileOptions();
            renderPerfumeGrid();
        }

        // Reset All Filters to Default
        function resetAllFilters() {
            activeGender = 'All Perfumes';
            activeScent = 'All Scents';
            renderGenderTabs();
            renderScentProfileOptions();
            renderPerfumeGrid();
        }

        // Update Card Volume Selection
        function selectCardVolume(event, id, volume) {
            event.stopPropagation();
            selectedVolumes[id] = volume;
            renderPerfumeGrid();
        }

        // Render 3-Bar Rating for Each Individual Note (1/3 = Mild, 2/3 = Moderate, 3/3 = Strong)
        function renderNoteThreeBarRating(bars, level) {
            const heights = ['h-2', 'h-2.5', 'h-3.5'];
            const barsHtml = [1, 2, 3].map((step, idx) => {
                const isFilled = step <= bars;
                return `<span class="w-1.5 ${heights[idx]} rounded-xs transition-colors ${
                    isFilled ? 'bg-taupe' : 'bg-borderSubtle'
                }"></span>`;
            }).join('');

            return `
                <div class="inline-flex items-center space-x-2 shrink-0" title="Note Intensity: ${bars}/3 (${level})">
                    <div class="inline-flex items-end space-x-1" aria-hidden="true">
                        ${barsHtml}
                    </div>
                    <span class="text-[10px] uppercase tracking-[0.1em] text-muted w-16 text-right">${bars}/3 ${level}</span>
                </div>
            `;
        }

        // Render 5-Dot Overall Scent Strength Indicator
        function renderStrengthDots(strength, label) {
            const dotsHtml = [1, 2, 3, 4, 5].map(dot => {
                const isFilled = dot <= strength;
                return `<span class="w-2.5 h-2.5 rounded-full transition-colors ${
                    isFilled 
                    ? 'bg-charcoal' 
                    : 'bg-transparent border border-charcoal/30'
                }"></span>`;
            }).join('');

            return `
                <div class="pt-4 mt-4 border-t border-borderSubtle/70 flex items-center justify-between gap-2" aria-label="Overall Scent Strength ${strength} out of 5: ${label}">
                    <span class="uppercase tracking-[0.15em] text-[10px] text-muted font-medium">Overall Strength</span>
                    <div class="flex items-center space-x-2.5">
                        <div class="flex items-center space-x-1.5" role="img" aria-hidden="true">
                            ${dotsHtml}
                        </div>
                        <span class="text-[11px] text-charcoal font-medium whitespace-nowrap">
                            ${strength}/5 &middot; <span class="text-taupe font-normal">${label}</span>
                        </span>
                    </div>
                </div>
            `;
        }

        // Render Perfume Cards Grid
        function renderPerfumeGrid() {
            const grid = document.getElementById('perfume-grid');
            const emptyState = document.getElementById('empty-filter-state');
            const summaryLabel = document.getElementById('active-filter-summary');

            const filtered = perfumes.filter(p => {
                const matchesGender = activeGender === 'All Perfumes' || p.gender === activeGender;
                const matchesScent = activeScent === 'All Scents' || p.scentTags.includes(activeScent);
                return matchesGender && matchesScent;
            });

            // Update Summary Counter
            const scentText = activeScent === 'All Scents' ? '' : ` • ${activeScent}`;
            summaryLabel.textContent = `Showing ${activeGender}${scentText} (${filtered.length} ${filtered.length === 1 ? 'Fragrance' : 'Fragrances'})`;

            if (filtered.length === 0) {
                grid.innerHTML = '';
                emptyState.classList.remove('hidden');
                return;
            } else {
                emptyState.classList.add('hidden');
            }

            grid.innerHTML = filtered.map(perfume => {
                const currentVol = selectedVolumes[perfume.id];
                const currentPrice = perfume.prices[currentVol];
                const fallbackSrc = getFallbackBottleSvg(perfume.name, perfume.brand, perfume.accentColor);

                return `
                <article 
                    onclick="openDetailModal('${perfume.id}')"
                    class="group cursor-pointer bg-white/85 hover:bg-white border border-borderSubtle hover:border-taupe/70 rounded-2xl overflow-hidden transition-all duration-300 flex flex-col justify-between shadow-[0_4px_24px_rgba(28,28,28,0.02)] hover:shadow-[0_14px_38px_rgba(28,28,28,0.07)] animate-fade-in"
                >
                    <div>
                        <!-- Top Perfume Studio Photo with Name Overlaid Directly on Photo -->
                        <div class="relative aspect-[4/3] w-full bg-stone overflow-hidden border-b border-borderSubtle/70">
                            <img 
                                src="${perfume.image}" 
                                alt="${perfume.name} by ${perfume.brand} perfume bottle"
                                loading="lazy"
                                onerror="this.onerror=null; this.src='${fallbackSrc}';"
                                class="w-full h-full object-cover object-center group-hover:scale-105 transition-transform duration-700 ease-out"
                            >
                            <!-- Subtle Editorial Legibility Gradient on Bottom of Photo -->
                            <div class="absolute inset-x-0 bottom-0 h-28 bg-gradient-to-t from-charcoal/85 via-charcoal/40 to-transparent pointer-events-none"></div>

                            <!-- Top Badges (Category & Concentration) -->
                            <div class="absolute top-3.5 left-3.5 right-3.5 flex items-center justify-between gap-2">
                                <span class="px-3 py-1 rounded-full bg-alabaster/92 backdrop-blur-sm text-charcoal text-[10px] uppercase tracking-[0.16em] font-medium shadow-sm">
                                    ${perfume.gender}
                                </span>
                                <span class="px-2.5 py-1 rounded-full bg-charcoal/85 backdrop-blur-sm text-alabaster text-[10px] uppercase tracking-[0.14em]">
                                    ${perfume.concentration}
                                </span>
                            </div>

                            <!-- Perfume Name & House Overlaid Directly on the Perfume Photo -->
                            <div class="absolute bottom-3.5 left-4 right-4 flex items-end justify-between gap-3">
                                <div>
                                    <span class="block text-[9px] uppercase tracking-[0.22em] text-taupeLight font-medium">
                                        ${perfume.brand}
                                    </span>
                                    <h4 class="font-editorial text-xl sm:text-2xl leading-tight text-alabaster drop-shadow-sm">
                                        ${perfume.name}
                                    </h4>
                                </div>
                                <span class="px-2.5 py-1 rounded-full bg-alabaster/95 text-charcoal font-editorial text-lg leading-none shadow-sm">
                                    $${currentPrice}
                                </span>
                            </div>
                        </div>

                        <!-- Card Content Body -->
                        <div class="p-6 sm:p-7">
                            <!-- Scent Character Tags -->
                            <div class="flex flex-wrap items-center gap-1.5 mb-3">
                                ${perfume.scentTags.map(tag => `
                                    <span class="px-2.5 py-0.5 rounded-full bg-stone text-muted text-[10px] uppercase tracking-[0.12em]">
                                        ${tag}
                                    </span>
                                `).join('')}
                            </div>

                            <!-- Perfume Name & Brand Underneath Photo -->
                            <div class="flex items-start justify-between gap-3 mb-2">
                                <div>
                                    <span class="block text-[10px] uppercase tracking-[0.2em] text-taupe font-medium mb-0.5">
                                        ${perfume.brand}
                                    </span>
                                    <h3 class="font-editorial text-2xl sm:text-[1.8rem] leading-tight text-charcoal group-hover:text-taupe transition-colors">
                                        ${perfume.name}
                                    </h3>
                                </div>
                                <span class="font-editorial text-2xl sm:text-[1.7rem] text-charcoal whitespace-nowrap pt-2">
                                    $${currentPrice}
                                </span>
                            </div>

                            <!-- Evocative One-Line Description -->
                            <p class="text-xs sm:text-sm text-muted leading-relaxed font-light mb-5">
                                ${perfume.tagline}
                            </p>

                            <!-- Structured Olfactory Notes with Dedicated 3-Bar Rating Per Note -->
                            <div class="space-y-2.5 pt-4 border-t border-borderSubtle/80 text-xs">
                                <div class="flex items-center justify-between text-[10px] uppercase tracking-[0.16em] text-muted pb-1">
                                    <span>Notes Breakdown</span>
                                    <span>3-Bar Note Strength</span>
                                </div>
                                ${perfume.notePyramid.map(noteItem => `
                                    <div class="flex items-center justify-between gap-2 py-1 border-b border-borderSubtle/40 last:border-b-0">
                                        <div class="min-w-0 pr-2">
                                            <span class="inline-block w-11 uppercase tracking-[0.14em] text-[10px] text-taupe font-medium">${noteItem.tier}</span>
                                            <span class="text-charcoal/95 font-normal">${noteItem.name}</span>
                                        </div>
                                        ${renderNoteThreeBarRating(noteItem.bars, noteItem.level)}
                                    </div>
                                `).join('')}
                            </div>

                            <!-- 5-Dot Overall Scent Strength Indicator -->
                            ${renderStrengthDots(perfume.strength, perfume.strengthLabel)}
                        </div>
                    </div>

                    <!-- Card Footer: Interactive Size Toggle & Brochure Details Trigger -->
                    <div class="px-6 sm:px-7 py-4 bg-stone/35 border-t border-borderSubtle flex flex-wrap items-center justify-between gap-3">
                        <!-- Dynamic Volume Selector Pills per Perfume -->
                        <div class="inline-flex items-center p-1 rounded-full bg-alabaster border border-borderSubtle" onclick="event.stopPropagation()">
                            ${perfume.sizes.map(size => `
                                <button 
                                    type="button"
                                    onclick="selectCardVolume(event, '${perfume.id}', '${size}')"
                                    class="px-3 py-1 rounded-full text-[11px] tracking-[0.1em] transition-all ${
                                        currentVol === size 
                                        ? 'bg-charcoal text-alabaster font-medium' 
                                        : 'text-muted hover:text-charcoal'
                                    }"
                                >
                                    ${size}
                                </button>
                            `).join('')}
                        </div>

                        <!-- Brochure Notes View Indicator -->
                        <span class="text-[11px] uppercase tracking-[0.14em] text-muted group-hover:text-charcoal transition-colors">
                            Full Pyramid &rarr;
                        </span>
                    </div>
                </article>
                `;
            }).join('');
        }

        // Open Full Olfactory Pyramid Detail Modal
        function openDetailModal(id) {
            const perfume = perfumes.find(p => p.id === id);
            if (!perfume) return;

            const currentVol = selectedVolumes[id];
            const price = perfume.prices[currentVol];
            const otherVol = perfume.sizes.find(s => s !== currentVol) || perfume.sizes[0];
            const fallbackSrc = getFallbackBottleSvg(perfume.name, perfume.brand, perfume.accentColor);
            const modalContent = document.getElementById('detail-modal-content');

            modalContent.innerHTML = `
                <div class="space-y-6">
                    <div class="flex flex-col sm:flex-row gap-6 items-start sm:items-center">
                        <div class="relative w-32 h-32 rounded-xl overflow-hidden border border-borderSubtle bg-stone shrink-0">
                            <img 
                                src="${perfume.image}" 
                                alt="${perfume.name} by ${perfume.brand}"
                                onerror="this.onerror=null; this.src='${fallbackSrc}';"
                                class="w-full h-full object-cover"
                            >
                            <div class="absolute inset-x-0 bottom-0 bg-charcoal/80 px-2 py-1 text-center">
                                <span class="block font-editorial text-xs text-alabaster truncate">${perfume.name}</span>
                            </div>
                        </div>
                        <div>
                            <div class="flex flex-wrap items-center gap-2 text-xs uppercase tracking-[0.18em] text-taupe mb-1.5">
                                <span>${perfume.gender}</span>
                                <span>&bull;</span>
                                <span>${perfume.brand}</span>
                                <span>&bull;</span>
                                <span>${perfume.concentration}</span>
                            </div>
                            <h3 class="font-editorial text-3xl sm:text-4xl text-charcoal">${perfume.name}</h3>
                            <p class="text-xs uppercase tracking-[0.16em] text-muted mt-1.5">
                                Profile: ${perfume.scentTags.join(', ')} &mdash; ${perfume.mood}
                            </p>
                        </div>
                    </div>

                    <p class="text-sm text-muted leading-relaxed font-light border-y border-borderSubtle py-5">
                        ${perfume.story}
                    </p>

                    <!-- Full Olfactory Pyramid with 3-Bar Note Strength Gauges -->
                    <div class="space-y-3">
                        <div class="flex items-center justify-between">
                            <h4 class="font-editorial text-2xl text-charcoal">Olfactory Pyramid &amp; Note Strength</h4>
                            <span class="text-[10px] uppercase tracking-[0.16em] text-muted">3-Bar Scale</span>
                        </div>
                        <div class="grid grid-cols-1 sm:grid-cols-3 gap-3">
                            ${perfume.notePyramid.map(noteItem => `
                                <div class="p-4 rounded-xl bg-stone/70 border border-borderSubtle flex flex-col justify-between gap-3">
                                    <div>
                                        <span class="block text-[10px] uppercase tracking-[0.18em] text-taupe mb-1">${noteItem.tier} Note</span>
                                        <p class="text-xs font-medium text-charcoal">${noteItem.name}</p>
                                    </div>
                                    <div class="pt-2 border-t border-borderSubtle/70 flex items-center justify-between">
                                        <div class="inline-flex items-end space-x-1">
                                            ${[1, 2, 3].map((step, idx) => {
                                                const heights = ['h-2', 'h-2.5', 'h-3.5'];
                                                return `<span class="w-1.5 ${heights[idx]} rounded-xs ${step <= noteItem.bars ? 'bg-taupe' : 'bg-borderSubtle'}"></span>`;
                                            }).join('')}
                                        </div>
                                        <span class="text-[10px] uppercase tracking-[0.12em] text-muted">${noteItem.bars}/3 ${noteItem.level}</span>
                                    </div>
                                </div>
                            `).join('')}
                        </div>
                    </div>

                    <!-- 5-Dot Overall Strength Rating in Modal -->
                    <div class="p-4 rounded-xl bg-stone/50 border border-borderSubtle">
                        <div class="flex items-center justify-between">
                            <div>
                                <span class="block text-[10px] uppercase tracking-[0.18em] text-muted mb-1">Overall Scent Intensity Rating</span>
                                <span class="text-xs text-charcoal font-medium">${perfume.strength} out of 5 Dots — ${perfume.strengthLabel}</span>
                            </div>
                            <div class="flex items-center space-x-2">
                                ${[1, 2, 3, 4, 5].map(dot => `
                                    <span class="w-3 h-3 rounded-full ${dot <= perfume.strength ? 'bg-charcoal' : 'border border-charcoal/30'}"></span>
                                `).join('')}
                            </div>
                        </div>
                    </div>

                    <!-- Modal Bottom Bar: Size & Direct Messenger Contact CTA -->
                    <div class="pt-4 border-t border-borderSubtle flex flex-col sm:flex-row sm:items-center justify-between gap-4">
                        <div class="flex items-center space-x-3">
                            <span class="font-editorial text-3xl text-charcoal">$${price}</span>
                            <span class="text-xs text-muted">/ ${currentVol} Flacon</span>
                        </div>
                        <div class="flex flex-wrap items-center gap-3">
                            <button 
                                onclick="switchModalVolume('${perfume.id}', '${otherVol}')"
                                class="px-4 py-3 rounded-full border border-borderSubtle text-xs uppercase tracking-[0.14em] text-muted hover:text-charcoal"
                            >
                                Switch to ${otherVol} ($${perfume.prices[otherVol]})
                            </button>
                            <a 
                                href="https://www.facebook.com/ariesgian.pelo.71"
                                target="_blank"
                                rel="noopener noreferrer"
                                class="inline-flex items-center space-x-2 px-6 py-3 rounded-full bg-charcoal text-alabaster text-xs uppercase tracking-[0.16em] hover:bg-taupe transition-colors"
                            >
                                <svg class="w-3.5 h-3.5 fill-current" viewBox="0 0 24 24" aria-hidden="true">
                                    <path d="M12 2C6.477 2 2 6.145 2 11.258c0 2.91 1.453 5.503 3.727 7.197V22l3.405-1.869c.909.252 1.871.387 2.868.387 5.523 0 10-4.145 10-9.258S17.523 2 12 2zm1.006 12.467l-2.547-2.717-4.969 2.717 5.466-5.802 2.609 2.717 4.907-2.717-5.466 5.802z"/>
                                </svg>
                                <span>Message Aries Pelo on Messenger</span>
                            </a>
                        </div>
                    </div>
                </div>
            `;

            const modal = document.getElementById('detail-modal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function switchModalVolume(id, newVol) {
            selectedVolumes[id] = newVol;
            renderPerfumeGrid();
            openDetailModal(id);
        }

        function closeDetailModal() {
            const modal = document.getElementById('detail-modal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        // Toggle Scent Guide Modal
        function toggleGuideModal(show) {
            const modal = document.getElementById('guide-modal');
            if (show) {
                modal.classList.remove('hidden');
                modal.classList.add('flex');
            } else {
                modal.classList.add('hidden');
                modal.classList.remove('flex');
            }
        }

        // Close modals on backdrop click or Escape key
        window.addEventListener('click', (e) => {
            if (e.target.id === 'detail-modal') closeDetailModal();
            if (e.target.id === 'guide-modal') toggleGuideModal(false);
        });

        window.addEventListener('keydown', (e) => {
            if (e.key === 'Escape') {
                closeDetailModal();
                toggleGuideModal(false);
            }
        });
    </script>
</body>
</html>
