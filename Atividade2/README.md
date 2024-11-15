# Atividades de função em phyton
#1 - Crie uma função para que o usuário digite o seu nome e a sua cidade. O programa deve exibir "Olá, [nome]! Você vive em [cidade].“

def saudacao_usuario():
    nome = input("Digite seu nome: ")
    cidade = input("Digite sua cidade: ")
    print(f"Olá, {nome}! Você vive em {cidade}.")

# Chama a função
saudacao_usuario()

#2 - Crie uma função para que o usuário digite o comprimento e a largura de um retângulo. O programa deve exibir a área e o perímetro do retângulo.

def calcular_area_perimetro():
    # Solicita os valores de comprimento e largura
    comprimento = float(input("Digite o comprimento do retângulo: "))
    largura = float(input("Digite a largura do retângulo: "))
    
    # Calcula a área e o perímetro
    area = comprimento * largura
    perimetro = 2 * (comprimento + largura)
    
    # Exibe os resultados
    print(f"A área do retângulo é: {area}")
    print(f"O perímetro do retângulo é: {perimetro}")

# Chama a função
calcular_area_perimetro()

#3 - Crie uma função para que o usuário digite uma medida em metros. O programa deve converter essa medida para centímetros e milímetros e exibir o resultado.

def converter_medidas():
    # Solicita ao usuário que insira a medida em metros
    metros = float(input("Digite uma medida em metros: "))
    
    # Converte para centímetros e milímetros
    centimetros = metros * 100
    milimetros = metros * 1000
    
    # Exibe os resultados
    print(f"{metros} metros equivale a {centimetros} centímetros e {milimetros} milímetros.")

# Chama a função
converter_medidas()

#4 - Crie uma função para que o usuário digite a largura e a altura de um retângulo. O programa deve calcular e exibir a área do retângulo.base = float(input("Digite o tamanho da base do retangulo (cm):"))

def calcular_area_retangulo():
    # Solicita ao usuário que insira a base e a altura do retângulo
    base = float(input("Digite o tamanho da base do retângulo (cm): "))
    altura = float(input("Digite a altura do retângulo (cm): "))
    
    # Calcula a área do retângulo
    area = base * altura
    
    # Exibe o resultado
    print(f"A área do retângulo é: {area} cm²")

# Chama a função
calcular_area_retangulo()

#5 - Crie uma função para que o usuário digite as idades de duas pessoas. O programa deve exibir se as idades são iguais ou diferentes.

def comparar_idades():
    # Solicita as idades das duas pessoas
    idade1 = int(input("Digite a idade da primeira pessoa: "))
    idade2 = int(input("Digite a idade da segunda pessoa: "))
    
    # Verifica se as idades são iguais ou diferentes
    if idade1 == idade2:
        print("As idades são iguais.")
    else:
        print("As idades são diferentes.")

# Chama a função
comparar_idades()

#6 - Crie uma função para que o usuário digite seu peso (em kg) e sua altura (em metros). O programa deve calcular e exibir o Índice de Massa Corporal (IMC).

def calcular_imc():
    try:
        peso = float(input("Digite seu peso em kg: "))
        altura = float(input("Digite sua altura em metros: "))
        
        if altura <= 0:
            print("A altura deve ser maior que zero.")
            return
        
        imc = peso / (altura ** 2)
        
        print(f"Seu IMC é: {imc:.2f}")
        
        if imc < 18.5:
            print("Classificação: Abaixo do peso")
        elif 18.5 <= imc < 24.9:
            print("Classificação: Peso normal")
        elif 25 <= imc < 29.9:
            print("Classificação: Sobrepeso")
        else:
            print("Classificação: Obesidade")
    
    except ValueError:
        print("Por favor, insira valores numéricos válidos para peso e altura.")

# Executar a função
calcular_imc()

#7 - Crie uma função para que o usuário digite dois números. O programa deve exibir se o primeiro número é maior, menor ou igual ao segundo número.

