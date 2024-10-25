# Atividade dicionário_tuplas

#1 Crie uma tupla chamada cidades que contenha os nomes de cinco cidades. Imprima a terceira cidade.

# Criação da tupla com cinco cidades
cidades = ('São Paulo', 'Rio de Janeiro', 'Belo Horizonte', 'Curitiba', 'Porto Alegre')

# Imprimindo a terceira cidade
print(cidades[2])

#2 Crie uma tupla chamada numeros com os seguintes valores: (1, 2, 3, 1, 4, 1). Utilize o método count() para contar quantas vezes o número 1 aparece na tupla.

# Criação da tupla com os valores
numeros = (1, 2, 3, 1, 4, 1)

# Contando quantas vezes o número 1 aparece na tupla
contagem = numeros.count(1)

# Imprimindo o resultado
print(contagem)

#3 Crie uma tupla chamada animais com os seguintes valores: ('cachorro', 'gato', 'pássaro'). Verifique se 'gato' está na tupla e imprima uma mensagem informando o resultado.

# Criação da tupla com os animais
animais = ('cachorro', 'gato', 'pássaro')

# Verificando se 'gato' está na tupla
if 'gato' in animais:
    print("Gato está na tupla.")
else:
    print("Gato não está na tupla.")

#4 Dada a tupla meses = ('janeiro', 'fevereiro', 'março', 'abril', 'maio'), encontre e imprima o índice do mês 'abril'.

# Criação da tupla com os meses
meses = ('janeiro', 'fevereiro', 'março', 'abril', 'maio')

# Encontrando o índice do mês 'abril'
indice_abril = meses.index('abril')

# Imprimindo o índice
print(indice_abril)

#5 Crie uma tupla chamada coordenadas que armazene a latitude e longitude de um local (ex: (-23.5505, -46.6333)). Imprima a latitude e a longitude separadamente.

# Criação da tupla com latitude e longitude
coordenadas = (-23.5505, -46.6333)

# Imprimindo a latitude e a longitude separadamente
latitude = coordenadas[0]
longitude = coordenadas[1]

print("Latitude:", latitude)
print("Longitude:", longitude)

#6 Crie um dicionário chamado carro com as chaves marca, modelo e ano. Atribua valores de sua escolha e imprima o modelo do carro.

# Criação do dicionário com as informações do carro
carro = {
    'marca': 'Toyota',
    'modelo': 'Corolla',
    'ano': 2020
}

# Imprimindo o modelo do carro
print(carro['modelo'])

#7 Use o dicionário carro que você criou no exercício anterior. Adicione uma nova chave chamada cor e atribua uma cor ao carro. Em seguida, imprima o dicionário completo.

# Usando o dicionário carro criado anteriormente
carro = {
    'marca': 'Toyota',
    'modelo': 'Corolla',
    'ano': 2020
}

# Adicionando a nova chave 'cor'
carro['cor'] = 'preto'

# Imprimindo o dicionário completo
print(carro)

#8 Dado o dicionário pessoa = {'nome': 'João', 'idade': 30, 'cidade': 'São Paulo'}, remova a chave idade e imprima o dicionário resultante.

# Dicionário dado
pessoa = {'nome': 'João', 'idade': 30, 'cidade': 'São Paulo'}

# Removendo a chave 'idade'
pessoa.pop('idade')

# Imprimindo o dicionário resultante
print(pessoa)

#9 Crie um dicionário chamado produto que contenha nome, preco e quantidade. Use um loop for para imprimir todos os pares chave/valor.

# Criação do dicionário com informações do produto
produto = {
    'nome': 'Notebook',
    'preco': 2500.00,
    'quantidade': 10
}

# Usando um loop for para imprimir todos os pares chave/valor
for chave, valor in produto.items():
    print(f"{chave}: {valor}")

#10 Dado o dicionário estudante = {'nome': 'Maria', 'curso': 'Biologia', 'ano': 2}, verifique se a chave curso existe. Se existir, imprima "A estudante está no curso de Biologia."

# Dicionário dado
estudante = {'nome': 'Maria', 'curso': 'Biologia', 'ano': 2}

