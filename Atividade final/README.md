# Funções Lambda

#1 - Crie uma função Lambda para que o usuário digite o seu nome e a sua cidade. O programa deve exibir "Olá, [nome]! Você vive em [cidade].“

# Função Lambda para saudação
saudar = lambda nome, cidade: f"Olá, {nome}! Você vive em {cidade}."

# Solicitando entrada do usuário
nome = input("Digite seu nome: ")
cidade = input("Digite sua cidade: ")

# Chamando a função e exibindo a mensagem
print(saudar(nome, cidade))

#2 - Crie uma função Lambda para que o usuário digite o comprimento e a largura de um retângulo. O programa deve exibir a área e o perímetro do retângulo.

# Funções Lambda para calcular área e perímetro
calcular_area = lambda comprimento, largura: comprimento * largura
calcular_perimetro = lambda comprimento, largura: 2 * (comprimento + largura)

# Solicitando entradas do usuário
comprimento = float(input("Digite o comprimento do retângulo: "))
largura = float(input("Digite a largura do retângulo: "))

# Calculando e exibindo os resultados
area = calcular_area(comprimento, largura)
perimetro = calcular_perimetro(comprimento, largura)

print(f"A área do retângulo é {area}.")
print(f"O perímetro do retângulo é {perimetro}.")

#3 - Crie uma função Lambda para que o usuário digite uma medida em metros. O programa deve converter essa medida para centímetros e milímetros e exibir o resultado.

# Funções Lambda para conversão
converter_para_cm = lambda metros: metros * 100
converter_para_mm = lambda metros: metros * 1000

# Solicitando entrada do usuário
medida_metros = float(input("Digite uma medida em metros: "))

# Realizando as conversões
medida_cm = converter_para_cm(medida_metros)
medida_mm = converter_para_mm(medida_metros)

# Exibindo os resultados
print(f"{medida_metros} metros equivalem a {medida_cm} centímetros.")
print(f"{medida_metros} metros equivalem a {medida_mm} milímetros.")

#4 - Crie uma função Lambda para que o usuário digite a largura e a altura de um retângulo. O programa deve calcular e exibir a área do retângulo.base = float(input("Digite o tamanho da base do retangulo (cm):"))

# Função Lambda para calcular a área do retângulo
calcular_area = lambda base, altura: base * altura

# Solicitando entrada do usuário
base = float(input("Digite o tamanho da base do retângulo (em cm): "))
altura = float(input("Digite a altura do retângulo (em cm): "))

# Calculando e exibindo o resultado
area = calcular_area(base, altura)
print(f"A área do retângulo é {area} cm².")

#5 - Crie uma função Lambda para que o usuário digite as idades de duas pessoas. O programa deve exibir se as idades são iguais ou diferentes.

# Função Lambda para verificar se as idades são iguais
verificar_idades = lambda idade1, idade2: "As idades são iguais." if idade1 == idade2 else "As idades são diferentes."

# Solicitando entradas do usuário
idade1 = int(input("Digite a idade da primeira pessoa: "))
idade2 = int(input("Digite a idade da segunda pessoa: "))

# Verificando e exibindo o resultado
resultado = verificar_idades(idade1, idade2)
print(resultado)

#6 - Crie uma função Lambda para que o usuário digite seu peso (em kg) e sua altura (em metros). O programa deve calcular e exibir o Índice de Massa Corporal (IMC).

# Função Lambda para calcular o IMC
calcular_imc = lambda peso, altura: peso / (altura ** 2)

# Solicitando entradas do usuário
peso = float(input("Digite seu peso (em kg): "))
altura = float(input("Digite sua altura (em metros): "))

# Calculando e exibindo o IMC
imc = calcular_imc(peso, altura)
print(f"Seu Índice de Massa Corporal (IMC) é {imc:.2f}.")

#7 - Crie uma função Lambda para que o usuário digite dois números. O programa deve exibir se o primeiro número é maior, menor ou igual ao segundo número.

# Função Lambda para comparar dois números
comparar_numeros = lambda num1, num2: (
    "O primeiro número é maior." if num1 > num2 else
    "O primeiro número é menor." if num1 < num2 else
    "Os dois números são iguais."
)

# Solicitando entradas do usuário
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

# Comparando e exibindo o resultado
resultado = comparar_numeros(num1, num2)
print(resultado)

#8 - Crie uma função Lambda para que o usuário digite três números. O programa deve calcular e exibir a média aritmética desses números.

# Função Lambda para calcular a média aritmética
calcular_media = lambda num1, num2, num3: (num1 + num2 + num3) / 3

# Solicitando entradas do usuário
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))
num3 = float(input("Digite o terceiro número: "))

