##Objetivo do Curso
        Esse curso foi criado de forma a habilitar 
        os times internos da empresa a ler, processar,
        manipular e recriar informacoes de arquivos texto
        sem interven&ccedil;ao manual e de forma que cada operacao
        possa ser rastreavel, reutilizavel e automatizada.

        *O objetivo &eacute; eliminar a edi&ccedil;&atilde;o manual de arquivos que
        sejam recebidos ou enviados a clientes.*

##Objetivo do Programador
        ###Por que Bons Programadores s&atilde;o Pregui&ccedil;osos?

        Pregui&ccedil;osos, porque apenas programadores pregui&ccedil;osos ir&atilde;o querer 
        escrever os tipos de ferramentas que podem substituí-los no final. 
        Pregui&ccedil;osos, porque somente um programador pregui&ccedil;oso vai evitar 
        escrever código monótono e repetitivo – assim evitando redundância, 
        o inimigo da mantenabilidade e flexibilidade de software. 
        No mais, as ferramentas e processos que vêm disso, disparados pela pregui&ccedil;a, ir&atilde;o aumentar a produ&ccedil;&atilde;o.
        Claro, essa &eacute; apenas meia verdade. para um programador pregui&ccedil;o 
        para ser um bom programador, ele (ou ela) tamb&eacute;m devem ser 
        extremamente n&atilde;o-pregui&ccedil;osos quando &eacute; hora de aprender como ser pregui&ccedil;oso, 
        ou seja, quais ferramentas de software tornam seu trabalho mais f&aacute;cil, 
        quais t&eacute;cnicas evitam redundância, e como ele pode fazer seu 
        trabalho ter mais mantenabilidade e ser facilmente refatorado.


##Arquivos de Texto
        Arquivos texto sao a interface universal (Citacao)
        Por mais que existam protocolos, 
        formas eletronicas de envio e recebimento de informacao, 
        o formato de texto em que cada linha &eacute; considerado 
        um registro de informacao independente, ainda &eacute; a forma
        universao de transmissao e recebimento de dados entre computadores.



##Porque Python? - Caracteristicas
        Python &eacute; a ferramenta ideal para programadores preguicosos pois &eacute;:

        **Uma Linguagem de Scripts**: Nao precisa de um compilador, ou da gera&ccedil;&atilde;o de um executavel ininteligivel por um 
        ser humano, apenas &eacute; necess&aacute;rio editar um arquivo texto e rodar esse arquivo texto, e esse arquivo em geral
        o mesmo independente de qual sistema operacional ou computador tu esta usando 
        **Linguagem Simples**: Diferente de muitas linguagens que existem no mercado, o python foi pensado de forma a
        ser uma linguagem simples para tarefas simples e rapidas, entao diversos conceitos como Programacao Funcional,
        Orientacao a Objetos, estruturas complexas de dados, s&atilde;o presentes no Python, mas, n&atilde;o s&atilde;o **Obrigatorias** de 
        serem usadas como em outras linguagens
        **Roda em Qualquer Lugar**: O Python vem instalado em qualquer distribuicao linux e &eacute; facilmente instalado
        no windows baixando ele em python.org. Se utilizado exclusivamente as funcionalidades da linguagem, &eacute; garantido
        que qualquer programa que rode no windows, rode no linux e vice-versa.

##Python nao &eacute; para:
        Porem o programador ira passar trabalho se usar python para:

        **Linguagem para processamento em modo daemon (servidor)**: Um aplicativo em modo daemon, fica na maquina esperando por
        comandos ou dados a serem enviados, todo programa servidor numa maquina em geral roda nesse modo, todos os web servers rodam
        dessa forma. O Python n&atilde;o &eacute; feito para ser rodado nesse modo, apesar de muitos sites famosos como o Instagram, Quora, entre 
        outros, serem feitos com Python. Nesses sites, o python &eacute; chamado a cada requisicacao ou a cada N requisicoes, mas, jamais
        fica rodando no memoria por muito tempo
        **Modelagem de Dados Complexos**: Python &eacute; uma linguagem dinamicamente tipada entao &eacute; complicado e muito facil de se gerar bugs
        em aplicacoes com um modelo de negocio complexo como CRMs onde existe relacoes fixas entre entidades como Clientes, Contratos,
        Titulos, Telefones, e essas relacoes devem ser rigidas e facilmente identificaveis no codigo
        **Performance Computacional**: Python n&atilde;o &eacute; uma linguagem que tem multthread nativo na maquina, e utiliza um mecanismo arcaico chamado
        GIL ( Great Interpretor Lock ) que praticamente indisponibiliza ele para aplicacoes paralelas massivas, pois indiferentemente
        de executar operacoes em paralelo, ele executa apenas instrucoes sequencialmente (* dando a impressao de paralelismo *).
        Acesso a recursos fisicos da maquina: Python nao permite acesso a recusos da maquina de forma direta, em vez disso, utiliza 
        uma interface em C para permitir que programas em C sejam compilados com Python.

