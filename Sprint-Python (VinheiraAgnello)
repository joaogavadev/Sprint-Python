import random

sorteio = random.randint(1, 5)

if sorteio == 1:
    nomefunc = "Joao"
elif sorteio == 2:
    nomefunc = "Carlos"
elif sorteio == 3:
    nomefunc = "Felipe"
elif sorteio == 4:
    nomefunc = "Lucas"
else:
    nomefunc = "Pedro"

print(f"Bem-vindo a Vinheria Agnelo. \nO funcionario {nomefunc} vai acompanha-lo nessa compra.")

print("Informe seu nome:")
nome = input()
print("Informe seu cep:")
cep = input()
print("Informe o ano de seu nascimento:")
anonasc = int(input())

idade = 2023 - anonasc
if idade < 18:
    print(f"{nome}, não é permitida a venda para menores de 18 anos.")
    exit()  
else:
    print("Pode continuar com a compra.")

subtotal = total = 0
msgfinal = f"Dados da compra: \nAtendido por {nomefunc}\nCliente: {nome}\nItens da Compra \tValor \tQuantidade \tSubtotal\n"

continua = "sim"

while continua.lower() == "sim":
    print("Escolha um dos vinhos da lista:")
    print("(1) Vinho suave tinto \t R$ 15.00")
    print("(2) Vinho seco tinto \t R$ 25.00")
    print("(3) Vinho branco suave \t R$ 35.00")
    print("(4) Vinho seco branco \t R$ 30.00")
    print("(5) Vinho sem alcool \t R$ 40.00")

    vinho = int(input("Digite o número correspondente ao vinho escolhido: "))
    quantidade = int(input("Digite a quantidade que deseja adquirir deste vinho: "))

    if vinho == 1:
        subtotal = 15 * quantidade
        msgfinal += f"Vinho suave tinto \t R$ 15.00 \t {quantidade} \t R$ {subtotal:.2f}\n"
    elif vinho == 2:
        subtotal = 25 * quantidade
        msgfinal += f"Vinho seco tinto \t R$ 25.00 \t {quantidade} \t R$ {subtotal:.2f}\n"
    elif vinho == 3:
        subtotal = 35 * quantidade
        msgfinal += f"Vinho branco suave \t R$ 35.00 \t {quantidade} \t R$ {subtotal:.2f}\n"
    elif vinho == 4:
        subtotal = 30 * quantidade
        msgfinal += f"Vinho seco branco \t R$ 30.00 \t {quantidade} \t R$ {subtotal:.2f}\n"
    elif vinho == 5:
        subtotal = 40 * quantidade
        msgfinal += f"Vinho sem alcool \t R$ 40.00 \t {quantidade} \t R$ {subtotal:.2f}\n"
    else:
        print("Por favor, escolha uma das opções da lista.")

    total += subtotal

    continua = input("Deseja continuar comprando? (sim ou não): ")

msgfinal += f"Total da compra: R$ {total:.2f}\n"

frete = total / 2

if total < 200:
    msgfinal += "Valor do frete: R$ {:.2f}\n".format(frete)
else:
    msgfinal += "FRETE GRÁTIS!\n"

msgfinal += f"{nome}, foi um prazer atende-lo. Volte em breve!"
print(msgfinal)