# Calculando e exibindo a média
media = calcular_media(num1, num2, num3)
print(f"A média aritmética dos números é {media:.2f}.")

#9 - Crie uma função Lambda para que o usuário digite o raio e a altura de um cilindro. O programa deve calcular e exibir o volume do cilindro.

import math

# Função Lambda para calcular o volume do cilindro
calcular_volume = lambda raio, altura: math.pi * (raio ** 2) * altura

# Solicitando entradas do usuário
raio = float(input("Digite o raio do cilindro (em metros): "))
altura = float(input("Digite a altura do cilindro (em metros): "))

# Calculando e exibindo o volume
volume = calcular_volume(raio, altura)
print(f"O volume do cilindro é {volume:.2f} metros cúbicos.")

#10 - Crie uma função Lambda para que o usuário digite duas palavras. O programa deve exibir se as palavras são iguais ou diferentes.

# Função Lambda para comparar duas palavras
comparar_palavras = lambda palavra1, palavra2: "As palavras são iguais." if palavra1 == palavra2 else "As palavras são diferentes."

# Solicitando entradas do usuário
palavra1 = input("Digite a primeira palavra: ")
palavra2 = input("Digite a segunda palavra: ")

# Comparando e exibindo o resultado
resultado = comparar_palavras(palavra1, palavra2)
print(resultado)

# Funções Lambda, parte 2

#1 Dada uma lista de números inteiros, use uma função lambda para retornar uma lista com o quadrado de cada número.

# Lista de números inteiros
numeros = [1, 2, 3, 4, 5]

# Função Lambda para calcular o quadrado de cada número
quadrados = list(map(lambda x: x ** 2, numeros))

# Exibindo os resultados
print(f"Quadrados dos números: {quadrados}")

#2 Dada uma lista de temperaturas em Celsius, use uma função lambda para convertê-las em Fahrenheit.

# Lista de temperaturas em Celsius
temperaturas_celsius = [0, 10, 20, 30, 40, 50]

# Função Lambda para converter Celsius para Fahrenheit
temperaturas_fahrenheit = list(map(lambda celsius: (celsius * 9/5) + 32, temperaturas_celsius))

# Exibindo os resultados
print(f"Temperaturas em Fahrenheit: {temperaturas_fahrenheit}")

#3 Dada uma lista de palavras, use uma função lambda para retornar uma lista com o comprimento de cada palavra.

# Lista de palavras
palavras = ["python", "lambda", "programação", "exemplo", "lista"]

# Função Lambda para calcular o comprimento de cada palavra
comprimentos = list(map(lambda palavra: len(palavra), palavras))

# Exibindo os resultados
print(f"Comprimentos das palavras: {comprimentos}")

#4 Use uma função lambda para dobrar os valores de uma lista de inteiros.

# Lista de inteiros
numeros = [1, 2, 3, 4, 5]

# Função Lambda para dobrar os valores da lista
dobrados = list(map(lambda x: x * 2, numeros))

# Exibindo os resultados
print(f"Valores dobrados: {dobrados}")

#5 Dada uma lista de nomes, use uma função lambda para adicionar o prefixo "Sr./Sra." antes de cada nome.

# Lista de nomes
nomes = ["João", "Maria", "Carlos", "Ana"]

# Função Lambda para adicionar o prefixo "Sr./Sra." antes de cada nome
nomes_com_prefixo = list(map(lambda nome: f"Sr./Sra. {nome}", nomes))

# Exibindo os resultados
print(f"Nomes com prefixo: {nomes_com_prefixo}")

#6 Dada uma lista de números, use uma função lambda para retornar apenas os números pares.

# Lista de números
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Função Lambda para filtrar apenas os números pares
numeros_pares = list(filter(lambda x: x % 2 == 0, numeros))

# Exibindo os resultados
print(f"Números pares: {numeros_pares}")

#7 Dada uma lista de palavras, use uma função lambda para retornar apenas as palavras com menos de 5 caracteres.

# Lista de palavras
palavras = ["cachorro", "gato", "carro", "lua", "sol", "casa", "flor"]

# Função Lambda para filtrar apenas palavras com menos de 5 caracteres
palavras_curta = list(filter(lambda palavra: len(palavra) < 5, palavras))

# Exibindo os resultados
print(f"Palavras com menos de 5 caracteres: {palavras_curta}")

#8 Dada uma lista de idades, use uma função lambda para retornar apenas as idades maiores que 18.

# Lista de idades
idades = [15, 18, 20, 25, 30, 17, 16]

# Função Lambda para filtrar apenas as idades maiores que 18
idades_maiores_que_18 = list(filter(lambda idade: idade > 18, idades))

