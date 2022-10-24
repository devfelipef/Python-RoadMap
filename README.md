# Python
Minhas anotações de aprendizados da linguagem Python

- **Comentário**
    
    ```python
    #Para comentar
    
    '''
    Para comentar varias linhas
    '''
    ```

- **Variáveis**
    
    ```python
    #Criando variaveis
    from re import X
    
    nome = "João"
    idade = 20
    altura = 1.80
    
    #Em python não é necessário declarar o tipo da variavel
    
    print(nome, idade, altura)
    
    #Para especificar o tipo da variavel
    x = str('João')
    y = int(20)
    z = float(1.80) 
    
    print(x, y, z)
    
    #Atribuir muitos valores a varias variaveis
    a, b, c = 'João', 20, 1.80
    print(a, b, c)
    
    #Atribuir o mesmo valor a varias variaveis
    d = e = f = 'João'
    print(d, e, f)
    
    #Variaveis globais
    x = "awesome"
    
    def myfunc():
      x = "fantastic"
      print("Python is " + x)
    myfunc()
    print("Python is " + x)
    
    #Para saber o tipo da variavel
    print(type(nome))
    print(type(idade))
    print(type(altura))
    
    #Tipos de dados
    x = str("Hello World") #str
    x = int(20) #int
    x = float(20.5) #float
    x = complex(1j) #complex
    x = list(("apple", "banana", "cherry")) #list
    x = tuple(("apple", "banana", "cherry")) #tuple
    x = range(6) #range
    x = dict(name="John", age=36) #dict
    x = set(("apple", "banana", "cherry")) #set
    x = frozenset(("apple", "banana", "cherry")) #frozenset
    x = bool(5) #bool
    x = bytes(5) #bytes
    x = bytearray(5) #bytearray
    x = memoryview(bytes(5)) #memoryview
    x = None #NoneType
    ```
    
- **Input**
    
    ```python
    #input
    def entradadedados():
      idade = input("Digite sua idade: ")
      texto = 'Sua idade é {}'.format(idade)
      print(texto)
    
    entradadedados()
    ```
    