##Oque preciso para programar em python...
        Assumindo que estamos trabalhando no windows &eacute; necess&aacute;rio:
        1) Baixar o instalador de Python em Python.org (Nessa versao utilizaremos a versao 2.7)
        2) Um editor de texto, recomendo o notepad++ ou qualquer outro para windows.
        3) O Terminal do Windows (Command Prompt)

##Ola Mundo em Pyhon
        Mostrar o GIF animado

##Do que compoe um programa
        Um programa de computador &eacute; um conjunto de instrucoes que permite que um computador receba dados e execute acoes sobre os mesmos.
        Cada programa, independentemente de cada linguagem de programacao &eacute; composto dos seguintes componentes:
        * Variaveis: Basicamente, um nome que guarda uma informa&ccedil;&atilde;o que pode variar com o tempo. Uma variavel pode conter outras variaveis.
        * Fun&ccedil;ões: Um conjunto de instrucoes a ser executado e que retorna ou n&atilde;o um determinado valor.
        * Controle de Fluxo: Uma instru&ccedil;&atilde;o de decis&atilde;o a ser executado pelo programa, geralmente no formato: se isso, entao isso, senao aquilo.

##Oque &eacute; uma Variavel
        Um computador geralmente &eacute; composto por um processador que executa instrucoes de maquina, implementadas em transistores, uma memoria que
        armazena informacoes e diversos dispositivos de entrada e saida de dados que gravam ou leem dados da memoria do computador.

        Dentro de um programa de computador &eacute; necessario representar os dados que estao armazenados na memoria RAM do computador. No passado
        os programadores tinha uma tabela num caderno em papel em que registravam manualmente o endereco de memoria de cada informacao na memoria, dessa forma
        tinhamos algo como:
        ``
        #0000A3F -&gt; CodCliente (4 Bytes)
        #0000A44 -&gt; Nome (30 Bytes)
        ``
        e assim vai

        Mas, isso era muito dificil de manter e a medida que a manutencao nos programas ficou mais frequente, se tornou cada vez mais dificil manter o caderno 
        atualizado. Dessa forma, se criou o conceito de variavel, em que um nome (chamado de simbolo) sera utilizado para acessar essa regiao de memoria entao
        podemos dai fazer assim:
        ```
        nome = &quot;Guilherme&quot;
        entrada = 1000
        parcelas = 10
        valor_parcela = 120

        E melhor, podemos acessar esses dados e fazer calculos e colocar em outra variavel:

        total_acordo = entrada + (parcelas * valor_parcela)
        ```

##Tipo de Variavel
        Por&eacute;m, com o uso das variaveis, temos o problema que para o computador a memoria &eacute; apenas um conjunto de numeros de forma linear e nao existe 
        distincao entre a forma ou o conteudo semantico desses dados. Para isso, se criou o conceito de tipo de dados. Cujos tipos mais comuns s&atilde;o:

        **String**: Um conjunto de caracteres, como &quot;Guilherme&quot;, em que cada caracter representa 1 byte.
        **Inteiro**: Um numero inteiro som virgula. Ex. 100, 20, 21, 45 e assim por diante...
        **Ponto-Flutuante:** Um numero com virgula, Ex. 100.21, 10.90, 22.34 e assim vai
        **Logicas**: Contendo apenas os valores Sim ou Nao

##Criando uma variavel
	Em Python, por ser uma linguagem de script, n&atilde;o &eacute; necess&aacute;rio que declaremos as variaveis antes de usa-las. 
	Entao &eacute; apenas necess&aacute;rio atribuir um valor inicial e sair usando como nos exemplos abaixo:

	```
	nome = &quot;Guilherme&quot; # Variavel do Tipo String
	idade = 40 # Variavel do tipo inteiro
	divida = 1000102.2 # Variavel do tipo ponto-flutuante
	programador = True # Variavel logica       
	```
      