# Exibindo os resultados
print(f"Idades maiores que 18: {idades_maiores_que_18}")

#9 Dada uma lista de strings, use uma função lambda para retornar as strings que começam com a letra "a".

# Lista de strings
strings = ["amigo", "banana", "abacaxi", "maçã", "amável", "mango"]

# Função Lambda para filtrar as strings que começam com "a"
strings_com_a = list(filter(lambda s: s.lower().startswith("a"), strings))

# Exibindo os resultados
print(f"Strings que começam com a letra 'a': {strings_com_a}")

#10 Dada uma lista de números inteiros, use uma função lambda para retornar apenas os números positivos.

# Lista de números inteiros
numeros = [-10, 15, -3, 20, -5, 30, 0]

# Função Lambda para filtrar apenas os números positivos
numeros_positivos = list(filter(lambda x: x > 0, numeros))

# Exibindo os resultados
print(f"Números positivos: {numeros_positivos}")

#11 Use uma função lambda para calcular a soma de uma lista de números.

# Lista de números
numeros = [1, 2, 3, 4, 5]

# Função Lambda para calcular a soma dos números
soma = reduce(lambda x, y: x + y, numeros)

# Exibindo o resultado
print(f"Soma dos números: {soma}")

#12 Use uma função lambda para multiplicar todos os elementos de uma lista.

from functools import reduce

# Lista de números
numeros = [1, 2, 3, 4, 5]

# Função Lambda para multiplicar todos os elementos da lista
produto = reduce(lambda x, y: x * y, numeros)

# Exibindo o resultado
print(f"Produto dos números: {produto}")

#13 Use uma função lambda para encontrar o maior número em uma lista.

# Lista de números
numeros = [10, 20, 35, 50, 5, 70, 30]

# Função Lambda para encontrar o maior número
maior_numero = max(numeros, key=lambda x: x)

# Exibindo o resultado
print(f"O maior número é: {maior_numero}")

#14 Use uma função lambda para concatenar uma lista de palavras em uma única string separada por espaços.

# Lista de palavras
palavras = ["Olá", "mundo", "isso", "é", "um", "teste"]

# Função Lambda para concatenar as palavras com espaço entre elas
concatenada = reduce(lambda x, y: x + " " + y, palavras)

# Exibindo o resultado
print(f"Palavras concatenadas: {concatenada}")

#15 Use uma função lambda para somar os dígitos de uma lista de inteiros, onde cada número é tratado individualmente.

# Lista de números inteiros
numeros = [123, 456, 789]

# Função Lambda para somar os dígitos de cada número
soma_dos_digitos = sum(map(lambda num: sum(int(digit) for digit in str(num)), numeros))

# Exibindo o resultado
print(f"Soma dos dígitos de todos os números: {soma_dos_digitos}")

#16 Use uma função lambda para dobrar os números de uma lista e retornar apenas os números que são maiores que 20.

# Lista de números
numeros = [5, 10, 15, 20, 25, 30]

# Função Lambda para dobrar os números e retornar apenas os que são maiores que 20
numeros_maiores_que_20 = list(filter(lambda x: x * 2 > 20, numeros))

# Exibindo os resultados
print(f"Números dobrados e maiores que 20: {numeros_maiores_que_20}")

#17 Dada uma lista de palavras, use uma função lambda para encontrar todas as palavras que contêm a letra "e" e conte quantas são.

# Lista de palavras
palavras = ["casa", "elefante", "bola", "abacaxi", "esperança", "carro"]

# Função Lambda para filtrar palavras que contêm a letra 'e'
palavras_com_e = list(filter(lambda palavra: 'e' in palavra, palavras))

# Contando quantas palavras contêm a letra 'e'
quantidade_palavras_com_e = len(palavras_com_e)

# Exibindo os resultados
print(f"Palavras que contêm a letra 'e': {palavras_com_e}")
print(f"Quantidade de palavras que contêm a letra 'e': {quantidade_palavras_com_e}")

#18 Converta uma lista de temperaturas de Fahrenheit para Celsius usando uma função lambda e, em seguida, retorne apenas as temperaturas abaixo de 20°C.

# Lista de temperaturas em Fahrenheit
temperaturas_fahrenheit = [32, 50, 68, 86, 104, 122]

# Função Lambda para converter Fahrenheit para Celsius
temperaturas_celsius = list(map(lambda f: (f - 32) * 5/9, temperaturas_fahrenheit))

# Filtrando as temperaturas abaixo de 20°C
temperaturas_abaixo_20 = list(filter(lambda c: c < 20, temperaturas_celsius))

# Exibindo os resultados
print(f"Temperaturas em Celsius abaixo de 20°C: {temperaturas_abaixo_20}")