- **Strings**
    
    ```python
    #String varias linhas
    a = """Lorem ipsum dolor sit amet,
    consectetur adipiscing elit,
    sed do eiusmod tempor incididunt
    ut labore et dolore magna aliqua."""
    print(a)
    
    #String são arrays
    a = "Hello, World!"
    print(a[1])
    
    #Loop em string
    for x in "banana":
      print(x)
    
    #Comprimento de string
    a = "Hello, World!"
    print(len(a))
    
    #Checar se uma string contem uma palavra
    txt = "The best things in life are free!"
    print("free" in txt)
    
    #Checar se uma string não contem uma palavra
    txt = "The best things in life are free!"
    print("expensive" not in txt)
    
    #Fatiamento de string
    b = "Hello, World!"
    print(b[2:5])
    
    #Modificar string
    a = "Hello, World!"
    print(a.upper()) #Maiuscula
    
    a = "Hello, World!"
    print(a.lower()) #Minuscula
    
    a = "Hello, World!"
    print(a.split(",")) #Quebra a string em uma lista
    
    a = "Hello, World!"
    print(a.replace("H", "J")) #Substituir
    
    a = "Hello, World!"
    print(a.capitalize()) #Primeira letra maiuscula
    
    a = "Hello, World!"
    print(a.casefold()) #Tudo minusculo
    
    a = "Hello, World!"
    print(a.center(20)) #Centralizar
    
    a = "Hello, World!"
    print(a.count("l")) #Contar
    
    a = "Hello, World!"
    print(a.encode()) #Codificar
    
    a = "Hello, World!"
    print(a.endswith(".")) #Verificar se termina com .
    
    a = "Hello, World!"
    print(a.find("r")) #Encontrar
    
    a = "Hello, World!"
    print(a.index("r")) #Encontrar
    
    a = "Hello, World!"
    print(a.isalnum()) #Verificar se é alfanumerico
    
    a = "Hello, World!"
    print(a.isalpha()) #Verificar se é alfabetico
    
    a = "Hello, World!"
    print(a.isdecimal()) #Verificar se é decimal
    
    a = "Hello, World!"
    print(a.isdigit()) #Verificar se é digito
    
    a = "Hello, World!"
    print(a.isidentifier()) #Verificar se é identificador
    
    a = "Hello, World!"
    print(a.islower()) #Verificar se é minusculo
    
    a = "Hello, World!"
    print(a.isnumeric()) #Verificar se é numerico
    
    a = "Hello, World!"
    print(a.isprintable()) #Verificar se é imprimivel
    
    a = "Hello, World!"
    print(a.isspace()) #Verificar se é espaço
    
    a = "Hello, World!"
    print(a.istitle()) #Verificar se é titulo
    
    a = "Hello, World!"
    print(a.isupper()) #Verificar se é maiusculo
    
    a = "Hello, World!"
    print(a.join("XYZ")) #Juntar
    
    a = "Hello, World!"
    print(a.ljust(20)) #Alinhar a esquerda
    
    a = "Hello, World!"
    print(a.rjust(20)) #Alinhar a direita
    
    a = "Hello, World!"
    print(a.partition(" ")) #Particionar
    
    a = "Hello, World!"
    print(a.rpartition(" ")) #Particionar de tras pra frente
    
    a = "Hello, World!"
    print(a.translate(a.maketrans("H", "J"))) #Traduzir
    
    #etc...
    #https://www.w3schools.com/python/python_strings.asp
    
    #Concatenar string
    a = "Hello"
    b = "World"
    c = a + " " + b
    print(c)
    
    #Formatar string
    age = 36
    txt = "My name is John, and I am {} years old"
    print(txt.format(age))
    
    quantity = 3
    itemno = 567
    price = 49.95
    myorder = "I want {} pieces of item {} for {} dollars."
    print(myorder.format(quantity, itemno, price))
    ```
    
- **Boolean**
    
    ```python
    print(10 > 9)
    print(10 == 9)
    print(10 < 9)
    
    a = 200
    b = 33
    
    def myFunction() :
      return True
    
    if myFunction():
      print("YES!")
    else:
      print("NO!")
    ```
    
- **Operadores**
    
    ```python
    #Operadores aritimeticos
    x = 5
    y = 3
    print(x + y) #Soma
    print(x - y) #Subtração
    print(x * y) #Multiplicação
    print(x / y) #Divisão
    print(x % y) #Resto
    print(x ** y) #Potencia
    print(x // y) #Divisão inteira
    
    #Operadores de atribuição
    x = 5
    x += 3
    print(x)
    
    x = 5
    x -= 3
    print(x)
    
    x = 5
    x *= 3
    print(x)
    
    #etc...
    #https://www.w3schools.com/python/python_strings.asp
    
    #Operadores de comparação
    x = 5
    y = 3
    print(x == y) #Igual
    print(x != y) #Diferente
    print(x > y) #Maior
    print(x < y) #Menor
    print(x >= y) #Maior ou igual
    print(x <= y) #Menor ou igual
    
    #Operadores lógicos
    x = 5
    print(x > 3 and x < 10) #E
    print(x > 3 or x < 4) #OU
    print(not(x > 3 and x < 10)) #NÃO
    
    #Operadores de identidade
    x = ["apple", "banana"]
    y = ["apple", "banana"]
    z = x
    print(x is z) #É
    print(x is not z) #Não é
    print(x is y) #É
    print(x is not y) #Não é
    
    #Operadores de associação
    x = ["apple", "banana"]
    print("banana" in x) #Está
    print("pineapple" not in x) #Não está
    
    #Operadores de bit a bit
    x = 10
    y = 4
    print(x & y) #E
    print(x | y) #OU
    print(x ^ y) #OU exclusivo
    print(~x) #NÃO
    print(x << 2) #Deslocamento a esquerda
    print(x >> 2) #Deslocamento a direita
    ```
    