# Verificando se a chave 'curso' existe
if 'curso' in estudante:
    print("A estudante está no curso de Biologia.")

# Atividade conjunto_set

#1 - Crie um conjunto chamado `frutas` que contenha os seguintes elementos: "maçã", "banana", "laranja" e "uva". Depois de criar o conjunto, exiba-o no console para confirmar os elementos adicionados.

# Criação do conjunto com as frutas
frutas = {"maçã", "banana", "laranja", "uva"}

# Exibindo o conjunto no console
print(frutas)

#2 - Utilizando o conjunto `frutas` criado anteriormente, adicione a fruta "morango" ao conjunto. Lembre-se que conjuntos não permitem duplicatas, então adicione um elemento que já exista para verificar o comportamento.

# Conjunto existente de frutas
frutas = {"maçã", "banana", "laranja", "uva"}

# Adicionando a fruta "morango" ao conjunto
frutas.add("morango")

# Tentando adicionar "banana" novamente para verificar o comportamento
frutas.add("banana")

# Exibindo o conjunto no console
print(frutas)

#3 - Remova a fruta "banana" do conjunto `frutas`. Se "banana" não estiver presente, o código pode gerar um erro. Verifique se a fruta existe antes de removê-la ou trate o erro adequadamente.

# Conjunto existente de frutas
frutas = {"maçã", "banana", "laranja", "uva", "morango"}

# Verificando se "banana" está no conjunto antes de removê-la
if "banana" in frutas:
    frutas.remove("banana")
    print("Banana removida com sucesso.")
else:
    print("A fruta 'banana' não está no conjunto.")

# Exibindo o conjunto atualizado
print(frutas)

#4 - Verifique se a fruta "laranja" está presente no conjunto `frutas` usando uma estrutura condicional. Exiba uma mensagem no console indicando se "laranja" está ou não presente no conjunto.

# Conjunto existente de frutas
frutas = {"maçã", "uva", "morango"}

# Verificando se "laranja" está presente no conjunto
if "laranja" in frutas:
    print("A fruta 'laranja' está presente no conjunto.")
else:
    print("A fruta 'laranja' não está presente no conjunto.")

#5 - Crie um segundo conjunto chamado `citrus`, contendo "laranja", "limão" e "tangerina". Faça a união dos conjuntos `frutas` e `citrus`, criando um novo conjunto que contém todos os elementos dos dois conjuntos. Exiba o resultado dessa união.

# Conjunto existente de frutas
frutas = {"maçã", "uva", "morango"}

# Criação do segundo conjunto citrus
citrus = {"laranja", "limão", "tangerina"}

# Fazendo a união dos conjuntos frutas e citrus
uniao = frutas.union(citrus)

# Exibindo o resultado da união
print(uniao)

#6 - Usando os conjuntos `frutas` e `citrus`, encontre a interseção entre eles, ou seja, os elementos que estão presentes em ambos os conjuntos. Exiba os elementos comuns.

# Conjunto existente de frutas
frutas = {"maçã", "uva", "morango"}

# Conjunto citrus
citrus = {"laranja", "limão", "tangerina"}

# Encontrando a interseção entre os conjuntos frutas e citrus
intersecao = frutas.intersection(citrus)

# Exibindo os elementos comuns
print(intersecao)

#7 - Encontre a diferença entre os conjuntos `frutas` e `citrus`, ou seja, os elementos que estão em `frutas` mas não estão em `citrus`. Exiba o resultado dessa diferença.

# Conjunto existente de frutas
frutas = {"maçã", "uva", "morango"}

# Conjunto citrus
citrus = {"laranja", "limão", "tangerina"}

# Encontrando a diferença entre os conjuntos frutas e citrus
diferenca = frutas.difference(citrus)

# Exibindo os elementos que estão em frutas mas não em citrus
print(diferenca)

#8 - Esvazie completamente o conjunto `citrus` usando um método específico que remove todos os elementos de um conjunto. Verifique se o conjunto foi realmente esvaziado ao exibi-lo no console após a operação.

# Conjunto citrus existente
citrus = {"laranja", "limão", "tangerina"}

