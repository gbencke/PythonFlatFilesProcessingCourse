##Objetivo do Curso
        Esse curso foi criado de forma a habilitar 
        os times internos da empresa a ler, processar,
        manipular e recriar informacoes de arquivos texto
        sem interven�ao manual e de forma que cada operacao
        possa ser rastreavel, reutilizavel e automatizada.

        *O objetivo � eliminar a edi��o manual de arquivos que
        sejam recebidos ou enviados a clientes.*

##Objetivo do Programador
        ###Por que Bons Programadores s�o Pregui�osos?

        Pregui�osos, porque apenas programadores pregui�osos ir�o querer 
        escrever os tipos de ferramentas que podem substitu�-los no final. 
        Pregui�osos, porque somente um programador pregui�oso vai evitar 
        escrever c�digo mon�tono e repetitivo � assim evitando redund�ncia, 
        o inimigo da mantenabilidade e flexibilidade de software. 
        No mais, as ferramentas e processos que v�m disso, disparados pela pregui�a, ir�o aumentar a produ��o.
        Claro, essa � apenas meia verdade. para um programador pregui�o 
        para ser um bom programador, ele (ou ela) tamb�m devem ser 
        extremamente n�o-pregui�osos quando � hora de aprender como ser pregui�oso, 
        ou seja, quais ferramentas de software tornam seu trabalho mais f�cil, 
        quais t�cnicas evitam redund�ncia, e como ele pode fazer seu 
        trabalho ter mais mantenabilidade e ser facilmente refatorado.


##Arquivos de Texto
        Arquivos texto sao a interface universal (Citacao)
        Por mais que existam protocolos, 
        formas eletronicas de envio e recebimento de informacao, 
        o formato de texto em que cada linha � considerado 
        um registro de informacao independente, ainda � a forma
        universao de transmissao e recebimento de dados entre computadores.



##Porque Python? - Caracteristicas
        Python � a ferramenta ideal para programadores preguicosos pois �:

        **Uma Linguagem de Scripts**: Nao precisa de um compilador, ou da gera��o de um executavel ininteligivel por um 
        ser humano, apenas � necess�rio editar um arquivo texto e rodar esse arquivo texto, e esse arquivo em geral
        o mesmo independente de qual sistema operacional ou computador tu esta usando 
        **Linguagem Simples**: Diferente de muitas linguagens que existem no mercado, o python foi pensado de forma a
        ser uma linguagem simples para tarefas simples e rapidas, entao diversos conceitos como Programacao Funcional,
        Orientacao a Objetos, estruturas complexas de dados, s�o presentes no Python, mas, n�o s�o **Obrigatorias** de 
        serem usadas como em outras linguagens
        **Roda em Qualquer Lugar**: O Python vem instalado em qualquer distribuicao linux e � facilmente instalado
        no windows baixando ele em python.org. Se utilizado exclusivamente as funcionalidades da linguagem, � garantido
        que qualquer programa que rode no windows, rode no linux e vice-versa.

##Python nao � para:
        Porem o programador ira passar trabalho se usar python para:

        **Linguagem para processamento em modo daemon (servidor)**: Um aplicativo em modo daemon, fica na maquina esperando por
        comandos ou dados a serem enviados, todo programa servidor numa maquina em geral roda nesse modo, todos os web servers rodam
        dessa forma. O Python n�o � feito para ser rodado nesse modo, apesar de muitos sites famosos como o Instagram, Quora, entre 
        outros, serem feitos com Python. Nesses sites, o python � chamado a cada requisicacao ou a cada N requisicoes, mas, jamais
        fica rodando no memoria por muito tempo
        **Modelagem de Dados Complexos**: Python � uma linguagem dinamicamente tipada entao � complicado e muito facil de se gerar bugs
        em aplicacoes com um modelo de negocio complexo como CRMs onde existe relacoes fixas entre entidades como Clientes, Contratos,
        Titulos, Telefones, e essas relacoes devem ser rigidas e facilmente identificaveis no codigo
        **Performance Computacional**: Python n�o � uma linguagem que tem multthread nativo na maquina, e utiliza um mecanismo arcaico chamado
        GIL ( Great Interpretor Lock ) que praticamente indisponibiliza ele para aplicacoes paralelas massivas, pois indiferentemente
        de executar operacoes em paralelo, ele executa apenas instrucoes sequencialmente (* dando a impressao de paralelismo *).
        Acesso a recursos fisicos da maquina: Python nao permite acesso a recusos da maquina de forma direta, em vez disso, utiliza 
        uma interface em C para permitir que programas em C sejam compilados com Python.