def comparar_numeros():
    try:
        numero1 = float(input("Digite o primeiro número: "))
        numero2 = float(input("Digite o segundo número: "))
        
        if numero1 > numero2:
            print("O primeiro número é maior que o segundo.")
        elif numero1 < numero2:
            print("O primeiro número é menor que o segundo.")
        else:
            print("Os dois números são iguais.")
    
    except ValueError:
        print("Por favor, insira valores numéricos válidos.")

# Executar a função
comparar_numeros()

#8 - Crie uma função para que o usuário digite três números. O programa deve calcular e exibir a média aritmética desses números.

def calcular_media():
    try:
        numero1 = float(input("Digite o primeiro número: "))
        numero2 = float(input("Digite o segundo número: "))
        numero3 = float(input("Digite o terceiro número: "))
        
        media = (numero1 + numero2 + numero3) / 3
        
        print(f"A média aritmética dos três números é: {media:.2f}")
    
    except ValueError:
        print("Por favor, insira valores numéricos válidos.")

# Executar a função
calcular_media()

#9 - Crie uma função para que o usuário digite o raio e a altura de um cilindro. O programa deve calcular e exibir o volume do cilindro.

import math

def calcular_volume_cilindro():
    try:
        raio = float(input("Digite o raio do cilindro em metros: "))
        altura = float(input("Digite a altura do cilindro em metros: "))
        
        if raio <= 0 or altura <= 0:
            print("O raio e a altura devem ser maiores que zero.")
            return
        
        volume = math.pi * (raio ** 2) * altura
        
        print(f"O volume do cilindro é: {volume:.2f} metros cúbicos")
    
    except ValueError:
        print("Por favor, insira valores numéricos válidos para o raio e a altura.")

# Executar a função
calcular_volume_cilindro()

#10 - Crie uma função para que o usuário digite duas palavras. O programa deve exibir se as palavras são iguais ou diferentes.

def comparar_palavras():
    palavra1 = input("Digite a primeira palavra: ").strip()
    palavra2 = input("Digite a segunda palavra: ").strip()
    
    if palavra1 == palavra2:
        print("As palavras são iguais.")
    else:
        print("As palavras são diferentes.")

# Executar a função
comparar_palavras()

# Funções em phyton 2

#1 - Escreva uma função que receba uma lista de números como entrada e retorne a soma de todos os elementos da lista.

def somar_elementos(lista):
    return sum(lista)

# Exemplo de uso
numeros = [1, 2, 3, 4, 5]
resultado = somar_elementos(numeros)
print(f"A soma dos elementos da lista é: {resultado}")

#2 - Crie uma função que receba uma lista como entrada e retorne a lista invertida, ou seja, a ordem dos elementos deve ser invertida.

def inverter_lista(lista):
    return lista[::-1]

# Exemplo de uso
numeros = [1, 2, 3, 4, 5]
lista_invertida = inverter_lista(numeros)
print(f"A lista invertida é: {lista_invertida}")

#3 - Escreva uma função que receba uma lista de números como entrada e retorne a média dos elementos da lista.

def calcular_media(lista):
    if len(lista) == 0:
        return 0  # Evita divisão por zero caso a lista esteja vazia
    return sum(lista) / len(lista)

# Exemplo de uso
numeros = [1, 2, 3, 4, 5]
media = calcular_media(numeros)
print(f"A média dos elementos da lista é: {media:.2f}")

#4 - Crie uma função que receba uma lista de strings como entrada e retorne a lista contendo o tamanho de cada string.

def tamanho_strings(lista):
    return [len(string) for string in lista]

# Exemplo de uso
palavras = ["maçã", "banana", "abacaxi", "uva"]
tamanhos = tamanho_strings(palavras)
print(f"O tamanho de cada string na lista é: {tamanhos}")

#5 - Escreva uma função que receba duas listas como entrada e retorne uma nova lista contendo apenas os elementos que são comuns a ambas as listas.

def elementos_comuns(lista1, lista2):
    return list(set(lista1) & set(lista2))

