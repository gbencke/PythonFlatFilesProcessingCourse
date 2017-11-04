##Objetivo do Curso
        Esse curso foi criado de forma a habilitar 
        os times internos da empresa a ler, processar,
        manipular e recriar informacoes de arquivos texto
        sem intervençao manual e de forma que cada operacao
        possa ser rastreavel, reutilizavel e automatizada.

        *O objetivo é eliminar a edição manual de arquivos que
        sejam recebidos ou enviados a clientes.*

##Objetivo do Programador
        ###Por que Bons Programadores são Preguiçosos?

        Preguiçosos, porque apenas programadores preguiçosos irão querer 
        escrever os tipos de ferramentas que podem substituí-los no final. 
        Preguiçosos, porque somente um programador preguiçoso vai evitar 
        escrever código monótono e repetitivo – assim evitando redundância, 
        o inimigo da mantenabilidade e flexibilidade de software. 
        No mais, as ferramentas e processos que vêm disso, disparados pela preguiça, irão aumentar a produção.
        Claro, essa é apenas meia verdade. para um programador preguiço 
        para ser um bom programador, ele (ou ela) também devem ser 
        extremamente não-preguiçosos quando é hora de aprender como ser preguiçoso, 
        ou seja, quais ferramentas de software tornam seu trabalho mais fácil, 
        quais técnicas evitam redundância, e como ele pode fazer seu 
        trabalho ter mais mantenabilidade e ser facilmente refatorado.


##Arquivos de Texto
        Arquivos texto sao a interface universal (Citacao)
        Por mais que existam protocolos, 
        formas eletronicas de envio e recebimento de informacao, 
        o formato de texto em que cada linha é considerado 
        um registro de informacao independente, ainda é a forma
        universao de transmissao e recebimento de dados entre computadores.



##Porque Python? - Caracteristicas
        Python é a ferramenta ideal para programadores preguicosos pois é:

        **Uma Linguagem de Scripts**: Nao precisa de um compilador, ou da geração de um executavel ininteligivel por um 
        ser humano, apenas é necessário editar um arquivo texto e rodar esse arquivo texto, e esse arquivo em geral
        o mesmo independente de qual sistema operacional ou computador tu esta usando 
        **Linguagem Simples**: Diferente de muitas linguagens que existem no mercado, o python foi pensado de forma a
        ser uma linguagem simples para tarefas simples e rapidas, entao diversos conceitos como Programacao Funcional,
        Orientacao a Objetos, estruturas complexas de dados, são presentes no Python, mas, não são **Obrigatorias** de 
        serem usadas como em outras linguagens
        **Roda em Qualquer Lugar**: O Python vem instalado em qualquer distribuicao linux e é facilmente instalado
        no windows baixando ele em python.org. Se utilizado exclusivamente as funcionalidades da linguagem, é garantido
        que qualquer programa que rode no windows, rode no linux e vice-versa.

##Python nao é para:
        Porem o programador ira passar trabalho se usar python para:

        **Linguagem para processamento em modo daemon (servidor)**: Um aplicativo em modo daemon, fica na maquina esperando por
        comandos ou dados a serem enviados, todo programa servidor numa maquina em geral roda nesse modo, todos os web servers rodam
        dessa forma. O Python não é feito para ser rodado nesse modo, apesar de muitos sites famosos como o Instagram, Quora, entre 
        outros, serem feitos com Python. Nesses sites, o python é chamado a cada requisicacao ou a cada N requisicoes, mas, jamais
        fica rodando no memoria por muito tempo
        **Modelagem de Dados Complexos**: Python é uma linguagem dinamicamente tipada entao é complicado e muito facil de se gerar bugs
        em aplicacoes com um modelo de negocio complexo como CRMs onde existe relacoes fixas entre entidades como Clientes, Contratos,
        Titulos, Telefones, e essas relacoes devem ser rigidas e facilmente identificaveis no codigo
        **Performance Computacional**: Python não é uma linguagem que tem multthread nativo na maquina, e utiliza um mecanismo arcaico chamado
        GIL ( Great Interpretor Lock ) que praticamente indisponibiliza ele para aplicacoes paralelas massivas, pois indiferentemente
        de executar operacoes em paralelo, ele executa apenas instrucoes sequencialmente (* dando a impressao de paralelismo *).
        Acesso a recursos fisicos da maquina: Python nao permite acesso a recusos da maquina de forma direta, em vez disso, utiliza 
        uma interface em C para permitir que programas em C sejam compilados com Python.

