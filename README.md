### 1) Sequência de Fibonacci
Aqui está um programa em Python que verifica se um número pertence à sequência de Fibonacci:

```python
def is_fibonacci(n):
    a, b = 0, 1
    while b <= n:
        if b == n:
            return True
        a, b = b, a + b
    return n == 0

numero = int(input("Informe um número: "))
if is_fibonacci(numero):
    print(f"O número {numero} pertence à sequência de Fibonacci.")
else:
    print(f"O número {numero} não pertence à sequência de Fibonacci.")
```

### 2) Verificar a existência da letra 'a' em uma string
Aqui está um programa em Python que verifica a existência da letra 'a' (maiúscula ou minúscula) em uma string e conta quantas vezes ela ocorre:

```python
def contar_a(texto):
    count = texto.lower().count('a')
    return count

string = input("Informe uma string: ")
ocorrencias = contar_a(string)

if ocorrencias > 0:
    print(f"A letra 'a' aparece {ocorrencias} vezes na string.")
else:
    print("A letra 'a' não aparece na string.")
```

### 3) Valor da variável SOMA ao final do processamento
O trecho de código realiza a soma dos números de 2 até 12 (porque `K` começa em 1 e é incrementado antes da soma).

- Quando `K = 2`, `SOMA = 2`
- Quando `K = 3`, `SOMA = 5`
- E assim por diante até `K = 12`.

A soma total é:
\[ 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9 + 10 + 11 + 12 = 77 \]

Portanto, o valor final de `SOMA` será **77**.

### 4) Descubra a lógica e complete o próximo elemento
a) **1, 3, 5, 7, 9**  
   - Padrão: sequência de números ímpares crescentes.

b) **2, 4, 8, 16, 32, 64, 128**  
   - Padrão: cada número é o dobro do anterior.

c) **0, 1, 4, 9, 16, 25, 36, 49**  
   - Padrão: quadrados perfeitos (0², 1², 2², 3², ...).

d) **4, 16, 36, 64, 100**  
   - Padrão: quadrados perfeitos de números pares (2², 4², 6², 8², 10²).

e) **1, 1, 2, 3, 5, 8, 13**  
   - Padrão: sequência de Fibonacci.

f) **2, 10, 12, 16, 17, 18, 19, 200**  
   - Padrão: números começando com 2 ou que contêm 2.

### 5) Problema dos três interruptores
Para descobrir qual interruptor controla cada lâmpada, você pode seguir os seguintes passos:

1. **Ligue o primeiro interruptor** e deixe ligado por alguns minutos.
2. **Desligue o primeiro interruptor** e ligue o segundo.
3. Vá até a sala das lâmpadas:
   - A lâmpada que está acesa é controlada pelo segundo interruptor.
   - A lâmpada que está apagada mas quente é controlada pelo primeiro interruptor.
   - A lâmpada que está apagada e fria é controlada pelo terceiro interruptor.

Com esses passos, você identifica qual interruptor controla cada lâmpada com apenas uma ida à sala das lâmpadas.
