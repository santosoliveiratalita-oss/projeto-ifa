<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A História dos Tropeiros</title>
    <style>
        :root {
            --primary: #5c3a21;
            --secondary: #d4a373;
            --light: #f4f1de;
            --dark: #2b1d12;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }
        header {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://unsplash.com') no-repeat center center/cover;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }
        header h1 {
            font-size: 3rem;
            margin-bottom: 10px;
        }
        header p {
            font-size: 1.2rem;
            font-style: italic;
        }
        nav {
            background-color: var(--primary);
            position: sticky;
            top: 0;
            z-index: 1000;
            text-align: center;
        }
        nav a {
            display: inline-block;
            color: white;
            padding: 15px 20px;
            text-decoration: none;
            font-weight: bold;
        }
        nav a:hover {
            background-color: var(--secondary);
            color: var(--dark);
        }
        .container {
            max-width: 1000px;
            margin: 40px auto;
            padding: 0 20px;
        }
        section {
            background: white;
            padding: 30px;
            margin-bottom: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        h2 {
            color: var(--primary);
            border-bottom: 2px solid var(--secondary);
            padding-bottom: 10px;
            margin-bottom: 20px;
        }
        ul {
            list-style-position: inside;
            margin-top: 10px;
        }
        li {
            margin-bottom: 8px;
        }
        .highlight-box {
            background-color: #fcf8f2;
            border-left: 5px solid var(--secondary);
            padding: 15px;
            margin: 20px 0;
            font-style: italic;
        }
        footer {
            background-color: var(--dark);
            color: var(--light);
            text-align: center;
            padding: 20px;
            margin-top: 50px;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <header>
        <h1>Os Tropeiros</h1>
        <p>Os desbravadores que conectaram o Brasil colonial a lombo de mula</p>
    </header>

    <nav>
        <a href="#quem-eram">Quem Eram</a>
        <a href="#importancia">Importância Econômica</a>
        <a href="#rotas">Principais Rotas</a>
        <a href="#culinaria">Culinária Tropeira</a>
    </nav>

    <div class="container">
        
        <section id="quem-eram">
            <h2>Quem eram os Tropeiros?</h2>
            <p>Os tropeiros foram condutores de tropas (comitivas de muares, cavalos e gado) que operaram no Brasil a partir do século XVII. Eles viajavam longas distâncias cruzando regiões de difícil acesso para transportar mercadorias, alimentos e animais entre as zonas produtoras e os centros consumidores do país.</p>
            <div class="highlight-box">
                "O tropeirismo foi fundamental para a integração territorial e cultural das regiões Sul, Sudeste e Centro-Oeste do Brasil."
            </div>
        </section>

        <section id="importancia">
            <h2>Importância Econômica e Social</h2>
            <p>Com a descoberta do ouro em Minas Gerais, a demanda por suprimentos e animais de carga disparou. Os tropeiros supriram essa necessidade conectando o Sul (produtor de gado) ao Sudeste minerador.</p>
            <ul>
                <li><strong>Fundação de Cidades:</strong> Os locais de parada das tropas (pousos) deram origem a dezenas de cidades, como Sorocaba, Ponta Grossa e Cruz Alta.</li>
                <li><strong>Comércio Ambulante:</strong> Além de animais, os tropeiros levavam notícias, tecidos, ferramentas e novidades das capitais para o interior.</li>
                <li><strong>Cultura:</strong> Disseminaram costumes, expressões e a música de viola por onde passavam.</li>
            </ul>
        </section>

        <section id="rotas">
            <h2>A Rota de Viamão a Sorocaba</h2>
            <p>A rota mais famosa e importante do tropeirismo era a <strong>Estrada das Tropas</strong>. Ela começava em Viamão (Rio Grande do Sul), cruzava os campos de Santa Catarina e do Paraná, e terminava na grande feira de muares em Sorocaba (São Paulo).</p>
            <p>Nessa feira, milhares de mulas eram comercializadas anualmente para serem utilizadas no transporte de carga nas minas de ouro e, posteriormente, nas plantações de café.</p>
        </section>

        <section id="culinaria">
            <h2>A Herança da Culinária Tropeira</h2>
            <p>A alimentação durante as viagens precisava ser prática, calórica e feita com ingredientes que não estragassem facilmente. Essa necessidade deu origem a pratos tradicionais da gastronomia brasileira:</p>
            <ul>
                <li><strong>Feijão Tropeiro:</strong> Mistura de feijão cozido com farinha de mandioca, torresmo, linguiça, ovos e temperos.</li>
                <li><strong>Arroz de Carreteiro:</strong> Arroz cozido com carne de sol ou charque desfiada, muito prático para se fazer em uma panela só no acampamento.</li>
                <li><strong>Charque:</strong> A carne salgada e seca ao sol era a base de quase todas as refeições por causa de sua longa durabilidade.</li>
            </ul>
        </section>

    </div>

    <footer>
        <p>Site sobre o Tropeirismo criado para o GitHub Pages.</p>
    </footer>

</body>
</html>
def exibir_menu():
    print("\n" + "="*50)
    print("      CONTEÚDO INTERATIVO: GEOGRAFIA DO PARANÁ")
    print("="*50)
    print("1. Visão Geral e Localização")
    print("2. Relevo e as Unidades Morfológicas")
    print("3. Clima e Vegetação")
    print("4. Hidrografia")
    print("5. População e Economia")
    print("6. Sair do programa")
    print("="*50)

def obter_conteudo_geografia():
    # Todo o conteúdo centralizado em uma única estrutura de dados
    return {
        "1": {
            "titulo": "Visão Geral e Localização",
            "texto": (
                "- Área Territorial: Aproximadamente 199.307 km² (2,34% do território nacional).\n"
                "- Localização: Região Sul do Brasil.\n"
                "- Fronteiras: São Paulo (norte/nordeste), Santa Catarina (sul), Oceano Atlântico (leste),\n"
                "             Argentina (sudoeste) e Paraguai (oeste).\n"
                "- Capital: Curitiba (localizada no Primeiro Planalto)."
            )
        },
        "2": {
            "titulo": "Relevo e as Cinco Unidades Morfológicas",
            "texto": (
                "O relevo paranaense desce em degraus de leste para oeste, dividido em:\n"
                "1. Litoral: Planície costeira e baías (Paranaguá e Guaratuba).\n"
                "2. Serra do Mar: Cordilheira que separa o litoral do interior (onde fica o Pico do Paraná, ponto mais alto com ~1.877m).\n"
                "3. Primeiro Planalto (Curitiba): Terreno cristalino, plano e ondulado.\n"
                "4. Segundo Planalto (Ponta Grossa/Campos Gerais): Formado por rochas sedimentares (Escarpa Devoniana).\n"
                "5. Terceiro Planalto (Guarapuava/Maringá/Cascavel): O maior deles, de rochas basálticas, onde a terra roxa propicia a agricultura."
            )
        },
        "3": {
            "titulo": "Clima e Vegetação",
            "texto": (
                "- Clima Predominante: Subtropical úmido (Cfa ao norte/litoral com verões quentes; Cfb ao sul/planalto com verões brandos).\n"
                "- Chuvas: Bem distribuídas ao longo de todo o ano, sem estação seca definida.\n"
                "- Vegetação Original: Composta pela Mata Atlântica na Serra do Mar/Litoral, Mata de Araucárias (Pinheiro-do-Paraná)\n"
                "  nos planaltos mais altos e frios, além de manchas de Campos Limpos no Segundo Planalto."
            )
        },
        "4": {
            "titulo": "Hidrografia",
            "texto": (
                "- Bacia Principal: Cerca de 92% do estado é drenado pela Bacia do Rio Paraná.\n"
                "- Principais Rios: Rio Iguaçu (famoso pelas Cataratas), Rio Paranapanema (divisa com SP), Rio Ivaí e Rio Piquiri.\n"
                "- Direção das Águas: Quase todos os grandes rios correm de leste para oeste, desaguando no Rio Paraná.\n"
                "- Potencial Hidrelétrico: Altíssimo, destacando-se a Usina Binacional de Itaipu."
            )
        },
        "5": {
            "titulo": "População e Economia",
            "texto": (
                "- População: 5º estado mais populoso do Brasil (cerca de 11,4 milhões de habitantes no Censo 2022).\n"
                "- Cidades Principais: Curitiba, Londrina, Maringá, Ponta Grossa, Cascavel e Foz do Iguaçu.\n"
                "- Economia: Uma das maiores do país (5º maior PIB). Destaca-se no setor agropecuário (soja, milho, trigo, aves),\n"
                "  no polo automotivo e industrial de Curitiba/região metropolitana, e no turismo (Foz do Iguaçu).\n"
                "- Logística: Abriga o Porto de Paranaguá, o maior porto graneleiro da América Latina."
            )
        }
    }

def executar_estudo():
    conteudo = obter_conteudo_geografia()
    
    while True:
        exibir_menu()
        opcao = input("Escolha o número do tópico que deseja estudar (1-6): ").strip()
        
        if opcao == "6":
            print("\nObrigado por estudar a Geografia do Paraná! Até logo.")
            break
        elif opcao in conteudo:
            print(f"\n--- {conteudo[opcao]['titulo'].upper()} ---")
            print(conteudo[opcao]['texto'])
            input("\nPressione ENTER para voltar ao menu...")
        else:
            print("\n[Erro] Opção inválida. Digite um número de 1 a 6.")

# Executa a aplicação de estudos
if __name__ == "__main__":
    executar_estudo()