##Oque preciso para programar em python...
        Assumindo que estamos trabalhando no windows é necessário:
        1) Baixar o instalador de Python em Python.org (Nessa versao utilizaremos a versao 2.7)
        2) Um editor de texto, recomendo o notepad++ ou qualquer outro para windows.
        3) O Terminal do Windows (Command Prompt)

##Ola Mundo em Pyhon
        Mostrar o GIF animado

##Do que compoe um programa
        Um programa de computador é um conjunto de instrucoes que permite que um computador receba dados e execute acoes sobre os mesmos.
        Cada programa, independentemente de cada linguagem de programacao é composto dos seguintes componentes:
        * Variaveis: Basicamente, um nome que guarda uma informação que pode variar com o tempo. Uma variavel pode conter outras variaveis.
        * Funções: Um conjunto de instrucoes a ser executado e que retorna ou não um determinado valor.
        * Controle de Fluxo: Uma instrução de decisão a ser executado pelo programa, geralmente no formato: se isso, entao isso, senao aquilo.

##Oque é uma Variavel
        Um computador geralmente é composto por um processador que executa instrucoes de maquina, implementadas em transistores, uma memoria que
        armazena informacoes e diversos dispositivos de entrada e saida de dados que gravam ou leem dados da memoria do computador.

        Dentro de um programa de computador é necessario representar os dados que estao armazenados na memoria RAM do computador. No passado
        os programadores tinha uma tabela num caderno em papel em que registravam manualmente o endereco de memoria de cada informacao na memoria, dessa forma
        tinhamos algo como:
        ``
        #0000A3F -> CodCliente (4 Bytes)
        #0000A44 -> Nome (30 Bytes)
        ``
        e assim vai

        Mas, isso era muito dificil de manter e a medida que a manutencao nos programas ficou mais frequente, se tornou cada vez mais dificil manter o caderno 
        atualizado. Dessa forma, se criou o conceito de variavel, em que um nome (chamado de simbolo) sera utilizado para acessar essa regiao de memoria entao
        podemos dai fazer assim:
        ```
        nome = "Guilherme"
        entrada = 1000
        parcelas = 10
        valor_parcela = 120

        E melhor, podemos acessar esses dados e fazer calculos e colocar em outra variavel:

        total_acordo = entrada + (parcelas * valor_parcela)
        ```

##Tipo de Variavel
        Porém, com o uso das variaveis, temos o problema que para o computador a memoria é apenas um conjunto de numeros de forma linear e nao existe 
        distincao entre a forma ou o conteudo semantico desses dados. Para isso, se criou o conceito de tipo de dados. Cujos tipos mais comuns são:

        **String**: Um conjunto de caracteres, como "Guilherme", em que cada caracter representa 1 byte.
        **Inteiro**: Um numero inteiro som virgula. Ex. 100, 20, 21, 45 e assim por diante...
        **Ponto-Flutuante:** Um numero com virgula, Ex. 100.21, 10.90, 22.34 e assim vai
        **Logicas**: Contendo apenas os valores Sim ou Nao

##Criando uma variavel
	Em Python, por ser uma linguagem de script, não é necessário que declaremos as variaveis antes de usa-las. 
	Entao é apenas necessário atribuir um valor inicial e sair usando como nos exemplos abaixo:

	```
	nome = "Guilherme" # Variavel do Tipo String
	idade = 40 # Variavel do tipo inteiro
	divida = 1000102.2 # Variavel do tipo ponto-flutuante
	programador = True # Variavel logica       
	```
      
##Mostrando o valor de uma variavel
	Para se mostrar o valor de uma variavel é necessario que se use o comando print que imprime o valor de uma ou mais variaveis
	alem de poder tambem combinar essa escrita com outras expressoes por exemplo:

	```
	nome = "Guilherme" # Variavel do Tipo String
	idade = 40 # Variavel do tipo inteiro
	print nome 
	#Ira imprimir Guilherme

	print 'idade de ', nome, ' eh ', idade, ' anos ' 
	#Ira imprimir "idade de Guilherme eh 40 anos"

	print 'Significa que ', nome, ' nasceu antes de ', (datetime.today() - timedelta(days=40*365))
	#Ira imprimir: Significa que Guilherme nasceu antes de 1977-11-3
	```