##Mostrando o valor de uma variavel
	Para se mostrar o valor de uma variavel &eacute; necessario que se use o comando print que imprime o valor de uma ou mais variaveis
	alem de poder tambem combinar essa escrita com outras expressoes por exemplo:

	```
	nome = &quot;Guilherme&quot; # Variavel do Tipo String
	idade = 40 # Variavel do tipo inteiro
	print nome 
	#Ira imprimir Guilherme

	print &#39;idade de &#39;, nome, &#39; eh &#39;, idade, &#39; anos &#39; 
	#Ira imprimir &quot;idade de Guilherme eh 40 anos&quot;

	print &#39;Significa que &#39;, nome, &#39; nasceu antes de &#39;, (datetime.today() - timedelta(days=40*365))
	#Ira imprimir: Significa que Guilherme nasceu antes de 1977-11-3
	```

##Convertendo de um tipo para o outro
	Importante salientar que apos ter sido atribuido o valor de uma variavel, ela tem um tipo e somente podemos 
	fazer operacoes entre variaveis de mesmo tipo, dessa forma:

	nome + idade # Dara um erro de tipo invalido

	Para isso &eacute; necessario converter o tipo de dados da variavel idade para um tipo compativel com nome, no 
	caso o tipo string, entao se fizermos

	nome + str(idade)

	ira funcionar corretamente

	As funcoes mais usadas sao:

	str() -&gt; Converte de um tipo qualquer para string
	int() -&gt; Converte de um tipo qualquer para inteiro
	float() -&gt; Converte de um tipo qualquer para ponto flutuante
	bool() -&gt; Converte de um tipo qualquer para booleano

	Cuidade para converter de um tipo que possa ser convertido para outro, por exemplo:

	int(&quot;Guilherme&quot;) # Ira dar um erro
	int(&quot;1&quot;) # Ira funcionar corretamente

##Variaveis Logicas
	Variaveis logicas sao um dos tipos mais comuns de variaveis e s&atilde;o essenciais para o controle do fluxo do programa,
	essas variaveis podem apenas conter os valores Sim/Nao, Verdadeiro/Falso, 0 ou 1.

	Sao produzidas por atribuicao simples:

	```
	eh_velho = True
	```
	Ou por Operacoes Logicas

	```
	eh_velho = idade &gt; 40
	```

	Os operadores logicos em Python s&atilde;o:
	```
	&gt;, &lt;, &lt;=, &gt;=, ==, !=, not , and, or
	```

	Podemos combinar diversas operacoes em uma so, da seguinte forma:

	```
	eh_velho = idade &gt; 40 and ( not nome == &quot;Guilherme&quot; )
	```

	Quer ira atribuir True a variavel: eh velho se a idade for maior que 40 e o nome nao for Guilherme.

##Exemplo pratico - Primeiro programa em Python
        Somando e mostrando

--------------------------------------------------------------

##Variaveis compostas e Estruturas de Dados
	Como podemos ver, usamos variaveis para representar posicoes na memoria, por&eacute;m declarar variaveis de forma individual
	&eacute; bastante penoso e ineficiente, dessa forma &eacute; necessario que possamos declarar conjuntos de variaveis e melhor variaveis
	que contem outras variaveis.

	Python tem varias estruturas de dados, mas, nesse curso iremos analisar os mais basicos que sao:
	* Lista : Uma lista &eacute; um conjunto de variaveis de mesmo tipo, por exemplo: Lista de CPFs, Lista de Contratos, Lista de Telefones e
	 assim por diante, por exemplo:
	```
	CPFS = [&#39;121232131&#39;,&#39;9832231&#39;,&#39;93468335&#39;,&#39;0001234562&#39;]
	```
	* Dicionario: Um conjunto de variaveis identificado por chave. Cada chave &eacute; unica e pode contar um tipo de dados distinto. Esse 
	tipo de dado eh fundamental para que possamos ter formas de dados complexas como os dados de um cliente. Por exemplo:
	```
	Cliente = { &#39;Nome&#39; : &#39;Guilherme&#39;, &#39;Idade&#39;: 40, &#39;Divida&#39; : 1212.09, &#39;Endereco&#39; : &#39;Rua XYZ, 60&#39; }
	```
	* Lista de Dicionarios: Podemos entao ter uma lista de dicionarios para poder manipular esses dados complexos:
	```
	lista_clientes = [
	 { &#39;Nome&#39; : &#39;Guilherme&#39;, &#39;Idade&#39;: 40, &#39;Divida&#39; : 1212.09, &#39;Endereco&#39; : &#39;Rua XYZ, 60&#39; }
	 { &#39;Nome&#39; : &#39;Manoel&#39;, &#39;Idade&#39;: 30, &#39;Divida&#39; : 912.19, &#39;Endereco&#39; : &#39;Rua ABC, 60&#39; }
	 { &#39;Nome&#39; : &#39;Felipe&#39;, &#39;Idade&#39;: 21, &#39;Divida&#39; : 2122.09, &#39;Endereco&#39; : &#39;Rua 123, 60&#39; }
	]
	```
	* Dicionario de Listas: Podemos tambem para dados muitos complexos ter listas como valores de um dicionario:
	```
	cliente_crm = {
	     &#39;Contratos&#39; : [&#39;010210/12&#39;, &#39;332122/12&#39;, &#39;898543/54&#39;],
	     &#39;Telefones&#39; : [&#39;514544333&#39;,&#39;3299987121&#39;,&#39;3199878121&#39;]
	}
	```
      
