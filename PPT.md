# UDACITY
PEDRA PAPEL TESOURA

from random import randint

itens = ['Pedra','Papel','Tesoura']
pc = randint(0,2)
jogador = int(input('''
[0]Pedra
[1]Papel
[2]Tesoura
Escolha ->'''))
print(f'Você escolheu {itens[jogador]} e o Computador escolheu {itens[pc]}')
#Condiçoes para o jogador ganhar do pc
if pc == 0 and jogador == 1:
    print('VOCÊ VENCEU O COMPUTADOR!')
elif pc == 1 and jogador == 2:
    print('VOCÊ VENCEU O COMPUTADOR!')
elif pc == 2 and jogador == 0:
    print('VOCÊ VENCEU O COMPUTADOR!')
#Condiçoes para o jogador perder para o PC
elif jogador == 0 and pc == 1:
    print('O COMPUTADOR VENCEU VOCÊ!')
elif jogador == 1 and pc == 2:
    print('O COMPUTADOR VENCEU VOCÊ!')
elif jogador == 2 and pc == 0:
    print('O COMPUTADOR VENCEU VOCÊ!')
#Condiçoes de empate
elif pc == jogador == 0:
    print('VOCÊ E O COMPUTADOR EMPATARAM!')
elif pc == jogador == 1:
    print('VOCÊ E O COMPUTADOR EMPATARAM!')
elif pc == jogador == 2:
    print('VOCÊ E O COMPUTADOR EMPATARAM!')
