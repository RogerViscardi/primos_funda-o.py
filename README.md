# primos_fundacao.py
Números primos maiores que 86 milhões que aparecem no seriado Fundação 

import math
def eh_primo(n):
    raiz = int(math.sqrt(n))
    for d in range(2, raiz+1 ):
#    for d in range(2, n//2+1 ):
        if n % d == 0:
            return False
    return True

for numero in range(86960947, 86982341):
    if eh_primo(numero):
        print(f'O número {numero} é primo!')