- **Listas**
    
    ```python
    #Listas python
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    print(MinhaLista)
    
    #Acessar item
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    print(MinhaLista[1])
    
    #Alterar item
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista[1] = "Laranja"
    print(MinhaLista)
    
    #Loop
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    for x in MinhaLista:
      print(x)
    
    #Verificar se existe
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    if "Maçã" in MinhaLista:
      print("Sim, 'Maçã' está na lista")
    
    #Tamanho da lista
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    print(len(MinhaLista))
    
    #Adicionar item
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista.append("Laranja")
    
    #Inserir item
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista.insert(1, "Laranja")
    
    #Remover item
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista.remove("Banana")
    
    #Remover item pelo indice
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista.pop(1)
    
    #Remover ultimo item
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista.pop()
    
    #Remover todos os itens
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista.clear()
    
    #Copiar lista
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista2 = MinhaLista.copy()
    
    #Copiar lista
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista2 = list(MinhaLista)
    
    #Juntar listas
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista2 = ["Laranja", "Limão"]
    MinhaLista3 = MinhaLista + MinhaLista2
    
    #Juntar listas
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista2 = ["Laranja", "Limão"]
    for x in MinhaLista2:
      MinhaLista.append(x)
    
    #Juntar listas
    MinhaLista = ["Maçã", "Banana", "Cereja"]
    MinhaLista2 = ["Laranja", "Limão"]
    MinhaLista.extend(MinhaLista2)
    
    #Construir lista
    MinhaLista = list(("Maçã", "Banana", "Cereja"))
    ```
    
- **Tuplas**
    
    ```python
    #Tuplas python
    MinhaTupla = ("Maçã", "Banana", "Cereja")
    print(MinhaTupla)
    
    #Acessar item
    MinhaTupla = ("Maçã", "Banana", "Cereja")
    print(MinhaTupla[1])
    
    #Loop
    MinhaTupla = ("Maçã", "Banana", "Cereja")
    for x in MinhaTupla:
      print(x)
    
    #Verificar se existe
    MinhaTupla = ("Maçã", "Banana", "Cereja")
    if "Maçã" in MinhaTupla:
      print("Sim, 'Maçã' está na tupla")
    
    #Tamanho da tupla
    MinhaTupla = ("Maçã", "Banana", "Cereja")
    print(len(MinhaTupla))
    
    #Remover item
    MinhaTupla = ("Maçã", "Banana", "Cereja")
    del MinhaTupla
    
    #Remover item
    MinhaTupla = ("Maçã", "Banana", "Cereja")
    MinhaTupla = list(MinhaTupla)
    MinhaTupla.remove("Banana")
    MinhaTupla = tuple(MinhaTupla)
    
    #Juntar tuplas
    MinhaTupla = ("Maçã", "Banana", "Cereja")
    MinhaTupla2 = ("Laranja", "Limão")
    MinhaTupla3 = MinhaTupla + MinhaTupla2
    
    #Construir tupla
    MinhaTupla = tuple(("Maçã", "Banana", "Cereja"))
    
    #Sets python
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    print(MinhaSet)
    
    #Acessar item
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    for x in MinhaSet:
      print(x)
    
    #Verificar se existe
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    print("Maçã" in MinhaSet)
    
    #Tamanho do set
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    print(len(MinhaSet))
    
    #Adicionar item
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    MinhaSet.add("Laranja")
    
    #Adicionar itens
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    MinhaLista = ["Laranja", "Limão"]
    MinhaSet.update(MinhaLista)
    
    #Remover item
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    MinhaSet.remove("Banana")
    
    #Remover item
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    MinhaSet.discard("Banana")
    
    #Remover item
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    x = MinhaSet.pop()
    
    #Remover todos os itens
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    MinhaSet.clear()
    
    #Copiar set
    MinhaSet = {"Maçã", "Banana", "Cereja"}
    MinhaSet2 = MinhaSet.copy()
    
    #etc...
    #https://www.w3schools.com/python/python_sets.asp
    ```
    