# Esvaziando completamente o conjunto citrus
citrus.clear()

# Verificando se o conjunto foi realmente esvaziado
print("Conjunto citrus após esvaziar:", citrus)


#9 - Converta o conjunto `frutas` em um conjunto imutável, ou seja, um conjunto que não pode ser alterado após sua criação. Crie esse conjunto imutável e exiba-o no console.

# Conjunto existente de frutas
frutas = {"maçã", "uva", "morango"}

# Convertendo o conjunto em um conjunto imutável (frozenset)
frutas_imutaveis = frozenset(frutas)

# Exibindo o conjunto imutável no console
print(frutas_imutaveis)

#10 - Conte quantos elementos únicos existem no conjunto `frutas` e exiba o número total de elementos no console.

# Conjunto existente de frutas
frutas = {"maçã", "uva", "morango"}

# Contando quantos elementos únicos existem no conjunto
numero_de_elementos = len(frutas)

# Exibindo o número total de elementos no console
print("Número total de elementos únicos no conjunto 'frutas':", numero_de_elementos)

# Lista de exercícios de fixação dos conteúdos de Listas, Tuplas, Sets e Dicionários.

#1. Crie uma lista contendo cinco números inteiros de sua escolha. Em seguida, percorra essa lista e imprima o valor de cada elemento multiplicado por 2. O resultado deve mostrar o novo valor de cada elemento, um por vez.

# Criar uma lista com cinco números inteiros
numeros = [3, 5, 7, 9, 11]

# Percorrer a lista e imprimir o valor de cada elemento multiplicado por 2
for numero in numeros:
    novo_valor = numero * 2
    print(novo_valor)

#2. Dada a lista ["maçã", "banana", "laranja", "uva"], remova o item "banana" da lista e adicione a fruta "melancia" no lugar. Depois, mostre a nova lista atualizada com as alterações feitas.

# Lista original
frutas = ["maçã", "banana", "laranja", "uva"]

# Remover "banana" da lista
frutas.remove("banana")

# Adicionar "melancia" no lugar
frutas.append("melancia")

# Mostrar a nova lista atualizada
print(frutas)

#3. Escreva um programa que receba uma lista de números inteiros e exiba qual é o maior número e qual é o menor número presente na lista. Certifique-se de mostrar ambos os valores ao final.

# Função para encontrar o maior e o menor número em uma lista
def encontrar_maior_menor(numeros):
    if not numeros:
        return None, None  # Retorna None se a lista estiver vazia
    
    maior = max(numeros)  # Encontra o maior número
    menor = min(numeros)  # Encontra o menor número
    return maior, menor

# Lista de números inteiros (exemplo)
numeros = [10, 5, 20, 3, 15]

# Encontrar o maior e o menor número
maior_numero, menor_numero = encontrar_maior_menor(numeros)

# Mostrar os resultados
print(f"O maior número é: {maior_numero}")
print(f"O menor número é: {menor_numero}")

#4. Crie uma função que receba uma lista contendo várias palavras (strings). A função deve devolver uma nova lista que contenha a quantidade de letras de cada palavra da lista original. Exiba essa nova lista com o número de letras correspondente a cada palavra.

# Função para contar letras de cada palavra em uma lista
def contar_letras(palavras):
    # Usar uma lista por compreensão para contar as letras
    return [len(palavra) for palavra in palavras]

# Lista de palavras (exemplo)
lista_palavras = ["maçã", "banana", "laranja", "uva"]

# Chamar a função e obter a nova lista com a quantidade de letras
quantidade_letras = contar_letras(lista_palavras)

# Exibir a nova lista com a quantidade de letras
print(quantidade_letras)

#5. Dada uma lista de números inteiros que você vai definir, ordene essa lista em ordem crescente e depois exiba o resultado da lista ordenada.

# Definindo uma lista de números inteiros
numeros = [42, 15, 8, 23, 4, 16]

# Ordenando a lista em ordem crescente
numeros_ordenados = sorted(numeros)

# Exibindo a lista ordenada
print(numeros_ordenados)