##Oque preciso para programar em python...
        Assumindo que estamos trabalhando no windows � necess�rio:
        1) Baixar o instalador de Python em Python.org (Nessa versao utilizaremos a versao 2.7)
        2) Um editor de texto, recomendo o notepad++ ou qualquer outro para windows.
        3) O Terminal do Windows (Command Prompt)

##Ola Mundo em Pyhon
        Mostrar o GIF animado

##Do que compoe um programa
        Um programa de computador � um conjunto de instrucoes que permite que um computador receba dados e execute acoes sobre os mesmos.
        Cada programa, independentemente de cada linguagem de programacao � composto dos seguintes componentes:
        * Variaveis: Basicamente, um nome que guarda uma informa��o que pode variar com o tempo. Uma variavel pode conter outras variaveis.
        * Fun��es: Um conjunto de instrucoes a ser executado e que retorna ou n�o um determinado valor.
        * Controle de Fluxo: Uma instru��o de decis�o a ser executado pelo programa, geralmente no formato: se isso, entao isso, senao aquilo.

##Oque � uma Variavel
        Um computador geralmente � composto por um processador que executa instrucoes de maquina, implementadas em transistores, uma memoria que
        armazena informacoes e diversos dispositivos de entrada e saida de dados que gravam ou leem dados da memoria do computador.

        Dentro de um programa de computador � necessario representar os dados que estao armazenados na memoria RAM do computador. No passado
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
        Por�m, com o uso das variaveis, temos o problema que para o computador a memoria � apenas um conjunto de numeros de forma linear e nao existe 
        distincao entre a forma ou o conteudo semantico desses dados. Para isso, se criou o conceito de tipo de dados. Cujos tipos mais comuns s�o:

        **String**: Um conjunto de caracteres, como "Guilherme", em que cada caracter representa 1 byte.
        **Inteiro**: Um numero inteiro som virgula. Ex. 100, 20, 21, 45 e assim por diante...
        **Ponto-Flutuante:** Um numero com virgula, Ex. 100.21, 10.90, 22.34 e assim vai
        **Logicas**: Contendo apenas os valores Sim ou Nao

##Criando uma variavel
	Em Python, por ser uma linguagem de script, n�o � necess�rio que declaremos as variaveis antes de usa-las. 
	Entao � apenas necess�rio atribuir um valor inicial e sair usando como nos exemplos abaixo:

	```
	nome = "Guilherme" # Variavel do Tipo String
	idade = 40 # Variavel do tipo inteiro
	divida = 1000102.2 # Variavel do tipo ponto-flutuante
	programador = True # Variavel logica       
	```
      
##Mostrando o valor de uma variavel
        Comando Print

##Convertendo de um tipo para o outro

##Variaveis Logicas

##Operacoes Logicas

##Exemplo pratico - Primeiro programa em Python
        Somando e mostrando

--------------------------------------------------------------

##Variaveis compostas
        Lista 
        Dicionario
        Lista de Dicionarios
        Dicionario de Listas
      
##Oque � uma Lista

##Operacoes sobre uma lista
        Adicionando a lista
        Acessando valores
        Removendo na lista
        Criando uma lista de uma lista
        Criando uma lista de uma String

##Oque � um Dicionario

##Operacoes sobre um Dicionario
        Adicionando um valor no Dicionario
        Acessando um valor no Dicionario
        Removendo um valor do Dicionario

##Lista de Dicionarios
        Para que? 

##Dicionarios de Listas
        Porque?

##Dicionario de Listas de Dicionarios
        Porque?

##Exemplo pratico de Estruturas de Dados

------------------------------------------------------------------------

##Manipulacao de Arquivos
        Porque manipular arquivos

##Lendo um Arquivo
        Lista de Linhas 

##Instrucoes de Controle
        Iterando sobre as linhas
        Criando uma nova lista 

##Gravando no Arquivo
        Escrevendo a Lista num arquivo

##Exemplo Pratico de Arquivos

-------------------------------------------------------------------------

##Controle de Fluxo

##Afinal oque a Gente tem q fazer mesmo??

##Instrucoes de Loop (For, While)

##Controle do Loop
        break, continue

##Instrucao de Decisao Logica (If)

##Exemplo Pratico de Controle de Fluxo

-------------------------------------------------------------------------

##Manipulacao de Strings.

##Concatenar Strings

##Tirando espacoe

##Adicionando espacos

##Dividindo strings em Listas

-------------------------------------------------------------------------

##Funcoes e Comandos Utilitarios

##Calculando Datas

##Pesquisando Arquivos nas Pastas

##Manipulando arquivos


