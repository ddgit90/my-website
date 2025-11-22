<！DOCTYPE HTML>
<HTML ラン=「ジャ」>
<頭>
    <メタ 文字セット=「UTF-8」>
    <メタ 名前=「ビューポート」 コンテンツ=「幅=デバイス幅、初期スケール=1。0」>
    <タイトル>レンズとしてのUX | レンズとしてのUX</タイトル>
    <スクリプト src=「https://cdn。tailwindcss。com"」></スクリプト>
    
    <link rel="preconnect" href="https://fonts。googleapis。com">
    <link href="https://fonts。googleapis。com/css2？family=Manrope:wght@300;500;800&family=Shippori+Mincho:wght@400;600&family=Space+Grotesk:wght@300;500;700&display=swap" rel="スタイルシート">
    
    <スクリプト src="https://cdnjs。cloudflare。com/ajax/libs/gsap/3。12。2/gsap。min。js"></script>
    <スクリプト src="https://cdnjs。cloudflare。com/ajax/libs/gsap/3。12。2/ScrollTrigger。min。js"></script>
    <スクリプト src="https://cdn。jsdelivr。net/gh/studio-freight/lenis@1。0。29/bundled/lenis。min。js"></script>

    <スクリプト>
     tailwind。config = {
     テーマ: {
     拡張: {
     フォントファミリー: {
     sans: ['"Manrope"', '"Space Grotesk"', 'sans-serif'],
     セリフ: ['"Shippori Mincho"', 'serif'],
     },
     色: {
     bg: '#EBEAE6',
     テキスト: '#1F1F1F',
     アクセント: '#FF4D00',
                    }
                }
            }
        }
    </スクリプト>

    <スタイル>
     本体 {
     背景色: #EBEAE6;
     色: #1F1F1F;
     オーバーフロー-x: 非表示；
        }

     /* 雑誌風グリド線 */
     。グリッド線 {
     位置: 固定；
     上: 0； 左: 0； 幅: 100%； 高さ: 100%;
     ディスプレイ: フレックス；
     justify-content: スペース間；
     ポインタイベント: なし；
     z インデックス: 0;
     パディング: 0 2rem;
     不透明度: 0。05;
        }
     。line {幅: 1px； 高さ: 100%； 背景色: #000; }

     /* むしろうんざく */
     。カーソル {
     幅: 20px； 高さ: 20px;
     境界線: 1px ソリッド #FF4D00;
     境界半径: 50%;
     位置: 固定；
     ポインタイベント: なし；
     z インデックス: 9999;
     遷移: 変換 0。2 秒、背景色 0。2 秒；
     ミックスブレンドモード: 乗算；
        }
     body。hovering。cursor {
     変換: スケール(3);
     背景色: #FF4D00;
     境界色: 透明；
     不透明度: 0。2;
        }

        /* 画像ホバー */
        .zoom-img-container { overflow: hidden; }
        .zoom-img-container img { transition: transform 1s cubic-bezier(0.2, 1, 0.3, 1); }
        .zoom-img-container:hover img { transform: scale(1.1); }
    </style>
</head>
<body class="cursor-none selection:bg-accent selection:text-white">

    <div class="cursor"></div>
    
    <div class="grid-lines">
        <div class="line"></div><div class="line"></div><div class="line"></div><div class="line"></div>
    </div>

    <nav class="fixed top-0 w-full p-8 flex justify-between items-start z-50 mix-blend-darken">
        <div class="text-sm font-bold tracking-widest uppercase hoverable">My UX Journal.</div>
        <div class="text-xs font-mono text-right hidden md:block">
            ISSUE: 05<br>
            <span class="text-accent">THE INVISIBLE HAND</span>
        </div>
    </nav>

    <main class="relative z-10">

        <section class="min-h-[80vh] flex flex-col justify-center px-8 pt-20 max-w-7xl mx-auto">
            <h1 class="text-[11vw] leading-[0.9] font-bold tracking-tighter uppercase text-reveal">
                It's Not<br>
                Just<br>
                <span class="text-accent ml-[8vw]">Visual.</span>
            </h1>
            <div class="mt-12 max-w-xl ml-auto">
                <p class="text-lg font-serif leading-relaxed">
                    UX（ユーザー体験）とは、<br>
                    「使いやすさ」という魔法をかける論理的思考。<br>
                    私たちが普段、無意識に行っている行動の裏側には、<br>
                    必ず誰かの"設計"が潜んでいる。
                </p>
            </div>
        </section>

        <section class="py-32 px-8 max-w-7xl mx-auto border-t border-black/10">
            <div class="grid md:grid-cols-2 gap-20 items-start relative"> 
                
                <div class="hidden md:block sticky top-24 h-fit">
                    <h2 class="text-6xl font-bold mb-4">The Logic</h2>
                    <div class="w-16 h-1 bg-accent mb-6"></div>
                    <p class="text-sm font-mono text-gray-500 max-w-xs">
                        UXデザインは感覚ではない。<br>
                        認知心理学と人間工学に基づく<br>
                        「おもてなし」の科学だ。
                    </p>
                </div>

                <div class="space-y-32">
                    <article class="group hoverable">
                        <div class="text-accent font-mono text-xs mb-2">01. COGNITIVE LOAD</div>
                        <h3 class="text-3xl font-bold mb-6">脳のメモリを節約する</h3>
                        <p class="text-gray-600 leading-loose font-serif mb-8">
                            人間が一度に覚えられる短期記憶は「マジカルナンバー4（かつては7）」と言われています。
                            良いUXは、ユーザーに「考えさせない」。情報は小出しにし、
                            「次へ」ボタンは最も押しやすい場所に置く。
                            ユーザーの脳のリソースを消費させないことが、最大の敬意なのです。
                        </p>
                    </article>

                    <article class="group hoverable">
                        <div class="text-accent font-mono text-xs mb-2">02. AFFORDANCE</div>
                        <h3 class="text-3xl font-bold mb-6">形が機能を語る</h3>
                        <p class="text-gray-600 leading-loose font-serif mb-8">
                            「アフォーダンス」とは、物が持つ「どう使われるべきか」というメッセージ。
                            平らな板は「押す」、取っ手は「引く」。
                            説明書を読まなくても使えるアプリは、このアフォーダンスが
                            画面の中に完璧に再現されているのです。
                        </p>
                    </article>
                </div>
            </div>
        </section>

        <section class="py-20 bg-white text-black relative overflow-hidden">
            <div class="px-8 max-w-7xl mx-auto">
                <div class="mb-16">
                    <h2 class="text-sm font-bold tracking-widest uppercase text-accent mb-2">UX IN THE WILD</h2>
                    <p class="text-4xl md:text-5xl font-serif">日常に潜む、3つの「設計」</p>
                </div>

                <div class="grid md:grid-cols-3 gap-8">
                    
                    <div class="group hoverable">
                        <div class="zoom-img-container aspect-square bg-gray-100 mb-6 relative">
                            <img src="https://images.unsplash.com/photo-1520699697851-3dc68aa3a474?q=80&w=2154&auto=format&fit=crop" class="w-full h-full object-cover grayscale group-hover:grayscale-0">
                            <div class="absolute top-4 left-4 bg-black text-white text-xs px-2 py-1 font-mono">PHYSICAL UX</div>
                        </div>
                        <h3 class="text-xl font-bold mb-2 group-hover:text-accent transition-colors">The Norman Door</h3>
                        <p class="text-sm text-gray-500 leading-relaxed">
                            「引く」のか「押す」のか分からないドアに出会ったことは？それはあなたが悪いのではなく、デザインの敗北です。平らなプレートなら「押す」、ハンドルなら「引く」。形だけで操作を教える、UXの原点です。
                        </p>
                    </div>

                    <div class="group hoverable">
                        <div class="zoom-img-container aspect-square bg-gray-100 mb-6 relative">
                            <div class="absolute inset-0 bg-neutral-900 flex flex-col gap-4 p-8 justify-center opacity-80">
                                <div class="h-4 bg-white/20 rounded w-3/4 animate-pulse"></div>
                                <div class="h-4 bg-white/20 rounded w-full animate-pulse"></div>
                                <div class="h-4 bg-white/20 rounded w-5/6 animate-pulse"></div>
                            </div>
                            <div class="absolute top-4 left-4 bg-black text-white text-xs px-2 py-1 font-mono">PERCEIVED SPEED</div>
                        </div>
                        <h3 class="text-xl font-bold mb-2 group-hover:text-accent transition-colors">Skeleton Screen</h3>
                        <p class="text-sm text-gray-500 leading-relaxed">
                            YouTubeやInstagramの読み込み中、グルグル回るアイコンではなく「グレーの枠」が表示されませんか？あれは「もうすぐ表示されますよ」という進捗感を与え、体感待ち時間を短くする高度な心理トリックです。
                        </p>
                    </div>

                    <div class="group hoverable">
                        <div class="zoom-img-container aspect-square bg-gray-100 mb-6 relative">
                            <img src="https://images.unsplash.com/photo-1596742578443-7682ef5251cd?q=80&w=2154&auto=format&fit=crop" class="w-full h-full object-cover grayscale group-hover:grayscale-0">
                            <div class="absolute top-4 left-4 bg-black text-white text-xs px-2 py-1 font-mono">INTERACTION</div>
                        </div>
                        <h3 class="text-xl font-bold mb-2 group-hover:text-accent transition-colors">Pull to Refresh</h3>
                        <p class="text-sm text-gray-500 leading-relaxed">
                            画面を下に引っ張って更新。これはスロットマシンのレバーを下げる動作から着想を得ています。「何が出るかな？」という期待感（ドーパミン）を刺激し、ユーザーをアプリに夢中にさせる発明でした。
                        </p>
                    </div>

                </div>
            </div>
        </section>

     <footer class="py-32 px-8 bg-text text-bg">
     <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-end">
     <分割>
     <h2 class="text-5xl md:text-7xl font-bold mb-6 tracking-tighter">テキスト-5xl md:text-7xl font-bold mb-6 tracking-tighter">テキスト-5xl md:text-7xl font-bold mb-6 tracking-tighter。</h2>
     <p class="text-white/60 font-mono text-sm">
     次回あやあやあやあやあやあ。たんんんんんちゃん機会ちょう。
     </p>
     </分割>
     <a href="#" class="mt-12 md:mt-0 px-8 py-4 border border-white/20 rounded-full hover:bg-white hover:text-black transition-colors hoverable">
     ぎょくくくくく
     </a>
     </分割>
     </ガンガン>

    </主要>

    <ココ>
     // 1。ぎょくくょくく
     const lenis = new Lenis({
     期間: 1。2、
     緩和:（t）=> 数学。min(1, 1。001 - 数学。pow(2, -10 * t）),
     ゆうっ:有当、
     });
     関数 raf（時間）{
     カツカ。raf（時間）;
     エ・エ・エ・エ（エ・エ）;
        }
     エ・エ・エ・エ（エ・エ）;

     // 2。GSAP
     gsap。registerPlugin（ScrollTrigger）;

     // ・・・・・公開
     gsap。from(".text-reveal", {
     y: 100、不透明度: 0、持続時間: 1。5、イーズ: 「パワー4。out"、遅延: 0。2
     });

     // 記了・・・・・
     gsap。・・・・・。toArray('記事')。forEach（記事 => {
     gsap。from（記了、{
     むつむつむつ: {
     記事: 記事、
     開始: 「上位85%」、
     },
     y: 30、不透明度: 0、持続時間: 1、ーズ: "power2。外た
     });
     });

     // 3。むちむち
     const = コン。querySelector(".cursor");
     const hoverables = ホバラブル。querySelectorAll(".hoverable");

     ウィンウ。addEventListener("mousemove",（e）=> {
     gsap。to（へ、{
     x: e。10、
     y: e。10、
     持続時間: 0。1、
     むーズ:「ツワー2。外た
     });
     });

     ・・・・・。forEach（el => {
     エル。addEventListener("mouseenter", () => イベントリスナー。体。クススト。add("オ"));
     エル。addEventListener("mouseleave", () => マウスブ。体。クススト。削除("カンカンカン"));
     });
    </やれやれ>
</体>
</HTML>