#6. Crie uma tupla que contenha os números de 1 a 5. Tente alterar o valor do segundo elemento dessa tupla e observe o que acontece. No final, explique por que você conseguiu ou não modificar o valor.

# Criando uma tupla com os números de 1 a 5
tupla_numeros = (1, 2, 3, 4, 5)

# Tentando alterar o segundo elemento da tupla
try:
    tupla_numeros[1] = 20  # Isso irá gerar um erro
except TypeError as e:
    print(f"Erro ao tentar modificar o segundo elemento: {e}")

# Exibindo a tupla original
print(tupla_numeros)

#7. Escreva um programa que receba uma tupla contendo diversos números inteiros. O programa deve calcular e exibir a soma de todos os números presentes na tupla.

# Função para calcular a soma dos números em uma tupla
def soma_tupla(numeros):
    return sum(numeros)

# Definindo uma tupla com números inteiros (exemplo)
tupla_numeros = (10, 20, 30, 40, 50)

# Calculando a soma dos números na tupla
resultado = soma_tupla(tupla_numeros)

# Exibindo o resultado da soma
print(f"A soma dos números na tupla é: {resultado}")

#8. Dada uma tupla que contém cinco números, crie uma função que retorne o primeiro e o último número dessa tupla. O programa deve imprimir ambos os valores corretamente.

# Função para retornar o primeiro e o último número de uma tupla
def primeiro_e_ultimo(tupla):
    primeiro = tupla[0]  # Primeiro elemento
    ultimo = tupla[-1]   # Último elemento
    return primeiro, ultimo

# Definindo uma tupla com cinco números (exemplo)
tupla_numeros = (5, 10, 15, 20, 25)

# Chamando a função para obter o primeiro e o último número
primeiro_numero, ultimo_numero = primeiro_e_ultimo(tupla_numeros)

# Exibindo os resultados
print(f"O primeiro número é: {primeiro_numero}")
print(f"O último número é: {ultimo_numero}")

#9. Converta a lista ["a", "b", "c", "d"] em uma tupla e, em seguida, exiba o tipo do novo objeto que foi criado. O programa deve deixar claro que o tipo mudou de lista para tupla.

# Definindo uma lista
lista = ["a", "b", "c", "d"]

# Convertendo a lista em uma tupla
tupla = tuple(lista)

# Exibindo a tupla e o tipo do novo objeto
print(f"A tupla é: {tupla}")
print(f"O tipo do novo objeto é: {type(tupla)}")

#10. Crie uma tupla com três números inteiros e uma string. Depois, verifique se o número 3 está presente nessa tupla e mostre uma mensagem dizendo se o número foi encontrado ou não.

# Criando uma tupla com três números inteiros e uma string
tupla = (1, 2, 3, "quatro")

# Verificando se o número 3 está presente na tupla
if 3 in tupla:
    print("O número 3 foi encontrado na tupla.")
else:
    print("O número 3 não foi encontrado na tupla.")

#11. Crie dois sets: set1 = {1, 2, 3, 4} e set2 = {3, 4, 5, 6}. Exiba a união dos dois sets (todos os elementos sem repetição), a interseção (elementos que aparecem nos dois sets) e a diferença (elementos presentes no primeiro set, mas não no segundo). Mostre os resultados de cada operação.

# Definindo os dois sets
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

# União dos dois sets
uniao = set1 | set2  # ou set1.union(set2)

# Interseção dos dois sets
interseccao = set1 & set2  # ou set1.intersection(set2)

# Diferença entre set1 e set2
diferenca = set1 - set2  # ou set1.difference(set2)

# Exibindo os resultados
print(f"União: {uniao}")
print(f"Interseção: {interseccao}")
print(f"Diferença (set1 - set2): {diferenca}")

#12. Dada a lista [1, 2, 2, 3, 4, 4, 5], remova os elementos duplicados transformando a lista em um set. Ao final, exiba o set resultante, que deve conter apenas valores únicos.

# Definindo a lista com elementos duplicados
lista = [1, 2, 2, 3, 4, 4, 5]

# Transformando a lista em um set para remover duplicatas
set_resultante = set(lista)

# Exibindo o set resultante
print(f"O set resultante é: {set_resultante}")