- **Dicionario**
    
    ```python
    #Dicionários python
    MinhaDicionario = { "nome": "João", "idade": 36 }
    print(MinhaDicionario)
    
    #Acessar item
    MinhaDicionario = { "nome": "João", "idade": 36 }
    print(MinhaDicionario["nome"])
    
    #Acessar item
    MinhaDicionario = { "nome": "João", "idade": 36 }
    print(MinhaDicionario.get("nome"))
    
    #Loop
    MinhaDicionario = { "nome": "João", "idade": 36 }
    
    for x in MinhaDicionario:
      print(x)
    
    #alterar valor
    MinhaDicionario = { "nome": "João", "idade": 36 }
    MinhaDicionario["idade"] = 40
    
    #adicionar item
    MinhaDicionario = { "nome": "João", "idade": 36 }
    MinhaDicionario["cor"] = "azul"
    
    #remover item
    MinhaDicionario = { "nome": "João", "idade": 36 }
    del MinhaDicionario["idade"]
    
    #remover item
    MinhaDicionario = { "nome": "João", "idade": 36 }
    MinhaDicionario.pop("idade")
    
    #Copiar dicionário
    MinhaDicionario = { "nome": "João", "idade": 36 }
    MinhaDicionario2 = MinhaDicionario.copy()
    
    #Dicionário aninhado
    MinhaDicionario = {
      "PrimeiroDicionario": {
        "nome": "João",
        "idade": 36
      },
      "SegundoDicionario": {
        "nome": "Maria",
        "idade": 37
      }
    }
    
    #etc...
    #https://www.w3schools.com/python/python_dictionaries.asp
    ```
    
- **IF, ELIF, ELSE**
    
    ```python
    #IF e ELSE
    a = 33
    b = 200
    if b > a:
      print("b é maior que a")
    
    #Elif
    a = 33
    b = 33
    if b > a:
      print("b é maior que a")
    elif a == b:
      print("a e b são iguais")
    
    #Else
    a = 200
    b = 33
    if b > a:
      print("b é maior que a")
    elif a == b:
      print("a e b são iguais")
    else:
      print("a é maior que b")
    ```
    
- **WHILE**
    
    ```python
    #While
    i = 1
    while i < 6:
      print(i)
      i += 1
    
    #Break
    i = 1
    while i < 6:
      print(i)
      if i == 3:
        break
      i += 1
    
    #Continue
    i = 0
    while i < 6:
      i += 1
      if i == 3:
        continue
      print(i)
    ```
    
- **For**
    
    ```python
    #For
    frutas = ["maçã", "banana", "cereja"]
    for x in frutas:
      print(x)
    
    #For
    frutas = ["maçã", "banana", "cereja"]
    for x in frutas:
      print(x)
      if x == "banana":
        break
    
    #For
    frutas = ["maçã", "banana", "cereja"]
    for x in frutas:
      if x == "banana":
        continue
      print(x)
    
    #For
    for i in range(0, 10):
      pass
    ```
    
- **Funções**
    
    ```python
    #Funções
    def primeirafuncao():
      print("Olá, eu sou uma função")
    
    minhaprimeirafuncao()
    
    #Funções de soma
    def primeirafuncao():
      print(5 + 3)
    
    minhaprimeirafuncao()
    
    #Funções com parâmetros
    def primeirafuncao(nome):
      print(nome + " Refsnes")
    
    minhaprimeirafuncao("Emil")
    
    def entradadedados():
      idade = input("Digite sua idade: ")
      texto = 'Sua idade é {}'.format(idade)
      print(texto)
    
    entradadedados()
    ```
    
- **Arquivos**
    
    ```python
    #Arquivos
    arquivo = open('arquivo.txt', 'w') 
    #w = write (escrever) 
    #r = read (ler)  
    #a = append (adicionar)  
    #r+ = read and write (ler e escrever)
    arquivo.close()
    ```
    
- **Orientado a objetos**
    
    ```python
    
    ```