##Operacoes sobre uma lista
	Para criar uma lista, apenas abrimos e fechamos colchetes:
	```
	lista_telefones = []
	```
	Para adicionar valores a lista, podemos simplesmente somar uma lista a outra lista, por exemplo
	```
	lista_telefones = lista_telefones + [&#39;5133254546&#39;,&#39;32999754433&#39;]
	```
	Para saber o numero de entradas numa lista, usamos a funcao len():
	```
	print len(lista_telefones) # ira imprimir 2
	```
	Todo o acesso a valores &eacute; por indice, iniciando por zero, entao podemos fazer assim:
	```
	print lista_telefones[1] # ira imprimir 32999754433
	```
	Para remover um item, podemos usar o comando del com o indice da lista:
	```
	del lista_telefones[0] # ira remover &#39;5133254546&#39; 
	```


##Operacoes Avancadas de Lista:
	Podemos usar slicing para criar listas de listas, por exemplo:
	```
	valores = [&#39;1&#39;,&#39;2&#39;,&#39;3&#39;,&#39;4&#39;,&#39;5&#39;]
        print valores[3:]  # Ira imprimir [&#39;1&#39;,&#39;2&#39;,&#39;3&#39;]
        print valores[:3]  # Ira imprimir [&#39;4&#39;,&#39;5&#39;,&#39;6&#39;]
        print valores[3:5] # Ira imprimir [&#39;4&#39;,&#39;5&#39;]
        print valores[-1]  # Ira imprimir [&#39;6&#39;], indices negativos sao de tras pra frente
	```
        Muitas vezes recebemos uma string e precisamos criar uma lista separados por
        um caracter especial, como uma virgula no caso dos arquivos CSV. Para isso, usamos o comando
        split do tipo string:
	```
        &quot;10,11,12,13,14,15&quot;.split(&quot;,&quot;) # ira retornar: [&#39;10&#39;,&#39;11&#39;,&#39;12&#39;,&#39;13&#39;,&#39;14&#39;,&#39;15&#39;]
	```
        Da mesma forma que o comando join faz o inverso:
	```
        &quot;,&quot;.join([&#39;10&#39;,&#39;11&#39;,&#39;12&#39;,&#39;13&#39;,&#39;14&#39;,&#39;15&#39;]) # ira retornar: &quot;10,11,12,13,14,15&quot;
	```

##Operacoes sobre um Dicionario
	Operar um dicionario &eacute; mais simples que uma lista, &eacute; apenas 
	acessar pelo nome da chave.

	Para criar um dicionario:
	```
	cliente = {}
	```
	Para atribuir um valor:
	```
	cliente[&#39;nome&#39;]=&quot;Guilherme&quot;
	cliente[&#39;idade&#39;]=40
	cliente[&#39;divida&#39;]=1200.50
	```
	Para acessar o valor:
	```
	print(cliente[&#39;idade&#39;])
	```
	Para remover a chave eh apenas usar o operador del
	```
	del cliente[&#39;idade&#39;]
	```

##Lista de Dicionarios
	Como vimos, podemos usar dicionarios para criar estruturas de dados mais complexos
	No caso de ter varios dados, podemos ter uma lista de dicionarios, como abaixo:
	```
	lista_clientes = [
	 { &#39;Nome&#39; : &#39;Guilherme&#39;, &#39;Idade&#39;: 40, &#39;Divida&#39; : 1212.09, &#39;Endereco&#39; : &#39;Rua XYZ, 60&#39; }
	 { &#39;Nome&#39; : &#39;Manoel&#39;, &#39;Idade&#39;: 30, &#39;Divida&#39; : 912.19, &#39;Endereco&#39; : &#39;Rua ABC, 60&#39; }
	 { &#39;Nome&#39; : &#39;Felipe&#39;, &#39;Idade&#39;: 21, &#39;Divida&#39; : 2122.09, &#39;Endereco&#39; : &#39;Rua 123, 60&#39; }
	]
        print lista_clientes[1][&#39;Nome&#39;] # Vai imprimir &quot;Manoel&quot;
	```

