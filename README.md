# Compra-de-produto
#programa demonstra 4 opções de pagamento de um determinado produto, onde cada opção resulta em uma causa

preço = float(input('insira o valor do produto: '))
print('''1 - à vista (cheque ou dinheiro) 
2 - à vista no cartão 
3 -  2x no cartão 
4 - 3x ou mais no cartão''')

opcao = int(input('qual sua opção: '))

if opcao == 1:
    bonus = (preço)*10/100
    desconto = preço - bonus
    print(f'você obteve 10% de desconto! o valor deu {desconto} reais')

elif opcao == 2:
    bonus = (preço)*5/100
    desconto = preço - bonus
    print(f'você obteve 5% de desconto! O valor deu {desconto} reais')

elif opcao == 3:
    print(f'o preço deu {preço} reais')

elif opcao == 4:
    juros = (preço)*20/100
    total = preço + juros
    totalparc = int(input('quantas pacelas?: '))
    parcela = total / totalparc 
    print(f'com juros de 20% deu {total} com parcelas de {parcela} reais')