#19 Use uma função lambda para selecionar apenas os números pares de uma lista e, em seguida, somar esses números.

from functools import reduce

# Lista de números
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Função Lambda para filtrar os números pares
numeros_pares = list(filter(lambda x: x % 2 == 0, numeros))

# Função Lambda para somar os números pares
soma_pares = reduce(lambda x, y: x + y, numeros_pares)

# Exibindo o resultado
print(f"Soma dos números pares: {soma_pares}")

#20 Use uma função lambda para substituir números negativos de uma lista por 0 e manter os positivos.

# Lista de números
numeros = [10, -5, 3, -2, 7, -8, 6]

# Função Lambda para substituir números negativos por 0 e manter os positivos
numeros_modificados = list(map(lambda x: x if x > 0 else 0, numeros))

# Exibindo o resultado
print(f"Lista modificada: {numeros_modificados}")

#21 Use uma função lambda para retornar a lista de cubos de cada elemento em uma lista de números.

# Lista de números
numeros = [1, 2, 3, 4, 5]

# Função Lambda para calcular o cubo de cada número
cubos = list(map(lambda x: x ** 3, numeros))

# Exibindo o resultado
print(f"Cubos dos números: {cubos}")

#22 Use uma função lambda para verificar se um número dado é primo (retornando True ou False).

# Função Lambda para verificar se um número é primo
is_prime = lambda n: n > 1 and all(n % i != 0 for i in range(2, int(n ** 0.5) + 1))

# Exemplo de uso
numero = 7
resultado = is_prime(numero)

# Exibindo o resultado
print(f"O número {numero} é primo? {resultado}")

#23 Use uma função lambda para dividir cada elemento de uma lista por 5 e retornar a nova lista.

# Lista de números
numeros = [10, 20, 30, 40, 50]

# Função Lambda para dividir cada número por 5
resultados = list(map(lambda x: x / 5, numeros))

# Exibindo o resultado
print(f"Lista com os números divididos por 5: {resultados}")

#24 Use uma função lambda para remover todas as vogais de uma string dada.

# String original
texto = "Olá, como você está?"

# Função Lambda para remover as vogais
remover_vogais = lambda s: ''.join([char for char in s if char.lower() not in 'aeiou'])

# Exibindo o resultado
resultado = remover_vogais(texto)
print(f"Texto sem vogais: {resultado}")

#25 Use uma função lambda para converter todas as palavras em uma lista para letras maiúsculas.

# Lista de palavras
palavras = ["olá", "como", "você", "está"]

# Função Lambda para converter as palavras para maiúsculas
palavras_maiusculas = list(map(lambda palavra: palavra.upper(), palavras))

# Exibindo o resultado
print(f"Palavras em maiúsculas: {palavras_maiusculas}")

#26 Use uma função lambda para retornar apenas os números negativos de uma lista de inteiros.

# Lista de números
numeros = [10, -5, 3, -2, 7, -8, 6]

# Função Lambda para filtrar os números negativos
numeros_negativos = list(filter(lambda x: x < 0, numeros))

# Exibindo o resultado
print(f"Números negativos: {numeros_negativos}")

#27 Use uma função lambda para converter todos os números de uma lista para seus valores absolutos.

# Lista de números
numeros = [-10, 5, -3, 7, -2, 8]

# Função Lambda para converter cada número para seu valor absoluto
valores_absolutos = list(map(lambda x: abs(x), numeros))

# Exibindo o resultado
print(f"Valores absolutos: {valores_absolutos}")

#28 Use uma função lambda para retornar uma lista com o resto da divisão de cada elemento por 3.

# Lista de números
numeros = [10, 20, 30, 40, 50]

# Função Lambda para calcular o resto da divisão de cada número por 3
restos = list(map(lambda x: x % 3, numeros))

# Exibindo o resultado
print(f"Resto da divisão por 3: {restos}")

#29 Dada uma lista de números, use uma função lambda para multiplicar cada elemento pelo seu índice.

# Lista de números
numeros = [10, 20, 30, 40, 50]

# Função Lambda para multiplicar cada número pelo seu índice
resultados = list(map(lambda x, i: x * i, numeros, range(len(numeros))))

# Exibindo o resultado
print(f"Resultados da multiplicação pelo índice: {resultados}")

#30 Use uma função lambda para verificar se uma palavra dada é um palíndromo (retornando True ou False).

# Função Lambda para verificar se uma palavra é um palíndromo
is_palindrome = lambda palavra: palavra == palavra[::-1]

# Exemplo de uso
palavra = "radar"
resultado = is_palindrome(palavra)

# Exibindo o resultado
print(f"A palavra '{palavra}' é um palíndromo? {resultado}")
