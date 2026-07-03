<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cidadania Digital & Combate às Fake News</title>
    <style>
        /* CSS Reset e Configurações Básicas */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary-color: #1e3a8a; /* Azul Escuro (Confiança) */
            --secondary-color: #3b82f6; /* Azul Claro (Ação) */
            --accent-color: #ef4444; /* Vermelho (Alerta) */
            --text-color: #1f2937; /* Cinza Escuro */
            --bg-light: #f3f4f6; /* Fundo Claro */
            --white: #ffffff;
        }

        body {
            color: var(--text-color);
            background-color: var(--bg-light);
            line-height: 1.6;
        }

        /* Barra de Navegação (Header) */
        header {
            background-color: var(--white);
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary-color);
        }
        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }
        .nav-links a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 500;
            transition: color 0.3s;
        }
        .nav-links a:hover {
            color: var(--secondary-color);
        }

        /* Seção Principal (Hero) */
        .hero {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: var(--white);
            padding: 5rem 2rem;
            text-align: center;
        }
        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 1rem;
        }
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto;
            opacity: 0.9;
        }

        /* Conteúdo e Grid do Site */
        .container {
            max-width: 1200px;
            margin: 3rem auto;
            padding: 0 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 2rem;
            color: var(--primary-color);
            margin-bottom: 2rem;
            position: relative;
        }
        .section-title::after {
            content: '';
            display: block;
            width: 50px;
            height: 4px;
            background-color: var(--secondary-color);
            margin: 0.5rem auto 0;
            border-radius: 2px;
        }

        /* Layout de Cards */
        .grid-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }
        .card {
            background-color: var(--white);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0,0,0,0.1);
        }
        .card h3 {
            color: var(--primary-color);
            margin-bottom: 1rem;
        }
        .card.alert h3 {
            color: var(--accent-color);
        }

        /* Guia Prático de Verificação */
        .guide-box {
            background-color: var(--white);
            padding: 3rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            margin-bottom: 4rem;
        }
        .steps {
            margin-top: 1.5rem;
        }
        .step-item {
            display: flex;
            gap: 1rem;
            margin-bottom: 1.5rem;
        }
        .step-number {
            background-color: var(--secondary-color);
            color: var(--white);
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            flex-shrink: 0;
        }

        /* Rodapé */
        footer {
            background-color: #111827;
            color: #9ca3af;
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo">CidadaniaDigital</div>
            <nav>
                <ul class="nav-links">
                    <li><a href="#inicio">Início</a></li>
                    <li><a href="#fake-news">Fake News</a></li>
                    <li><a href="#como-identificar">Como Identificar</a></li>
                    <li><a href="#pilares">Pilares</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <section id="inicio" class="hero">
            <h1>Construindo uma Cidadania Digital Consciente</h1>
            <p>Navegar na internet exige responsabilidade. Aprenda a proteger sua mente e sua comunidade no ambiente online combatendo a desinformação com fatos.</p>
        </section>

        <div class="container">
            
            <section id="fake-news">
                <h2 class="section-title">O Impacto das Fake News</h2>
                <div class="grid-cards">
                    <div class="card alert">
                        <h3>⚠️ O que são?</h3>
                        <p>Fake news são notícias ou informações falsas fabricadas intencionalmente para enganar o público, ganhar visualizações ou manipular opiniões e comportamentos na sociedade.</p>
                    </div>
                    <div class="card">
                        <h3>📢 Velocidade de Propagação</h3>
                        <p>Como costumam apelar para emoções fortes como medo ou indignação, essas histórias falsas se espalham muito mais rápido do que fatos reais e checados.</p>
                    </div>
                    <div class="card">
                        <h3>🛡️ Sua Responsabilidade</h3>
                        <p>Ser um cidadão digital significa romper essa corrente. Compartilhar um boato sem checar prejudica pessoas, afeta a saúde pública e enfraquece a verdade.</p>
                    </div>
                </div>
            </section>

            <section id="como-identificar" class="guide-box">
                <h2 class="section-title">Guia Prático: Como Checar Informações</h2>
                <div class="steps">
                    <div class="step-item">
                        <div class="step-number">1</div>
                        <div>
                            <strong>Avalie a fonte:</strong> O link pertence a um portal de notícias conhecido e confiável? Portais desconhecidos com muitos anúncios saltando na tela exigem atenção dobrada.
                        </div>
                    </div>
                    <div class="step-item">
                        <div class="step-number">2</div>
                        <div>
                            <strong>Não leia apenas o título:</strong> Títulos chamativos e exagerados servem para conseguir cliques. Leia todo o texto e procure os dados reais por trás dele.
                        </div>
                    </div>
                    <div class="step-item">
                        <div class="step-number">3</div>
                        <div>
                            <strong>Pesquise no buscador:</strong> Copie o tema e jogue no Google. Se for um acontecimento real, outros canais de comunicação de grande relevância também estarão noticiando.
                        </div>
                    </div>
                    <div class="step-item">
                        <div class="step-number">4</div>
                        <div>
                            <strong>Use agências de checagem:</strong> Recorra a agências especializadas em desmascarar mentiras virtuais, como o Fato ou Fake, Agência Lupa ou Boatos.org.
                        </div>
                    </div>
                </div>
            </section>

            <section id="pilares">
                <h2 class="section-title">Pilares Essenciais da Cidadania Digital</h2>
                <div class="grid-cards">
                    <div class="card">
                        <h3>🔒 Segurança de Dados</h3>
                        <p>Manter senhas fortes, usar autenticação em duas etapas e nunca compartilhar informações pessoais sensíveis em canais públicos.</p>
                    </div>
                    <div class="card">
                        <h3>🤝 Empatia na Rede</h3>
                        <p>Lembrar que existem pessoas reais do outro lado da tela. Combater o cyberbullying e promover discussões saudáveis e respeitosas.</p>
                    </div>
                    <div class="card">
                        <h3>💡 Senso Crítico</h3>
                        <p>Avaliar com critério o conteúdo que você consome e compartilha, entendendo o papel e a influência dos algoritmos na sua timeline.</p>
                    </div>
                </div>
            </section>

        </div>
    </main>

    <footer>
        <p>&copy; 2026 Portal Cidadania Digital. Desenvolvido para promover uma internet mais segura, ética e consciente.</p>
    </footer>

</body>
</html>