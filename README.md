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
    </footer
    
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
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Edição Especial - História de Rio Negro</title>
    <style>
        /* Importando fontes com estilo de imprensa antiga e leitura limpa */
        @import url('https://googleapis.com');

        body {
            background-color: #fcfaf2; /* Tom de papel antigo/jornal */
            font-family: 'Lora', serif;
            color: #1a1a1a;
            margin: 0;
            padding: 20px;
        }

        .newspaper-container {
            max-width: 800px;
            margin: 0 auto;
            background: #fcfaf2;
            padding: 20px;
            border: 1px solid #d2cbb8;
        }

        /* Cabeçalho do Jornal */
        .newspaper-header {
            text-align: center;
            border-bottom: 4px double #1a1a1a;
            padding-bottom: 10px;
            margin-bottom: 20px;
        }

        .newspaper-title {
            font-family: 'Cinzel', serif;
            font-size: 2.8rem;
            margin: 0;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .newspaper-meta {
            display: flex;
            justify-content: space-between;
            font-family: 'Playfair Display', serif;
            font-style: italic;
            border-top: 1px solid #1a1a1a;
            border-bottom: 1px solid #1a1a1a;
            padding: 5px 10px;
            margin-top: 10px;
            font-size: 0.9rem;
        }

        /* Estrutura da Matéria */
        .headline {
            font-family: 'Playfair Display', serif;
            font-size: 2.2rem;
            font-weight: 700;
            text-align: center;
            margin: 25px 0 15px 0;
            line-height: 1.2;
        }

        .subhead {
            font-family: 'Playfair Display', serif;
            font-style: italic;
            font-size: 1.2rem;
            text-align: center;
            color: #444;
            margin-bottom: 25px;
            border-bottom: 1px dashed #bebaa8;
            padding-bottom: 15px;
        }

        /* O segredo do layout de jornal: Múltiplas Colunas */
        .article-columns {
            column-count: 2;
            column-gap: 30px;
            column-rule: 1px solid #bebaa8;
            text-align: justify;
            text-justify: inter-word;
        }

        .article-columns p {
            margin-top: 0;
            margin-bottom: 15px;
            line-height: 1.6;
            font-size: 1.05rem;
            text-indent: 20px; /* Parágrafo recuado clássico */
        }

        /* Letra capitular no primeiro parágrafo */
        .article-columns p.lead {
            text-indent: 0;
        }
        .article-columns p.lead::first-letter {
            font-family: 'Playfair Display', serif;
            font-size: 3.5rem;
            float: left;
            margin-top: 6px;
            margin-right: 8px;
            line-height: 0.8;
            font-weight: bold;
        }

        /* Caixa de Destaque / Entrevista / Citação */
        .pull-quote {
            background-color: #f5f1e3;
            border-top: 2px solid #1a1a1a;
            border-bottom: 2px solid #1a1a1a;
            padding: 15px;
            margin: 20px 0;
            font-family: 'Playfair Display', serif;
            font-style: italic;
            font-size: 1.15rem;
            text-align: center;
            break-inside: avoid; /* Evita que a caixa quebre entre colunas */
        }

        /* Responsividade para telas pequenas */
        @media (max-width: 600px) {
            .article-columns {
                column-count: 1;
            }
            .newspaper-title {
                font-size: 1.8rem;
            }
            .headline {
                font-size: 1.6rem;
            }
        }
    </style>
</head>
<body>

    <div class="newspaper-container">
        <!-- Cabeçalho Cronológico -->
        <header class="newspaper-header">
            <h1 class="newspaper-title">O Rio-Negrense</h1>
            <div class="newspaper-meta">
                <span>Ano CVI • Nº 24.890</span>
                <span>Rio Negro, Paraná</span>
                <span>Edição Histórica</span>
            </div>
        </header>

        <!-- Títulos da Reportagem -->
        <main>
            <h2 class="headline">A Primazia Histórica da Rua Quinze de Novembro</h2>
            <div class="subhead">Como o logradouro de Rio Negro antecipou em quase duas décadas a homenagem à República Brasileira</div>

            <!-- Corpo do Texto em Colunas -->
            <div class="article-columns">
                <p class="lead">
                    Ao caminhar pelo movimentado centro de Rio Negro, o cidadão incauto pode presumir que a principal artéria comercial do município partilha da mesma origem heráldica de tantas outras praças e avenidas espalhadas pelo território nacional. Todavia, a história oculta sob os paralelepípedos da Rua 15 de Novembro revela um pioneirismo cronológico singular.
                </p>

                <p>
                    Diferente dos endereços homônimos que celebram o golpe militar republicano liderado pelo Marechal Deodoro da Fonseca em 1889, o batismo da via rio-negrense deu-se exatos dezenove anos antes do evento nacional. 
                </p>

                <div class="pull-quote">
                    "Enquanto o Brasil ainda vivia sob a égide do Império de Dom Pedro II, as placas rionegrenses já estampavam a icônica data."
                </div>

                <p>
                    Os registros históricos oficiais confirmam que a alteração de nomenclatura ocorreu no ano de 1870. O objetivo da edilidade local era imortalizar o dia 15 de novembro daquele ano, data em que se consolidou a tão almejada emancipação política e administrativa do município de Rio Negro.
                </p>

                <p>
                    Antes de receber a designação que a tornaria famosa, a via era conhecida rudimentarmente como a "Rua do Portão Novo". Sua função primordial era conectar o antigo porto de balsas — que cruzava o impetuoso rio — até a estrada geral que ditava o fluxo de tropeiros e mercadorias na região. 
                </p>
                
                <p>
                    Este resgate documental devolve à municipalidade um orgulho cívico notável: o direito de salvaguardar a primeiríssima Rua 15 de Novembro de toda a história do Brasil.
                </p>
            </div>
        </main>
    </div>

</body>
</html>
# GESTÃO PÚBLICA

## Reportagem Especial: Gestão Pública em Rio Negro-PR
### Análise detalhada sobre os avanços, desafios e as novas estratégias da administração municipal na região.

**Publicado em:** 31 de Agosto de 2026  
**Local:** Rio Negro - PR

---

[Insira o texto dos seus parágrafos aqui...]
# 🗞️ Notícias de Rio Negro — Edição Histórica

Acompanhe as principais crônicas, marcos e memórias que moldaram a história e a identidade do município de Rio Negro, na divisa entre o Paraná e Santa Catarina.

---

## 🏛️ Patrimônio e Memória Cultural

Rio Negro preserva em suas ruas e arquitetura os traços marcantes da colonização europeia e de sua relevância estratégica no Sul do Brasil.

### O Legado da Colonização
A formação da identidade local carrega a forte influência de imigrantes alemães, alemães do Volga, bucovinos, poloneses e italianos. Essa rica mistura cultural reflete-se diretamente até hoje na culinária, nas festividades e nos costumes da população rionegrense.

### Monumentos Históricos e Arquitetura
* **Ponte Metálica Dr. Diniz Assis Henning:** Inaugurada em 1896, é o principal símbolo da união entre Rio Negro (PR) e Mafra (SC).
* **Parque Eco-Turístico São Luís de Tolosa:** Antigo seminário franciscano, o local hoje abriga a prefeitura municipal, uma vasta reserva natural e espaços dedicados à preservação da memória local.

---

## ⏳ Linha do Tempo: Principais Marcos Históricos

1. **1829:** Passagem da expedição que abriu a Estrada da Mata, consolidando o antigo Caminho das Tropas na região.
2. **1870:** Desmembramento de Rio Negro do município de Lapa, marcando sua emancipação política oficial.
3. **1896:** Inauguração da Ponte Metálica, impulsionando o comércio regional e o transporte entre os dois estados.

---

## 📊 Estatísticas e Dados do Município

| Indicador | Descrição |
| :--- | :--- |
| **Localização** | Região Sudeste do Paraná (Divisa PR/SC) |
| **Fundação** | 15 de novembro de 1870 |
| **Principais Atividades** | Agropecuária, Comércio e Indústria de Transformação |

---

*Edição histórica produzida para fins de documentação e preservação da memória pública regional.*
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
import seaborn as sns

# Configuração visual do Seaborn para gráficos elegantes
sns.set_theme(style="whitegrid")
plt.rcParams["figure.figsize"] = (12, 5)

# ==============================================================================
# 1. MODELAGEM DOS DADOS HISTÓRICOS E CONTEMPORÂNEOS
# ==============================================================================

# Dados sobre a transição da população do PR (Urbana vs Rural) - 1960 a 2026
anos = [1960, 1970, 1980, 1991, 2000, 2010, 2026]
pop_urbana = [29.1, 36.2, 58.7, 72.3, 81.2, 85.3, 88.5]  # em %
pop_rural = [100 - x for x in pop_urbana]

df_transicao = pd.DataFrame(
    {"Ano": anos, "Urbana (%)": pop_urbana, "Rural (%)": pop_rural}
)

# Dados dos destinos contemporâneos da emigração paranaense (Principais fluxos)
destinos_migracao = {
    "Destino/Tipo de Fluxo": [
        "São Paulo",
        "Santa Catarina",
        "Mato Grosso / MS",
        "Intra-estadual (Cidades Médias)",
        "Movimento Pendular (Metropolitano)",
    ],
    "Intensidade Estimada (%)": [35, 25, 15, 15, 10],
}
df_destinos = pd.DataFrame(destinos_migracao)

# ==============================================================================
# 2. PLOTAGEM DOS GRÁFICOS
# ==============================================================================

# Gráfico 1: A transição Urbana/Rural decorrente da Reestruturação Produtiva
plt.subplot(1, 2, 1)
plt.plot(
    df_transicao["Ano"],
    df_transicao["Urbana (%)"],
    marker="o",
    linewidth=2.5,
    color="navy",
    label="Urbana",
)
plt.plot(
    df_transicao["Ano"],
    df_transicao["Rural (%)"],
    marker="s",
    linewidth=2.5,
    color="forestgreen",
    label="Rural",
)
plt.title(
    "Transição da População do Paraná\n(Êxodo Rural pós-Mecanização)", fontsize=12
)
plt.xlabel("Ano")
plt.ylabel("Porcentagem (%)")
plt.ylim(0, 100)
plt.legend()

# Gráfico 2: Fluxos e Destinos Contemporâneos da Mobilidade
plt.subplot(1, 2, 2)
sns.barplot(
    x="Intensidade Estimada (%)",
    y="Destino/Tipo de Fluxo",
    data=df_destinos,
    palette="viridis",
    hue="Destino/Tipo de Fluxo",
    legend=False,
)
plt.title("Principais Vetores dos Fluxos Contemporâneos\nda População do PR", fontsize=12)
plt.xlabel("Participação / Peso Estimado (%)")
plt.ylabel("")

# Ajustes finais de layout e exibição
plt.tight_layout()
plt.show()

# ==============================================================================
# 3. RELATÓRIO ANALÍTICO VIA TERMINAL
# ==============================================================================
print("-" * 70)
print("  ANÁLISE SINTÉTICA DA MOBILIDADE HUMANA NO PARANÁ")
print("-" * 70)
print(f"-> Auge do Êxodo Rural: Entre 1970 e 1980 a população urbana saltou de {pop_urbana[1]}% para {pop_urbana[2]}%.")
print(f"-> Cenário Atual (2026): Estabilização urbana em torno de {pop_urbana[-1]}%.")
print("-> Características Contemporâneas:")
print("   1. Desconcentração da capital rumo a polos regionais (Cidades Médias).")
print("   2. Consolidação de Santa Catarina como forte polo de atração.")
print("   3. Pendularidade diária nas Regiões Metropolitanas (Curitiba, Maringá, Londrina).")
print("-" * 70)