##Convertendo de um tipo para o outro
	Importante salientar que apos ter sido atribuido o valor de uma variavel, ela tem um tipo e somente podemos 
	fazer operacoes entre variaveis de mesmo tipo, dessa forma:

	nome + idade # Dara um erro de tipo invalido

	Para isso é necessario converter o tipo de dados da variavel idade para um tipo compativel com nome, no 
	caso o tipo string, entao se fizermos

	nome + str(idade)

	ira funcionar corretamente

	As funcoes mais usadas sao:

	str() -> Converte de um tipo qualquer para string
	int() -> Converte de um tipo qualquer para inteiro
	float() -> Converte de um tipo qualquer para ponto flutuante
	bool() -> Converte de um tipo qualquer para booleano

	Cuidade para converter de um tipo que possa ser convertido para outro, por exemplo:

	int("Guilherme") # Ira dar um erro
	int("1") # Ira funcionar corretamente

##Variaveis Logicas
	Variaveis logicas sao um dos tipos mais comuns de variaveis e são essenciais para o controle do fluxo do programa,
	essas variaveis podem apenas conter os valores Sim/Nao, Verdadeiro/Falso, 0 ou 1.

	Sao produzidas por atribuicao simples:

	```
	eh_velho = True
	```
	Ou por Operacoes Logicas

	```
	eh_velho = idade > 40
	```

	Os operadores logicos em Python são:
	```
	>, <, <=, >=, ==, !=, not , and, or
	```

	Podemos combinar diversas operacoes em uma so, da seguinte forma:

	```
	eh_velho = idade > 40 and ( not nome == "Guilherme" )
	```

	Quer ira atribuir True a variavel: eh velho se a idade for maior que 40 e o nome nao for Guilherme.

##Exemplo pratico - Primeiro programa em Python
        Somando e mostrando

--------------------------------------------------------------

##Variaveis compostas e Estruturas de Dados
	Como podemos ver, usamos variaveis para representar posicoes na memoria, porém declarar variaveis de forma individual
	é bastante penoso e ineficiente, dessa forma é necessario que possamos declarar conjuntos de variaveis e melhor variaveis
	que contem outras variaveis.

	Python tem varias estruturas de dados, mas, nesse curso iremos analisar os mais basicos que sao:
	* Lista : Uma lista é um conjunto de variaveis de mesmo tipo, por exemplo: Lista de CPFs, Lista de Contratos, Lista de Telefones e
	 assim por diante, por exemplo:
	```
	CPFS = ['121232131','9832231','93468335','0001234562']
	```
	* Dicionario: Um conjunto de variaveis identificado por chave. Cada chave é unica e pode contar um tipo de dados distinto. Esse 
	tipo de dado eh fundamental para que possamos ter formas de dados complexas como os dados de um cliente. Por exemplo:
	```
	Cliente = { 'Nome' : 'Guilherme', 'Idade': 40, 'Divida' : 1212.09, 'Endereco' : 'Rua XYZ, 60' }
	```
	* Lista de Dicionarios: Podemos entao ter uma lista de dicionarios para poder manipular esses dados complexos:
	```
	lista_clientes = [
	 { 'Nome' : 'Guilherme', 'Idade': 40, 'Divida' : 1212.09, 'Endereco' : 'Rua XYZ, 60' }
	 { 'Nome' : 'Manoel', 'Idade': 30, 'Divida' : 912.19, 'Endereco' : 'Rua ABC, 60' }
	 { 'Nome' : 'Felipe', 'Idade': 21, 'Divida' : 2122.09, 'Endereco' : 'Rua 123, 60' }
	]
	```
	* Dicionario de Listas: Podemos tambem para dados muitos complexos ter listas como valores de um dicionario:
	```
	cliente_crm = {
	     'Contratos' : ['010210/12', '332122/12', '898543/54'],
	     'Telefones' : ['514544333','3299987121','3199878121']
	}
	```
      