##Dicionarios de Listas
	Podemos usar tambem listas nos diciionarios para aumentar a complexidade dos 
	dados.
	```
	cliente_crm = {
	     &#39;Contratos&#39; : [&#39;010210/12&#39;, &#39;332122/12&#39;, &#39;898543/54&#39;],
	     &#39;Telefones&#39; : [&#39;514544333&#39;,&#39;3299987121&#39;,&#39;3199878121&#39;]
	}

	print &quot;,&quot;.join(cliente_crm[&#39;Contratos&#39;]) # vai imprimir &quot;010210/12,332122/12,898543/54&quot;

	```

##Exemplo pratico de Estruturas de Dados

------------------------------------------------------------------------

##Manipulacao de Arquivos
	Um arquivo do ponto de vista do python &eacute; apenas uma sequencia de caracteres com
	tantos caracteres de controle e mostraveis na tela.

	Uma linha eh terminada pelo caracter \n 
	Cada coluna pode ser tanto delimitada pela distancia do ultimo caracter de quebra de linha
	ou por um caracter especifico.

##Lendo um Arquivo
	Para abrir um arquivo usamos um comando do tipo open que recebe tanto o nome do arquivo
	quanto o proposito para a abertura dele.
	```
	arq = open(&quot;cpfs.txt&quot;,&quot;r&quot;)
	```
	No caso acima,  abrimos o arquivo para leitura. É importante fechar o arquivo apos o uso para que 
	possa ser liberado. Para evitar que esquecamos de fechar o arquivo, &eacute; aconselhavel que usamos
	o comando com um conjunto do tipo with, assim:
	```
	with open(&quot;cpfs.txt&quot;,&quot;r&quot;) as arq:
	    ... Faz algo ...
	```
	Para facilitar a nossa vida, o python permite ler o arquivo e criar uma lista de linhas do arquivo
	```
	linhas_cpf = []
	with open(&quot;cpfs.txt&quot;,&quot;r&quot;) as arq:
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
	    if linha[14] == &#39;C&#39;:
		print linha	
	```
	Podemos criar uma lista a partir de uma interacao e uma selecao:
	```
	linhas_finais = []
	for linha in linhas_cpf:
	    if linha[14] == &#39;C&#39;:
	       linhas_finais.append(linha)
	```
	No caso acima a lista linhas_finais vai ter as linhas filtradas.


##Interando e Tomando Decisoes
	O Python tem uma funcionalidade muito legal para que possamos filtrar e criar listas a partir de listas ja existentes
	que &eacute; o &quot;list compreehension&quot;. 

	Funciona assim:
	```
	linhas__finais = [x for x in linhas_cpf where x[14]==&#39;C&#39;]
	```
	Ou seja, para cada linha x in linhas_cpf, me retorna a linha aonde o caracter 14 seja x. O comando acima &eacute; exatamente o 
	mesmo que: 
	```
	linhas_finais = []
	for linha in linhas_cpf:
	    if linha[14] == &#39;C&#39;:
	       linhas_finais.append(linha)
	```

##Gravando no Arquivo
	Para Escrever as linhas filtradas num arquivo, &eacute; muito facil, com o mesmo mecanismo 
	que lemos, mas, com o comando de writelines e abrindo o arquivo para escrita com &quot;w&quot;
	```

	linhas_cpf = []
	with open(&quot;cpfs.txt&quot;,&quot;r&quot;) as arq:
	     linhas_cpf = arq.readlines()

	linhas__finais = [x for x in linhas_cpf where x[14]==&#39;C&#39;]
	with open(&quot;cpfs_litrados.txt&quot;,&quot;w&quot;) as arq:
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
	nome = &#39;Guilherme Poisl Bencke&#39;
	print(&#39;Poisl&#39; in nome) # retorno True
	print(nome.startswith(&#39;Guilherme&#39;) # retorna True
	print(nome.endswith(&#39;Bencke&#39;) # retorno True
	```

	###Conversao de Maius.Minusc.
	```
	nome = &#39;Guilherme Poisl Bencke&#39;
        nome.upper() # Retorna &quot;GUILHERME POISL BENCKE&quot;
        nome.lower() # Retorno &quot;guilherme poisl bencke&quot;
	```

        ###Removendo e tirando caracteres de inicio/fim
	```
        cpf=&quot;12234121&quot;
        cpf.rjust(20,&#39;0&#39;) # Vai retornar 0000000000000012234121

        cpf=&quot;000012234121&quot;
        cpf.strip(&quot;0&quot;) $ Vai retornar 12234121
	```

        ###Sabendo a posicao de uma string em outra string
	nome = &#39;Guilherme Poisl Bencke&#39;
        nome.index(&quot;Poisl&quot;) # Retorna 10 
  



