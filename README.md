# Exercicio098.py

from time import sleep

def contador (i, f, p):
    if p < 0:
        p *= -1
    if p == 0:
        p = 1
    print(f'Contador de {i} ate {f} passando {p}')
    sleep(2.5)

    if i < f:
        cont = i
        while cont <= f:
            print(f'{cont}', end=' ',flush=True)
            sleep(0.5)
            cont += p
        print('FIM')

    else:
        cont = i
        while cont >= f:
            print(f'{cont}', end=' ',flush=True)
            sleep(0.5)
            cont -= p
        print('FIM')

#Programa principal
contador(1,10,1)
contador(10,0,2)
print('Agora é sua vez!!!')
print('-='*20)

ini = int(input('Digite o começo:'))
fim = int(input('Digite o fim:'))
pas = int(input('Digite o passo:'))
contador(ini,fim,pas)