##Operacoes sobre uma lista
	Para criar uma lista, apenas abrimos e fechamos colchetes:
	```
	lista_telefones = []
	```
	Para adicionar valores a lista, podemos simplesmente somar uma lista a outra lista, por exemplo
	```
	lista_telefones = lista_telefones + ['5133254546','32999754433']
	```
	Para saber o numero de entradas numa lista, usamos a funcao len():
	```
	print len(lista_telefones) # ira imprimir 2
	```
	Todo o acesso a valores é por indice, iniciando por zero, entao podemos fazer assim:
	```
	print lista_telefones[1] # ira imprimir 32999754433
	```
	Para remover um item, podemos usar o comando del com o indice da lista:
	```
	del lista_telefones[0] # ira remover '5133254546' 
	```


##Operacoes Avancadas de Lista:
	Podemos usar slicing para criar listas de listas, por exemplo:
	```
	valores = ['1','2','3','4','5']
        print valores[3:]  # Ira imprimir ['1','2','3']
        print valores[:3]  # Ira imprimir ['4','5','6']
        print valores[3:5] # Ira imprimir ['4','5']
        print valores[-1]  # Ira imprimir ['6'], indices negativos sao de tras pra frente
	```
        Muitas vezes recebemos uma string e precisamos criar uma lista separados por
        um caracter especial, como uma virgula no caso dos arquivos CSV. Para isso, usamos o comando
        split do tipo string:
	```
        "10,11,12,13,14,15".split(",") # ira retornar: ['10','11','12','13','14','15']
	```
        Da mesma forma que o comando join faz o inverso:
	```
        ",".join(['10','11','12','13','14','15']) # ira retornar: "10,11,12,13,14,15"
	```

##Operacoes sobre um Dicionario
	Operar um dicionario é mais simples que uma lista, é apenas 
	acessar pelo nome da chave.

	Para criar um dicionario:
	```
	cliente = {}
	```
	Para atribuir um valor:
	```
	cliente['nome']="Guilherme"
	cliente['idade']=40
	cliente['divida']=1200.50
	```
	Para acessar o valor:
	```
	print(cliente['idade'])
	```
	Para remover a chave eh apenas usar o operador del
	```
	del cliente['idade']
	```

##Lista de Dicionarios
	Como vimos, podemos usar dicionarios para criar estruturas de dados mais complexos
	No caso de ter varios dados, podemos ter uma lista de dicionarios, como abaixo:
	```
	lista_clientes = [
	 { 'Nome' : 'Guilherme', 'Idade': 40, 'Divida' : 1212.09, 'Endereco' : 'Rua XYZ, 60' }
	 { 'Nome' : 'Manoel', 'Idade': 30, 'Divida' : 912.19, 'Endereco' : 'Rua ABC, 60' }
	 { 'Nome' : 'Felipe', 'Idade': 21, 'Divida' : 2122.09, 'Endereco' : 'Rua 123, 60' }
	]
        print lista_clientes[1]['Nome'] # Vai imprimir "Manoel"
	```

##Dicionarios de Listas
	Podemos usar tambem listas nos diciionarios para aumentar a complexidade dos 
	dados.
	```
	cliente_crm = {
	     'Contratos' : ['010210/12', '332122/12', '898543/54'],
	     'Telefones' : ['514544333','3299987121','3199878121']
	}

	print ",".join(cliente_crm['Contratos']) # vai imprimir "010210/12,332122/12,898543/54"

	```

##Exemplo pratico de Estruturas de Dados

------------------------------------------------------------------------

##Manipulacao de Arquivos
	Um arquivo do ponto de vista do python é apenas uma sequencia de caracteres com
	tantos caracteres de controle e mostraveis na tela.

	Uma linha eh terminada pelo caracter \n 
	Cada coluna pode ser tanto delimitada pela distancia do ultimo caracter de quebra de linha
	ou por um caracter especifico.

##Lendo um Arquivo
	Para abrir um arquivo usamos um comando do tipo open que recebe tanto o nome do arquivo
	quanto o proposito para a abertura dele.
	```
	arq = open("cpfs.txt","r")
	```
	No caso acima,  abrimos o arquivo para leitura. É importante fechar o arquivo apos o uso para que 
	possa ser liberado. Para evitar que esquecamos de fechar o arquivo, é aconselhavel que usamos
	o comando com um conjunto do tipo with, assim:
	```
	with open("cpfs.txt","r") as arq:
	    ... Faz algo ...
	```
	Para facilitar a nossa vida, o python permite ler o arquivo e criar uma lista de linhas do arquivo
	```
	linhas_cpf = []
	with open("cpfs.txt","r") as arq:
	     linhas_cpf = arq.readlines()
	```
	O codigo acima ira abrir o arquivo, ler as linhas, e colocar as linhas na lista linhas_cpf, 
	e finalimente fechar o arquivo.

	Agora que temos todas as linhas numa lista, podemos trabalhar com esse arquivo.


