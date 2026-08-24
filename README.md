import time

def exibir_introducao():
    print("=" * 60)
    print("       SISTEMA DE EXPLORAÇÃO DA HISTÓRIA DOS TROPEIROS       ")
    print("=" * 60)
    print("Os tropeiros foram condutores de tropas de animais (mulas e cavalos)")
    print("que integraram as regiões sul e sudeste do Brasil entre os séculos")
    print("XVIII e XIX, transportando mercadorias e impulsionando a economia.")
    print("=" * 60 + "\n")

def menu_principal():
    print("[1] O que é o Tropeirismo?")
    print("[2] A Rota Principal (Caminho das Tropas)")
    print("[3] A Culinária Tropeira")
    print("[4] Importância Cultural e Cidades Fundadas")
    print("[5] Sair")
    return input("\nEscolha uma opção para explorar: ")

def o_que_e():
    print("\n--- O QUE FOI O TROPEIRISMO ---")
    print("Surgiu com a necessidade de abastecer a região das minas de ouro em")
    print("Minas Gerais. Como o transporte era difícil, os tropeiros cruzavam")
    print("estados levando gado, alimentos, ferramentas e vestuário no lombo de mulas.")
    print("Eles foram os primeiros 'canais de logística' do Brasil colonial.")

def rota_principal():
    print("\n--- A ROTA PRINCIPAL (CAMINHO DO VIAMÃO) ---")
    print("A rota mais famosa começava em Viamão (RS), passava por Sorocaba (SP)")
    print("- onde ocorriam as grandes feiras de comercialização de animais -")
    print("e seguia até as regiões mineradoras de Minas Gerais.")
    print("\nEstados conectados: RS -> SC -> PR -> SP -> MG")

def culinaria():
    print("\n--- A CULINÁRIA TROPEIRA ---")
    print("Como as viagens duravam meses, os alimentos precisavam ser não perecíveis.")
    print("A base da alimentação era composta por:")
    print("- Feijão (origem do famoso Feijão Tropeiro)")
    print("- Carne seca e toucinho")
    print("- Farinha de mandioca ou de milho")
    print("- Café com rapadura")

def importancia():
    print("\n--- IMPORTÂNCIA E LEGADO ---")
    print("Os locais de pouso dos tropeiros deram origem a dezenas de cidades")
    print("no Sul e Sudeste do Brasil, como Castro (PR), Lapa (PR), Ponta Grossa (PR),")
    print("Lages (SC) e Sorocaba (SP). Deixaram um forte legado na música, vestimenta,")
    print("linguajar e culinária dessas regiões.")

def main():
    exibir_introducao()
    while True:
        opcao = menu_principal()
        
        if opcao == "1":
            o_que_e()
        elif opcao == "2":
            rota_principal()
        elif opcao == "3":
            culinaria()
        elif opcao == "4":
            importancia()
        elif opcao == "5":
            print("\nObrigado por valorizar a história e cultura brasileira! Até logo.")
            break
        else:
            print("\nOpção inválida. Tente novamente.")
        
        print("-" * 60)
        time.sleep(1)

if __name__ == "__main__":
    main()
