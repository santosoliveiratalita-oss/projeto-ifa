<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aula: Economia do Paraná</title>
    <style>
        /* Cores Temáticas Baseadas no Paraná */
        :root {
            --azul-escuro: #1A365D;
            --verde-parana: #1E4620;
            --cinza-claro: #F7FAFC;
            --texto: #2D3748;
            --branco: #FFFFFF;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--cinza-claro);
            color: var(--texto);
            line-height: 1.6;
        }

        /* Menu de Navegação */
        header {
            background-color: var(--azul-escuro);
            color: var(--branco);
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo {
            font-size: 1.3rem;
            font-weight: bold;
            letter-spacing: 0.5px;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }

        .nav-links a {
            color: var(--branco);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #63B3ED;
        }

        /* Banner Principal (Hero) */
        .hero {
            background: linear-gradient(135deg, var(--azul-escuro) 0%, var(--verde-parana) 100%);
            color: var(--branco);
            text-align: center;
            padding: 4rem 1rem;
        }

        .hero h1 {
            font-size: 2.3rem;
            margin-bottom: 0.8rem;
        }

        .hero p {
            font-size: 1.1rem;
            max-width: 700px;
            margin: 0 auto 1.5rem auto;
            opacity: 0.9;
        }

        .tag-pib {
            display: inline-block;
            background-color: #ECC94B;
            color: #1A202C;
            padding: 0.4rem 1rem;
            border-radius: 20px;
            font-weight: bold;
            font-size: 0.9rem;
        }

        /* Container de Conteúdo */
        main {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 1.5rem;
        }

        .section-title {
            text-align: center;
            margin: 2.5rem 0 1.5rem 0;
            color: var(--azul-escuro);
            font-size: 1.8rem;
        }

        /* Layout em Grade para os Setores */
        .grid-setores {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .card-setor {
            background: var(--branco);
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            border-top: 5px solid var(--verde-parana);
        }

        .card-setor h3 {
            color: var(--azul-escuro);
            margin-bottom: 0.5rem;
        }

        /* Tabela Resumo dos Dados */
        .tabela-container {
            overflow-x: auto;
            margin: 2rem 0;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: var(--branco);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        th, td {
            padding: 0.8rem 1rem;
            text-align: left;
        }

        th {
            background-color: var(--azul-escuro);
            color: var(--branco);
        }

        tr:nth-child(even) {
            background-color: #EDF2F7;
        }

        /* Rodapé */
        footer {
            background-color: var(--azul-escuro);
            color: var(--branco);
            text-align: center;
            padding: 1.5rem;
            margin-top: 4rem;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- Cabeçalho Administrativo / Menu -->
    <header>
        <nav>
            <div class="logo">Geografia: Economia do PR</div>
            <ul class="nav-links">
                <li><a href="#introducao">Introdução</a></li>
                <li><a href="#setores">Estrutura Produtiva</a></li>
                <li><a href="#dados">Indicadores</a></li>
            </ul>
        </nav>
    </header>

    <!-- Banner Didático -->
    <section class="hero" id="introducao">
        <h1>Material de Apoio: Economia Paranaense</h1>
        <p>Análise da formação do espaço econômico regional, infraestrutura logística e força produtiva do estado.</p>
        <div class="tag-pib">4ª Maior Economia do Brasil</div>
    </section>

    <!-- Conteúdo Principal -->
    <main>
        <!-- Seção Texto Explicativo -->
        <section>
            <h2 class="section-title">Visão Geral</h2>
            <p style="margin-bottom: 1rem; text-align: justify;">
                A estrutura econômica do Paraná caracteriza-se por uma forte integração entre o campo e a cidade. Historicamente moldado por ciclos extrativistas (como a erva-mate e a madeira) e pela expansão cafeeira, o estado transformou seu território em um dos polos produtivos mais competitivos do país.
            </p>
        </section>

        <!-- Seção Grade com os Três Setores -->
        <section id="setores">
            <h2 class="section-title">Estrutura Produtiva Regional</h2>
            <div class="grid-setores">
                <div class="card-setor">
                    <h3>Setor Primário</h3>
                    <p>O agronegócio é o grande pilar do estado, com destaque para a produção intensiva de grãos (soja, milho e trigo) e a forte cadeia de proteína animal (aves e suínos).</p>
                </div>
                <div class="card-setor" style="border-top-color: var(--azul-escuro);">
                    <h3>Setor Secundário</h3>
                    <p>Concentrado no leste e norte do estado, a indústria automobilística, de papel e celulose, metalmecânica e a agroindústria processadora movem a transformação tecnológica.</p>
                </div>
                <div class="card-setor">
                    <h3>Setor Terciário</h3>
                    <p>Representa a maior fatia de ocupação laboral. O comércio de bens e os serviços corporativos são impulsionados por Curitiba e grandes centros de integração regional.</p>
                </div>
            </div>
        </section>

        <!-- Seção de Dados e Indicadores Econômicos -->
        <section id="dados">
            <h2 class="section-title">Indicadores e Logística</h2>
            <div class="tabela-container">
                <table>
                    <thead>
                        <tr>
                            <th>Eixo Estratégico</th>
                            <th>Destaque e Relevância</th>
                            <th>Impacto Econômico</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td><strong>PIB Estadual</strong></td>
                            <td>4ª posição no ranking nacional de riquezas geradas.</td>
                            <td>Representa cerca de 6,1% do PIB do Brasil.</td>
                        </tr>
                        <tr>
                            <td><strong>Porto de Paranaguá</strong></td>
                            <td>Maior porto graneleiro da América Latina.</td>
                            <td>Principal canal de escoamento internacional da produção do Sul do país.</td>
                        </tr>
                        <tr>
                            <td><strong>Mercosul</strong></td>
                            <td>Posicionamento geográfico altamente estratégico.</td>
                            <td>Facilita a conexão física de comércio entre o Brasil, Paraguai e Argentina.</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </section>
    </main>

    <!-- Rodapé da Aula -->
    <footer>
        <p>&copy; 2026 Geografia Econômica - Conteúdo Educativo e Pedagógico.</p>
    </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aula Expandida: Economia do Paraná</title>
    <style>
        :root {
            --azul-escuro: #1A365D;
            --azul-claro: #2B6CB0;
            --verde-parana: #1E4620;
            --verde-destaque: #2F855A;
            --cinza-fundo: #F7FAFC;
            --texto: #2D3748;
            --branco: #FFFFFF;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--cinza-fundo);
            color: var(--texto);
            line-height: 1.6;
        }

        /* Menu de Navegação */
        header {
            background-color: var(--azul-escuro);
            color: var(--branco);
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo {
            font-size: 1.3rem;
            font-weight: bold;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }

        .nav-links a {
            color: var(--branco);
            text-decoration: none;
            font-weight: 500;
            font-size: 0.95rem;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #63B3ED;
        }

        /* Banner Principal (Hero) */
        .hero {
            background: linear-gradient(135deg, var(--azul-escuro) 0%, var(--verde-parana) 100%);
            color: var(--branco);
            text-align: center;
            padding: 5rem 1rem;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem auto;
            opacity: 0.9;
        }

        .tags-container {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
        }

        .badge {
            background-color: #ECC94B;
            color: #1A202C;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-weight: bold;
            font-size: 0.85rem;
        }

        /* Estrutura de Conteúdo */
        main {
            max-width: 1200px;
            margin: 3rem auto;
            padding: 0 1.5rem;
        }

        .section-title {
            text-align: center;
            margin: 3rem 0 1.5rem 0;
            color: var(--azul-escuro);
            font-size: 2rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 50px;
            height: 4px;
            background-color: var(--verde-parana);
            margin: 8px auto 0 auto;
            border-radius: 2px;
        }

        .text-block {
            background: var(--branco);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
            margin-bottom: 2rem;
            text-align: justify;
        }

        .text-block h3 {
            color: var(--azul-claro);
            margin-bottom: 1rem;
        }

        /* Grid de Cards dos Setores */
        .grid-setores {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .card-setor {
            background: var(--branco);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            border-top: 5px solid var(--verde-parana);
        }

        .card-setor h3 {
            color: var(--azul-escuro);
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .card-setor ul {
            margin-top: 1rem;
            padding-left: 1.2rem;
        }

        .card-setor li {
            margin-bottom: 0.5rem;
            font-size: 0.95rem;
        }

        /* Tabelas Informativas */
        .tabela-container {
            overflow-x: auto;
            margin: 2rem 0;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: var(--branco);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        th, td {
            padding: 1rem;
            text-align: left;
        }

        th {
            background-color: var(--azul-escuro);
            color: var(--branco);
        }

        tr:nth-child(even) {
            background-color: #EDF2F7;
        }

        /* Rodapé */
        footer {
            background-color: var(--azul-escuro);
            color: var(--branco);
            text-align: center;
            padding: 2rem;
            margin-top: 5rem;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- Menu Principal -->
    <header>
        <nav>
            <div class="logo">Geografia Prática</div>
            <ul class="nav-links">
                <li><a href="#visao-geral">Visão Geral</a></li>
                <li><a href="#pilares">Três Setores</a></li>
                <li><a href="#infraestrutura">Infraestrutura</a></li>
                <li><a href="#dados-estatisticos">Dados Estatísticos</a></li>
            </ul>
        </nav>
    </header>

    <!-- Banner de Destaques -->
    <section class="hero">
        <h1>A Economia e Força Produtiva do Paraná</h1>
        <p>Um estudo aprofundado sobre um dos estados mais competitivos do Brasil, sua diversificação industrial, potência agrícola e infraestrutura logística regional.</p>
        <div class="tags-container">
            <span class="badge">4ª Maior Economia do Brasil</span>
            <span class="badge">Líder em Cooperativismo</span>
            <span class="badge">Maior Porto Graneleiro da AL</span>
        </div>
    </section>

    <!-- Conteúdo Centralizado -->
    <main>
        
        <!-- Seção 1: Visão Geral -->
        <section id="visao-geral">
            <h2 class="section-title">Visão Geral da Economia</h2>
            <div class="text-block">
                <h3>Formação e Dinâmica Espacial</h3>
                <p>
                    A economia do Estado do Paraná destaca-se nacionalmente pela sua resiliência e alto grau de integração entre a produção do campo e os parques industriais urbanos. Historicamente dependente de ciclos agrícolas únicos (como os da extração de madeira, ciclo da erva-mate e a economia cafeeira), o estado passou por um intenso processo de modernização a partir da segunda metade do século XX. Essa transição consolidou uma economia diversificada, que descentralizou as riquezas e estimulou o crescimento de grandes polos regionais como Londrina, Maringá, Cascavel, Ponta Grossa e a Região Metropolitana de Curitiba.
                </p>
                <br>
                <p>
                    O grande diferencial paranaense está na robustez do seu <strong>sistema cooperativista</strong>. Grandes cooperativas locais organizam pequenos e médios produtores, fornecendo tecnologia de ponta, assistência técnica especializada e capacidade industrial de processamento, transformando matéria-prima bruta em produtos de alto valor agregado exportados para todo o mundo.
                </p>
            </div>
        </section>

        <!-- Seção 2: Os Três Setores -->
        <section id="pilares">
            <h2 class="section-title">A Estrutura dos Três Setores</h2>
            <div class="grid-setores">
                
                <!-- Setor Primário -->
                <div class="card-setor">
                    <h3>Setor Primário (Agro)</h3>
                    <p>O campo é o motor financeiro original do Paraná. Caracteriza-se pelo uso de agricultura de alta precisão e rotação de culturas eficientes.</p>
                    <ul>
                        <li><strong>Grãos:</strong> Liderança nacional na produção combinada de soja, milho e trigo.</li>
                        <li><strong>Proteína Animal:</strong> Maior produtor e exportador de carne de frango do Brasil, além de forte presença na suinocultura.</li>
                        <li><strong>Tecnologia:</strong> Pioneirismo na adoção do sistema de plantio direto na palha.</li>
                    </ul>
                </div>

                <!-- Setor Secundário -->
                <div class="card-setor" style="border-top-color: var(--azul-claro);">
                    <h3>Setor Secundário (Indústria)</h3>
                    <p>A atividade industrial paranaense expandiu-se e deixou de ser apenas processadora de alimentos, abrigando tecnologia complexa.</p>
                    <ul>
                        <li><strong>Automotivo:</strong> Presença de um dos maiores polos automotivos do país na Região Metropolitana de Curitiba.</li>
                        <li><strong>Agroindústria:</strong> Unidades industriais gigantes voltadas ao abate de animais e refino de óleos.</li>
                        <li><strong>Papel e Celulose:</strong> Polo florestal massivo localizado na região centro-oriental do estado.</li>
                    </ul>
                </div>

                <!-- Setor Terciário -->
                <div class="card-setor" style="border-top-color: var(--verde-destaque);">
                    <h3>Setor Terciário (Serviços)</h3>
                    <!DOCTYPE html>
                    <html lang="pt-BR">
                    <head>
                        <meta charset="UTF-8">
                        <meta name="viewport" content="width=device-width, initial-scale=1.0">
                        <title>Aula Interativa: Economia do Paraná</title>
                        <style>
                            :root {
                                --azul-escuro: #1A365D;
                                --azul-claro: #2B6CB0;
                                --verde-parana: #1E4620;
                                --verde-claro: #2F855A;
                                --cinza-fundo: #F7FAFC;
                                --texto: #2D3748;
                                --branco: #FFFFFF;
                            }
                    
                            * {
                                margin: 0;
                                padding: 0;
                                box-sizing: border-box;
                                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
                            }
                    
                            body {
                                background-color: var(--cinza-fundo);
                                color: var(--texto);
                                line-height: 1.6;
                            }
                    
                            /* Menu Superior */
                            header {
                                background-color: var(--azul-escuro);
                                color: var(--branco);
                                padding: 1rem 2rem;
                                position: sticky;
                                top: 0;
                                z-index: 1000;
                                box-shadow: 0 2px 5px rgba(0,0,0,0.1);
                            }
                    
                            nav {
                                display: flex;
                                justify-content: space-between;
                                align-items: center;
                                max-width: 1200px;
                                margin: 0 auto;
                            }
                    
                            .logo {
                                font-size: 1.3rem;
                                font-weight: bold;
                            }
                    
                            /* Banner Principal */
                            .hero {
                                background: linear-gradient(135deg, var(--azul-escuro) 0%, var(--verde-parana) 100%);
                                color: var(--branco);
                                text-align: center;
                                padding: 4rem 1rem;
                            }
                    
                            .hero h1 {
                                font-size: 2.3rem;
                                margin-bottom: 0.8rem;
                            }
                    
                            .hero p {
                                max-width: 800px;
                                margin: 0 auto;
                                opacity: 0.9;
                            }
                    
                            /* Container do Sistema de Abas */
                            main {
                                max-width: 1100px;
                                margin: 3rem auto;
                                padding: 0 1.5rem;
                            }
                    
                            .tabs-nav {
                                display: flex;
                                justify-content: center;
                                gap: 10px;
                                margin-bottom: 2rem;
                                border-bottom: 2px solid #E2E8F0;
                                padding-bottom: 10px;
                                flex-wrap: wrap;
                            }
                    
                            .tab-btn {
                                background: none;
                                border: none;
                                padding: 0.75rem 1.5rem;
                                font-size: 1.1rem;
                                font-weight: 600;
                                color: #718096;
                                cursor: pointer;
                                transition: all 0.3s;
                                border-radius: 5px;
                            }
                    
                            .tab-btn:hover {
                                color: var(--azul-claro);
                                background-color: #EDF2F7;
                            }
                    
                            .tab-btn.active {
                                color: var(--branco);
                                background-color: var(--azul-claro);
                            }
                    
                            /* Conteúdo das Abas */
                            .tab-content {
                                display: none;
                                animation: fadeIn 0.5s ease;
                            }
                    
                            .tab-content.active {
                                display: block;
                            }
                    
                            @keyframes fadeIn {
                                from { opacity: 0; transform: translateY(10px); }
                                to { opacity: 1; transform: translateY(0); }
                            }
                    
                            /* Layout com Imagem e Texto */
                            .flex-container {
                                display: flex;
                                gap: 2rem;
                                align-items: center;
                                background: var(--branco);
                                padding: 2rem;
                                border-radius: 8px;
                                box-shadow: 0 4px 6px rgba(0,0,0,0.05);
                                margin-bottom: 2rem;
                            }
                    
                            @media (max-width: 768px) {
                                .flex-container {
                                    flex-direction: column;
                                }
                            }
                    
                            .info-text {
                                flex: 1;
                            }
                    
                            .info-image {
                                flex: 1;
                                width: 100%;
                                max-height: 300px;
                                object-fit: cover;
                                border-radius: 8px;
                                box-shadow: 0 4px 8px rgba(0,0,0,0.1);
                            }
                    
                            /* Sanfonas Expansíveis (Ver Mais) */
                            accordion-group {
                                display: block;
                                margin-top: 1.5rem;
                            }
                    
                            details {
                                background-color: #EDF2F7;
                                padding: 1rem;
                                border-radius: 6px;
                                margin-bottom: 0.8rem;
                                transition: background 0.3s;
                            }
                    
                            details[open] {
                                background-color: #E2E8F0;
                            }
                    
                            summary {
                                font-weight: bold;
                                color: var(--azul-escuro);
                                cursor: pointer;
                                outline: none;
                                user-select: none;
                            }
                    
                            details p {
                                margin-top: 0.8rem;
                                padding-left: 0.5rem;
                                border-left: 3px solid var(--verde-parana);
                            }
                    
                            /* Rodapé */
                            footer {
                                background-color: var(--azul-escuro);
                                color: var(--branco);
                                text-align: center;
                                padding: 1.5rem;
                                margin-top: 5rem;
                                font-size: 0.85rem;
                            }
                        </style>
                    </head>
                    <body>
                    
                        <header>
                            <nav>
                                <div class="logo">Geografia Interativa</div>
                                <div style="font-size: 0.9rem; opacity: 0.8;">Módulo de Economia Regional</div>
                            </nav>
                        </header>
                    
                        <section class="hero">
                            <h1>Economia do Paraná em Foco</h1>
                            <p>Explore a infraestrutura, a força de produção e as vantagens logísticas do estado de maneira dinâmica.</p>
                        </section>
                    
                        <main>
                            <!-- Navegação das Abas -->
                            <div class="tabs-nav">
                                <button class="tab-btn active" onclick="openTab(event, 'agronegocio')">Agronegócio</button>
                                <button class="tab-btn" onclick="openTab(event, 'logistica')">Logística e Portos</button>
                                <button class="tab-btn" onclick="openTab(event, 'indicadores')">Indicadores Totais</button>
                            </div>
                    
                            <!-- ABA 1: AGRONEGÓCIO -->
                            <div id="agronegocio" class="tab-content active">
                                <div class="flex-container">
                                    <div class="info-text">
                                        <h2>O Motor do Campo Paranaense</h2>
                                        <p>O agronegócio paranaense é altamente competitivo devido ao emprego intensivo de biotecnologia agrícola e à organização dos pequenos produtores por meio de cooperativas funcionais de grande porte.</p>
                                        
                                        <!-- Elementos Expansíveis (Clique para abrir) -->
                                        <accordion-group>
                                            <details>
                                                <summary>🌾 Clique para ver as principais culturas agrícolas</summary>
                                                <p>O Paraná disputa anualmente o topo da produção nacional de grãos, com safras gigantescas de soja, milho e trigo, sendo referência em plantio sustentável.</p>
                                            </details>
                                            <details>
                                                <summary>🍗 Clique para ver a força das proteínas animais</summary>
                                                <p>O estado detém a liderança absoluta no abate de frangos do país, exportando cortes de aves e carne suína para mercados exigentes como Ásia e União Europeia.</p>
                                            </details>
                                        </accordion-group>
                                    </div>
                                    <img src="https://parana.pr.gov.br" alt="Colheita de soja no Paraná" class="info-image">
                                </div>
                            </div>
                    
                            <!-- ABA 2: LOGÍSTICA -->
                            <div id="logistica" class="tab-content">
                                <div class="flex-container">
                                    <div class="info-text">
                                        <h2>Porto de Paranaguá e Conectividade</h2>
                                        <p>O Paraná atua como uma ponte de ligação natural para o Mercosul. O escoamento central da produção é amparado por malhas rodoviárias que convergem ao litoral.</p>
                                        
                                        <accordion-group>
                                            <details>
                                                <summary>⚓ Clique para ver os dados operacionais do Porto</summary>
                                                <p>O complexo portuário opera como o maior polo graneleiro da América Latina. É a principal porta de saída física dos grãos gerados no Centro-Sul brasileiro.</p>
                                            </details>
                                            <details>
                                                <summary>🛣️ Clique para ver o Corredor de Exportação da BR-277</summary>
                                                <p>A rodovia BR-277 corta o estado de leste a oeste, ligando Foz do Iguaçu na fronteira paraguaia diretamente ao porto comercial.</p>
                                            </details>
                                        </accordion-group>
                                    </div>
                                    <img src="https://parana.pr.gov.br" alt="Navios de carga no Porto de Paranaguá" class="info-image">
                                </div>
                            </div>
                    
                            <!-- ABA 3: INDICADORES -->
                            <div id="indicadores" class="tab-content">
                                <div class="flex-container" style="flex-direction: column; align-items: stretch;">
                                    <h2>Resumo Estratégico Socioeconômico</h2>
                                    <p>Clique em cada setor abaixo para abrir a análise e projeções macroeconômicas:</p>
                                    
                                    <details style="background-color: #FFF; border: 1px solid #E2E8F0;">
                                        <summary>📊 Posicionamento no PIB Nacional</summary>
                                        <p>O estado gera cerca de 6,1% de toda a riqueza nacional declarada, o que o consolida firmemente como a 4ª maior economia e um polo financeiro atrativo para novos investimentos industriais.</p>
                                    </details>
                    
                                    <details style="background-color: #FFF; border: 1px solid #E2E8F0;">
                                        <summary>⚡ Matriz Energética Sustentável</summary>
                                        <p>A abundância de recursos hídricos permite que o Paraná concentre plantas geradoras críticas, com destaque para a Usina Hidrelétrica Binacional de Itaipu.</p>
                                    </details>
                                </div>
                    