##Instrucoes de Controle
	Bem, agora que temos uma lista com as linhas do arquivo, precisamos ler elas, mas, com os metodos que possuimos
	apenas podemos fazer isso linha a linha ou fazer listas de listas.

	O Python permite loopar a cada item da item usando a instrucao for. Dessa forma, podemos entao executar comandos
	individualmente a cada linha. Como por exemplo:
	```
	for linha in linhas_cpf:
	    print linha
	```
	Esse trecho de codigo ira imprimir na tela todas as linhas da lista: linhas__cpf. Se desejarmos as ultimas 50
	linhas podemos usar slicing tambem.
	```
	for linha in linhas_cpf[-3:]:
	    print linha
	```

##Tomando Decisoes 
	Porem, digamos que queremos apenas imprimir as linhas cujo caracter 14 na linha seja o C, ou seja Cartao de Credito,
	Para isso, podemos usar a instrucao if com uma condicao logica para filtrar as linhas necessarias:
	```
	for linha in linhas_cpf:
	    if linha[14] == 'C':
		print linha	
	```
	Podemos criar uma lista a partir de uma interacao e uma selecao:
	```
	linhas_finais = []
	for linha in linhas_cpf:
	    if linha[14] == 'C':
	       linhas_finais.append(linha)
	```
	No caso acima a lista linhas_finais vai ter as linhas filtradas.


##Interando e Tomando Decisoes
	O Python tem uma funcionalidade muito legal para que possamos filtrar e criar listas a partir de listas ja existentes
	que é o "list compreehension". 

	Funciona assim:
	```
	linhas__finais = [x for x in linhas_cpf where x[14]=='C']
	```
	Ou seja, para cada linha x in linhas_cpf, me retorna a linha aonde o caracter 14 seja x. O comando acima é exatamente o 
	mesmo que: 
	```
	linhas_finais = []
	for linha in linhas_cpf:
	    if linha[14] == 'C':
	       linhas_finais.append(linha)
	```

##Gravando no Arquivo
	Para Escrever as linhas filtradas num arquivo, é muito facil, com o mesmo mecanismo 
	que lemos, mas, com o comando de writelines e abrindo o arquivo para escrita com "w"
	```

	linhas_cpf = []
	with open("cpfs.txt","r") as arq:
	     linhas_cpf = arq.readlines()

	linhas__finais = [x for x in linhas_cpf where x[14]=='C']
	with open("cpfs_litrados.txt","w") as arq:
	     arq.writelines()

	```
	No exemplo acima, podemos ver que lemos as linhas, 
        filtramos as linhas lidas dos arquivo, e escrevemos as linhas
	num segundo arquivo.

##Exemplo Pratico de Arquivos

-------------------------------------------------------------------------

##Manipulacao de Strings.

	O Python tem diversos comandos para fazer a nossa vida facil para manipular
	strings, vou tentar apenas listar alguns:
	
        ###Teste de Conteudo
	```
	nome = 'Guilherme Poisl Bencke'
	print('Poisl' in nome) # retorno True
	print(nome.startswith('Guilherme') # retorna True
	print(nome.endswith('Bencke') # retorno True
	```

	###Conversao de Maius.Minusc.
	```
	nome = 'Guilherme Poisl Bencke'
        nome.upper() # Retorna "GUILHERME POISL BENCKE"
        nome.lower() # Retorno "guilherme poisl bencke"
	```

        ###Removendo e tirando caracteres de inicio/fim
	```
        cpf="12234121"
        cpf.rjust(20,'0') # Vai retornar 0000000000000012234121

        cpf="000012234121"
        cpf.strip("0") $ Vai retornar 12234121
	```

        ###Sabendo a posicao de uma string em outra string
	nome = 'Guilherme Poisl Bencke'
        nome.index("Poisl") # Retorna 10 
  



