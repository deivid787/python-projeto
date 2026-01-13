import random
def titulo():
   print('='* 30)

#principal

cont= 0
usu = -1

#laço principal
while usu != 0:
 escolha_2 = random.randint(1, 100)
 escolha_3 = random.randint(1, 200)
 #interface
 titulo()
 print(" jogo da adivinhaçao")
 titulo()
 print(
    '[0] para sair\n'
    '[1] para facil \n'
    '[2] para medio\n'
    '[3] para dificil'
 )

 usu = int(input('Escolhe a opçao: '))
 titulo()
 if usu == 1:
   while cont < 15:
      escolha_1= random.randint(1, 50)
      jogador = int(input('escolhe um numero ate 50: '))
      if jogador == escolha_1:
        titulo()
        print(f"O jogador ganhou na tentativa {cont}")
        break
      cont += 1
      print(f'A maquina escolheu {escolha_1} e ganhou !!!!')
 elif usu == 2:
    while cont < 10:
      jogador = int(input('Escolhe um numero de 1 a 100: '))
      if jogador == escolha_2:
        titulo()
        print(f"O jogador ganhou na {cont} tentativa")
        break
      cont += 1
    print(f"A maquina escolheu {escolha_2} e ganhou")
 elif usu == 3:
    while cont < 7:
      jogador = int(input("Escolhe um numero de 1 a 200: "))
      if jogador == escolha_3:
        titulo()
        print(f"O jogador ganhou na tentativa {cont}")
        break
      cont += 1
    print(f"A maquina escolheu {escolha_3} e ganhou")