# Exemplo de uso
lista_a = [1, 2, 3, 4, 5]
lista_b = [4, 5, 6, 7, 8]
comuns = elementos_comuns(lista_a, lista_b)
print(f"Os elementos comuns entre as duas listas são: {comuns}")

#6 - Crie uma função que receba uma lista como entrada e retorne uma nova lista contendo apenas os elementos únicos (sem repetição) da lista original.

def elementos_unicos(lista):
    return list(set(lista))

# Exemplo de uso
numeros = [1, 2, 3, 2, 4, 5, 5, 6]
unicos = elementos_unicos(numeros)
print(f"Os elementos únicos da lista são: {unicos}")

#7 - Escreva uma função que receba uma lista de números como entrada e retorne uma lista contendo apenas os números pares da lista original.

def numeros_pares(lista):
    return [num for num in lista if num % 2 == 0]

# Exemplo de uso
numeros = [1, 2, 3, 4, 5, 6, 7, 8]
pares = numeros_pares(numeros)
print(f"Os números pares da lista são: {pares}")

#8 - Crie uma função que receba uma lista de números como entrada e retorne o maior elemento da lista.

def maior_elemento(lista):
    if not lista:
        return None  # Retorna None se a lista estiver vazia
    return max(lista)

# Exemplo de uso
numeros = [10, 20, 5, 40, 30]
maior = maior_elemento(numeros)
print(f"O maior elemento da lista é: {maior}")

#9 - Escreva uma função que receba uma lista como entrada e retorne True se a lista estiver ordenada de forma crescente, e False caso contrário.

def lista_ordenada(lista):
    return lista == sorted(lista)

# Exemplo de uso
numeros = [1, 2, 3, 4, 5]
ordenada = lista_ordenada(numeros)
print(f"A lista está ordenada de forma crescente? {ordenada}")

#10 - Crie uma função que receba duas listas como entrada e retorne True se uma lista for subconjunto da outra, e False caso contrário.

def eh_subconjunto(lista1, lista2):
    return set(lista1).issubset(set(lista2)) or set(lista2).issubset(set(lista1))

# Exemplo de uso
lista_a = [1, 2, 3]
lista_b = [1, 2, 3, 4, 5]
subconjunto = eh_subconjunto(lista_a, lista_b)
print(f"Uma lista é subconjunto da outra? {subconjunto}")

# Funções em phyton 3

#1. Crie uma função que receba uma lista de números e retorne uma lista contendo apenas os números ímpares.

def numeros_impares(lista):
    return [num for num in lista if num % 2 != 0]

# Exemplo de uso
numeros = [1, 2, 3, 4, 5, 6, 7, 8]
impares = numeros_impares(numeros)
print(f"Os números ímpares da lista são: {impares}")

#2. Escreva uma função que receba uma lista e retorne uma nova lista com o dobro de cada elemento.

def dobrar_elementos(lista):
    return [num * 2 for num in lista]

# Exemplo de uso
numeros = [1, 2, 3, 4, 5]
dobrados = dobrar_elementos(numeros)
print(f"A nova lista com o dobro de cada elemento é: {dobrados}")

#3. Faça uma função que receba uma lista e retorne uma lista sem duplicatas.

def remover_duplicatas(lista):
    return list(set(lista))

# Exemplo de uso
numeros = [1, 2, 3, 2, 4, 5, 5, 6]
sem_duplicatas = remover_duplicatas(numeros)
print(f"A lista sem duplicatas é: {sem_duplicatas}")

#4. Crie uma função que receba uma lista e um valor divisor e retorne uma lista dos elementos que são divisíveis pelo divisor.

def divisiveis_por(lista, divisor):
    if divisor == 0:
        return []  # Evita divisão por zero
    return [num for num in lista if num % divisor == 0]

# Exemplo de uso
numeros = [10, 15, 20, 25, 30, 35]
divisor = 5
divisiveis = divisiveis_por(numeros, divisor)
print(f"Os números divisíveis por {divisor} são: {divisiveis}")

#5. Escreva uma função que receba duas listas e retorne um conjunto com os elementos que aparecem em ambas.
