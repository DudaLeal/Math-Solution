# Math-Solution
#Projeto final da disciplina de computação 1 da Universidade Federal do Rio de Janeiro
#Uniiversidade Federal do Rio de Janeiro
#Computação 1
#Eduarda Leal de Carvalho

import math
#É importado o módulo math para que ele auxilie e facilite ao usuário em certos tipos de contas.
#É solicitado ao usuário para que ele(a) forneça seu nome.
#Logo em seguida, irá ser impresso na tela uma frase de boas vindas.
nome = input("Por favor digite seu nome: \n")
print("\t BEM VINDO",nome.upper())
print("Para continuar, escolha uma das seguintes opções:\n")
#Para que o usuário continue e realize o que deseja, irá ser fornecido uma lista de opções para que seja escolhida.
while True:    
    inicio = input("Para operações básicas digite '1'\n"
                  "Para conversor de medidas digite '2'\n"
                  "Para geometria digite '3'\n"
                  "Para álgebra digite '4'\n"                  
                  "Para sair do programa digite 'sair' \n")
    if inicio == 'sair':
#Sendo digitado pelo usuário 'sair', o programa será automaticamente fechado. 
        print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n ")
        exit()
    if inicio == '1':
# se for escolhido "1", irá ser redirecionado para operações básicas e será mostrado uma nova lista com os nomes das operações e os seus sinais correspondentes para serem chamadas.
        print("\t CONTAS BÁSICAS: \n")
        operacao = input("Digite a operação:\n '+' para Soma \n '-' para Subtração\n '/' para Divisão \n '*' para Multiplicação \n 'raiz' para Raiz quadrada \n '**' para Potenciação\n ")
        resultado = float
        if operacao == '+':
# "+" representa a conta Soma.
            print(" Soma é uma operação que permite adicionar uma quantidade a outra(s).\n ")
            primeiro = input("Digite o primeiro número:\n ")
            segundo = input("Digite o segundo número:\n ")
            resultado = float(primeiro) + float(segundo)
            print(" O resultado é: " ,resultado)
        elif operacao == "-":
# "-" representa a conta Subtração.
            print(" Subtração é uma operação de subtrair (separar uma parte de um todo, tirar, eliminar, baixar, reduzir ou cortar algo).\n ")
            primeiro = input("Digite o primeiro número:\n ")
            segundo = input("Digite o segundo número:\n ")
            resultado = float(primeiro) - float(segundo)
            print(" O resultado é : " ,resultado)
        elif operacao == "*":
# "*" representa a conta Multiplicação.
            print(" Multiplicação é uma operação que consiste em uma adição sucessivas de um mesmo número produzindo um resultado que chamamos de produto.\n ")
            primeiro = input("Digite o primeiro número:\n ")
            segundo = input("Digite o segundo número:\n ")
            resultado = float(primeiro) * float(segundo)
            print(" O resultado é : " ,resultado)
        elif operacao == "/":
# "/" representa a conta Divisão.
            print("que é uma operação que realiza a divisão de números naturais e é o mesmo que repartir em partes iguais os números.\n  Na operação de divisão, o dividendo é como se chama o número a ser dividido, enquanto que o divisor é o número que divide o cálculo e quociente é o resultado da operação.\n ")
            primeiro = input("Digite o primeiro número:\n ")
            segundo = input("Digite o segundo número:\n ")
            resultado = float(primeiro) / float(segundo)
            print(" O resultado é : " ,resultado)
        elif operacao == "raiz":
# "raiz" representa a conta Raiz quadrada.
            print(" Raiz quadrada é uma operação onde a raiz quadrada de um número x é um número único e não negativo que, quando multiplicado por si próprio, se iguala a x.\n")
            num = float(input("Digite o número:\n "))
            resultado = math.sqrt(num)
            print(" O resultado é : " ,resultado)
        elif operacao == "**":
# "**" representa a conta Potência.
            print(" Potência é uma operação onde é uma notação simplificada de representar a multiplicação de um número que chamamos de base, repetidamente pelo valor de uma potência que nos determina quantas vezes devemos multiplicar este número.\n")
            num = float(input("Digite o número:\n " ))
            pot=float(input("Digite o valor da potência:\n "))
            resultado = num**pot
            print(" O resultado é : " ,resultado)
        else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.
            print("\t IMPOSSÍVEL REALIZAR A OPERAÇÃO!!!\n ")
    
        
# COVERSOR
    if inicio == '2':
#Caso o usuário escolha '2', irá ser redirecionado para a parte de conversão de medidas.
        print("\t CONVERSOR DE UNIDADES: \n")
        print("Para prosseguir escolha uma das seguintes opções: ")
        while True:
            unidade = input("Comprimento digite 1\n"
                       "Temperatura digite 2\n"
                       "Volume digite 3\n"
                       "Massa digite 4\n"
                       "Dados digite 5\n"
                       "Para sair do programa digite 'sair' \n")
            if unidade == 'sair':
#Sendo digitado pelo usuário 'sair', será automaticamente fechado o programa.    
                print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                exit()
            elif unidade == '1':
#Sendo escolhido a opção '1', o usuário é redirecionado a conversão de comprimento, e para que seja feita a conversão desejada, é fornecida uma listagem para que seja feita corretamente.
#Basta o usuário digitar o número correspondente de cada unidade.
                print("COMPRIMENTO: \n")
                print("Para prosseguir, escolha uma das opções abaixo: ")
                while True:
                    comp = input("M ----> Cm digite 1\n"
                              "M ----> Mm digite 2\n"
                              "Cm ----> M digite 3\n"
                              "Cm ----> mm digite 4\n"
                              "Mm ----> M digite 5\n"
                              "Mm ----> Cm digite 6\n"
                              "Para sair do programa digite 'sair' \n")
                    if comp == 'sair':
#Sendo digitado pelo usuário 'sair', será automaticamente fechado o programa. 
                        print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                        exit()
                    if comp == '1':
                        print("M ----> CM\n")
                        v1 = input("Digite o comprimento em Metros: ")
                        resp = float(v1) * (100)
                        print(" O COMPRIMENTO EM É: ",resp," CM")                      
                    elif comp=='2':
                        print("M ----> MM\n")
                        v1 = input("Digite o comprimento em Metros: ")
                        resp = float(v1) * 10000
                        print(" O COMPRIMENTO É:",resp, " MM")
                    elif comp == '3':
                        print("CM ----> M\n")
                        v1 = input("Digite o comprimento em Centímetros: ")
                        resp = float(v1) / 100
                        print(" O COMPRIMENTO É:",resp, " M")
                    elif comp == '4':
                        print("CM ----> MM\n")
                        v1 = input("Digite o comprimento em Centímetros: ")
                        resp = float(v1) * 100
                        print(" O COMPRIMENTO É:",resp, "MM")
                    elif comp == '5':
                        print("MM ----> M\n")
                        v1 = input("Digite o comprimento em Milímetros: ")                        
                        resp = float(v1) / 10000
                        print(" O COMPRIMENTO É:",resp, "M")
                    elif comp == '6':
                        print("MM ----> CM\n")                        
                        v1 = input("Digite o comprimento em Milímetros: ")
                        resp = float(v1) / 100
                        print(" O COMPRIMENTO É:",resp, "CM")
                    else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.
                        print ("\t CARACTER INVÁLIDO!!!\n")
            elif unidade == '2':
#Sendo escolhido a opção '2',o usuário é redirecionado a lista de Temperatura.
#Antes de ser feito diretamente a conta, é perguntado ao usuário se ele deseja uma explicação a respeito das escalas termomêtricas.
#Caso o usuário opte por uma explicação, será pedido que seja indicado a numeração de acordo com o tema de sua opção.
#Após ser perguntado, irá ser perguntado ao usuário, qual conversão deseja ser feita e para isso, basta digitar o número correspondente a cada uma.
                print("CONVERSOR DE TEMPERATURA: \n")
                inicio = input(" Caso deseje uma explicação a respeito das temperaturas:\n Para Celsius, digite '1'\n Para Fahrenheit, digite '2'\n Para Kelvin, digite '3'\n")
                if inicio == '1':
                    print(" Celsius: É conhecida como a escala centígrada, é uma escala termométrica do sistema métrico usada na maioria dos países do mundo.\n Teve origem a partir do modelo proposto pelo astrônomo sueco Anders Celsius.\n Esta escala é baseada nos pontos de fusão e de ebulição da água, em condição atmosférica padrão, aos quais são atribuídos os valores de 0 °C e 100 °C, respectivamente.\n Enquanto que os valores de congelamento e evaporação da água estão aproximadamente corretos, a definição original não é apropriada como um padrão formal pois ela depende da definição de pressão atmosférica padrão, que por sua vez depende da própria definição de temperatura.\n A definição oficial atual de grau Celsius define 0,01 °C como o ponto triplo da água, e 1 grau Celsius como sendo 1/273,16 da diferença de temperatura entre o ponto triplo da água e o zero absoluto.\n Esta definição garante que 1 grau Celsius apresente a mesma variação de temperatura que 1 kelvin.\n")
                elif inicio == '2':
                    print(" Fahrenheit é uma escala de temperatura proposta por Daniel Gabriel Fahrenheit em 1724.\n Sua unidade é o grau Fahrenheit (símbolo: °F).\n Nesta escala o ponto de fusão da água é de 32 °F e o ponto de ebulição é de 212 °F.\n Uma diferença de 1,8 °F é igual a uma diferença de 1 °C.\n  Muito utilizada pelo o povo grego, para medir a temperatura de um corpo.\n É utilizado para medir a temperatura chamada de Rankine, que leva o marco zero de sua escala ao zero absoluto e possui a mesma variação da escala fahrenheit, existindo, portanto, correlação entre a escala de Rankine e grau fahrenheit do mesmo modo que existe correlação das escalas kelvin e grau Celsius.\n ")
                elif inicio == '3':
                    print("O kelvin (símbolo: K) é a unidade de base do Sistema Internacional de Unidades (SI) para a grandeza temperatura termodinâmica.\n O kelvin é a fração 1/273,16 da temperatura termodinâmica do ponto triplo da água, ou seja, é definido de tal modo que o ponto triplo da água é exatamente 273,16 K.\n   É utilizado para medir a temperatura absoluta de um objeto, com zero absoluto sendo 0 K. A escala kelvin recebeu este nome em homenagem ao físico e engenheiro irlandês William Thomson (1824–1907), 1º barão Kelvin, que escreveu sobre a necessidade de uma 'escala termométrica absoluta'\n Diferentemente do grau Fahrenheit e do grau Celsius, o kelvin não é referido nem escrito como um grau.\n  O kelvin é a unidade primária de medida de temperatura nas ciências físicas, mas é frequentemente usado em conjunção com o grau Celsius, que tem a mesma magnitude.\n")
                print("Para prosseguir, escolha uma das opções: ")
                while True:
                    temp = input("º Celsius ----> ºFahrenheit: \n'1'\n"
                              "º Celsius ----> Kelvin: \n'2'\n"
                              "º Fahrenheit ----> º Celsius: \n'3'\n"
                              "º Fahrenheit ----> Kelvin: \n'4'\n"
                              "Kelvin ----> º Celsius: \n'5'\n"
                              "Kelvin ----> º Fahrenheit: \n'6'\n"
                              "Para sair do programa digite 'sair' \n")
                    if temp == 'sair':
#Sendo digitado pelo usuário 'sair', será automaticamente fechado o programa. 
                        print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                        exit()
                    if temp == '1':
                        print("\t ºCELSIUS ----> ºFAHRENHEIT: \n")
                        a = input("Digite a temperatura em graus celsius: ")
                        resp1 = float(a) * 9 
                        resp = ( float(resp1) + 160) / 5
                        print(" A TEMPERATURA EM ºF É:",resp)
                    elif temp == '2':
                        print("\t CELSIUS ----> KELVIN: \n")
                        a = input("Digite a temperatura em graus celsius: ")
                        resp = float(a) + 273
                        print(" A TEMPERATURA EM K É:",resp)
                    elif temp == '3':
                        print("\t FAHRENHEIT ----> CELSIUS: \n")
                        a = input("Digite a temperatura em graus fahrenheit: ")
                        resp1 = float(a) * 5
                        resp = (float(resp1) - 160) / 9
                        print(" A TEMPERATURA EM ºC É:",resp)
                    elif temp == '4':
                        print("\t FAHRENHEIT ----> KELVIN: \n")
                        a = input("Digite a temperatura em fahrenheit: ")
                        resp1 = float(a) + 459.67
                        resp = float(resp1) / 1.8
                        print(" A TEMPERATURA EM K É:",resp)
                    elif temp == '5':
                        print("\t KELVIN ----> CELSIUS: \n")
                        a = input("Digite a temperatura em kelvin: ")
                        resp = float(a) - 273
                        print(" A TEMPERETURA EM ºC É:",resp)
                    elif temp == '6':
                        print("\t KELVIN ----> FAHRENHEIT: \n")
                        a = input("Digite a temperatura em kelvin: ")
                        resp1 = float(a) * 1.8
                        resp = float(resp1) - 459.67
                        print(" A TEMPERATURA EM ºF É:",resp)
                    else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.
                        print ("\t CARACTER INVÁLIDO!!!\n")
            elif unidade == '3':
#Sendo escolhido a opção '3', o usuário é redirecionado para a lista de Volume.
#Para realizar a conversão, basta o usuário digitar o número que corresponde a cada conversão.
                print("\t CONVERSOR DE VOLUME: \n")
                print("Para prosseguir, escolha uma das opções: ")
                while True:
                    vol = input("Litro ----> Mililitro: \n'1'\n"
                              "Litro ----> Metro cúbico: \n'2'\n"
                              "Litro ----> Centímetro cúbico: \n'3'\n"
                              "Mililitro ----> Litro: \n'4'\n"
                              "Para sair do programa digite 'sair' \n")
                    if vol == 'sair':
#Sendo digitado pelo usuário 'sair', será automaticamente fechado o programa. 
                        print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                        exit()
                    elif vol == '1':
                        print("\t LITRO ----> MILILITRO: \n")
                        a = input("Digite o volume em litros:")
                        resp = float(a) * 1000
                        print(" O VOLUME EM ML É:",resp)
                    elif vol == '2':
                        print("\t LITRO ----> METRO CÚBICO:\n")
                        a = input("Digite o volume em litros: ")
                        resp = float(a) / 1000
                        print(" O VOLUME EM M³ É:",resp)
                    elif vol == '3':
                        print("\t LITRO ----> CENTÍMETRO CÚBICO: \n")
                        a = input("Digite o volume em litros: ")
                        resp = float(a) * 1000
                        print(" O VOLUME EM CM³ É:",resp)
                    elif vol == '4':
                        print("\t MILILITRO ----> LITRO: \n")
                        a = input("Digite o volume em mililitros: ")
                        resp = float(a) / 1000
                        print(" O VOLUME EM L É:",resp)
                    else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.
                        print ("\t CARACTER INVÁLIDO!!!\n")
                        
            elif unidade == '4':
#Sendo escolhido a opção '4', o usuário é redirecionado a lista de Massa.
#Para ser realizada a conversão, o usuário deve selecionar a numeração correspondente a conversão desejada.
                print("\t MASSA: \n")
                print("Para prosseguir, escolha umas das opções: ")
                while True:
                    massa = input("TONELADAS ----> KG: \n'1'\n"
                              "TONELADAS ----> G: \n'2'\n"
                              "TONELADAS ----> MG: \n'3'\n"
                              "QUILOGRAMAS ----> T: \n'4'\n"
                              "QUILOGRAMAS ----> G: \n'5'\n"
                              "QUILOGRAMAS ----> MG: \n'6'\n"
                              "GRAMAS ----> T: \n'7'\n"
                              "GRAMAS ----> KG: \n'8'\n"
                              "GRAMAS ----> MG: \n'9'\n"
                              "Para sair do programa digite 'sair' \n")
                    if massa == 'sair':
#Sendo digitado pelo usuário 'sair', será automaticamente fechado o programa. 
                        print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                        exit()
                    if massa == '1':
                        print("\t TONELADA ----> KG:\n")
                        c = input("Digite o valor em tonelada: ")
                        resp = float(c) * 1000
                        print(" A MASSA EM KG É:",resp)    
                    elif massa == '2':
                        print("\t TONELADA ----> G: \n")
                        c = input("Digite o valor em tonelada: ")
                        resp = float(c) * 1000000
                        print(" A MASSA EM G É:",resp)
                    elif massa == '3':
                        print("\t TONELADA ----> MG: \n")
                        c = input("Digite o valor em tonelada: ")
                        resp = float(c) * 1000000000
                        print(" A MASSA EM MG É:",resp)
                    elif massa == '4':
                        print("\t QUILOGRAMAS ----> T: \n")
                        c = input("Digite o valor em quilograma: ")
                        resp = float(c) / 1000
                        print(" A MASSA EM T É:",resp)
                    elif massa == '5':
                        print("\t QUILOGRAMAS ----> G: \n")
                        c = input("Digite o valor em quilograma: ")
                        resp = float(c) * 1000
                        print(" A MASSA EM G É:",resp)
                    elif massa == '6':
                        print("\t QUILOGRAMAS ----> MG: \n")
                        c= input("Digite o valor em quilograma: ")
                        resp = float(c) * 1000000
                        print(" A MASSA EM MG É:",resp)
                    elif massa == '7':
                        print("\t GRAMAS ----> T: \n")
                        c= input("Digite o valor em grama: ")
                        resp = float(c) / 1000000
                        print(" A MASSA EM T É:",resp)
                    elif massa == '8':
                        print("\t GRAMAS ----> KG: \n")
                        c = input("Digite o valor em grama: ")
                        resp = float(c) / 1000
                        print(" A MASSA EM KG É:",resp)                        
                    elif massa == '9':
                        print("\t GRAMAS ----> MG: \n")
                        c = input("Digite o valor em grama: ")
                        resp = float(c) * 1000
                        print(" A MASSA EM MG É:",resp)
                    else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.
                        print ("\t CARACTER INVÁLIDO!!!\n")
                        
            elif unidade == '5':
#Sendo escolhido a opção '5', o usuário é redirecionado a lista de Dados.
#Para ser executada a função, o usuário deverá digitar o número correspondente a conversão que deseja. 
                print("\t DADOS: \n")
                print("Para prosseguir, esoclha uma das seguintes opções: ")
                while True:
                    dado = input("BIT ----> BYTE: \n'1'\n"
                              "BYTE ----> MEGABYTE: \n'2'\n"
                              "BYTE ----> GIGABYTE: \n'3'\n"
                              "MEGABYTE ----> BITE: \n'4'\n"
                              "MEGABYTE ----> GIGABYTE: \n'5'\n"
                              "MEGABYTE ----> TERABYTE: \n'6'\n"
                              "GIGABYTE ----> BYTE: \n'7'\n"
                              "GIGABYTE ----> MEGABYTE: \n'8'\n"
                              "GIGABYTE ----> TERABYTE: \n'9'\n"
                              "TERABYTE ----> MEGABYTE: \n'10'\n"
                              "TERABYTE ----> GIGABYTE: \n'11'\n"
                              "Para sair do programa digite 'sair' \n")
                    if dado == 'sair':
#Sendo digitado pelo usuário 'sair', será automaticamente fechado o programa. 
                        print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                        exit()
                    elif dado == '1':
                        print("\t BIT ----> BYTE: \n")
                        a = input("DIGITE O VALOR EM BIT: \n")
                        resp = float(a) * 0.125 
                        print(" OS DADOS EM BYTES SÃO:",resp)
                    elif dado == '2':
                        print("\t BYTE ----> MEGABYTE: \n")
                        a = input("DIGITE O VALOR EM BYTE: \n")
                        resp = float(a) * 1000000
                        print(" OS DADOS EM MEGABYTE SÃO:",resp)
                    elif dado == '3':
                        print("\t BYTE ----> GIGABYTE: \n")
                        a = input("DIGITE O VALOR EM BYTE: \n")
                        resp = float(a) * 125000000
                        print(" OS DADOS EM GIGABYTES SÃO:",resp)
                    elif dado == '4':
                        print('\t MEGABYTE ----> BYTE: \n')
                        a = input("DIGITE O VALOR E MEGABYTE: ")
                        resp = float(a) / 100000
                        print(" OS DADOS EM BYTES SÃO: ",resp)
                    elif dado == '5':
                        print("\t MEGABYTE ----> GIGABYTE: \n")
                        a = input("DIGITE O VALOR EM MEGABYTE: ")
                        resp = float(a) / 0.008
                        print(" OS DADOS EM GIGABYTES SÃO:",resp)
                    elif dado == '6':
                        print("\t MEGABYTE ----> TERABYTE: \n")
                        a = input("DIGITE O VALOR EM MEGABYTE: ")
                        resp = float(a) / 0.000000125
                        print(" OS DADOS EM TERABYTE SÃO:",resp)
                    elif dado == '7':
                        print("\t GIGABYTE ----> BYTE: \n")
                        a = input("DIGITE O VALOR EM GIGABYTE: ")
                        resp = float(a) * 125000000
                        print(" OS DADOS EM BYTES SÃO:",resp)
                    elif dado == '8':
                        print("\t GIGABYTE ----> MEGABYTE: \n")
                        a = input("DIGITE O VALOR A SER CONVERTIDO: ")
                        resp = float(a) * 1000
                        print(" OS DADOS EM MEGABYTES SÃO:",resp)
                    elif dado == '9':
                        print("\t GIGABYTE ----> TERABYTE: \n")
                        a = input('DIGITE O VALOR EM GIGABYTE: \n')
                        resp = float(a) / 0.000125
                        print(" OS DADOS EM TERABYTES SÃO:",resp)
                    elif dado == '10':
                        print("\t TERABYTE ----> MEGABYTE: \n")
                        a = input("DIGITE O VALOR EM TERABYTE: ")
                        resp = float(a) * 1000000
                        print(" OS DADOS EM MEGABYTES SÃO:",resp)
                    elif dado == '11':
                        print('\t TERABYTE ----> GIGABYTE: \n')
                        a = input('DIGITE O VALOR EM TERABYTE: ')
                        resp = float(a) * 1000
                        print(" OS DADOS EM GIGABYTES SÃO:",resp)
                    else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.
                        print("\t CARACTER INVÁLIDO!!!\n")

# GEOMETRIA
#Caso o usuário escolha '3', irá ser redirecionado a parte de Geometria.
    if inicio == '3':
        print("\t GEOMETRIA \n")
        print("Para prosseguir, escolha uma das opções abaixo: ")
        while True:
            geometria = input("Área digite 1\n"
                              "Volume digite 2\n"
                              "Teorema de Pitágoras digite 3\n"
                              "Para sair do programa digite 'sair' \n")
            if geometria == 'sair':
#Sendo digitado pelo usuário 'sair', será automaticamente fechado o programa. 
                print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                exit()
            if geometria == '3':
#Sendo escolhido o número '3', o usuário é redirecionado para o Teorema de Pitágoras.
#Antes de ser feito diretamente a conta, é perguntado ao usuário se ele deseja uma explicação.
#Logo em seguida, é pedido para que seja inserido os valores para que possa ser feita as contas através da fôrmula especificada.
                print("\t TEOREMA DE PITÁGORAS: \n")
                inicio = input(" Antes de realizar a conta, deseja uma explicação passo a passo?\n Se sim, digite '1'\n Se não,digite '2'\n")
                if inicio == '1':
                    print("Em um triângulo retângulo, o quadrado da hipotenusa é igual à soma dos quadrados dos catetos.\nO maior lado do triângulo fica sempre oposto ao maior ângulo, que é o ângulo de 90°.\n Esse lado recebe o nome de hipotenusa e será representado aqui pela letra a.\n Os demais lados do triângulo são chamados de catetos e serão aqui representados pelas letras b e c.\n O teorema de Pitágoras afirma que é válida a relação a seguir: sqrt(c) = a**2 + b**2.\n Assim, podemos dizer que o quadrado da medida da hipotenusa é igual à soma dos quadrados das medidas dos catetos.\n")
                a = input("DIGITE O VALOR DO CATETO 1: ")
                b = input("DIGITE O VALOR DO CATETO 2: ")
                resp = math.sqrt(float(a)* float(a)+ float(b)*float(b))
                print(" O VALOR DA HIPOTENUSA É:",resp)
            elif geometria == '1':
#Sendo escolhido o número '1', o usuário é redirecionado para Área. 
#Antes de ser feito diretamente a conta, é perguntado ao usuário se ele deseja uma explicação.
#Caso o usuário opte por uma explicação, será pedido que seja indicado a numeração de acordo com o tema de sua opção.
#Logo em seguida, é pedido para que seja inserido os valores para que possa ser feita as contas através da fôrmula especificada.
                print("\t ÁREA \n")
                print ("Equivale a medida da superfície de uma figura geométrica.")
                print("Para prosseguir, escolha uma das opções abaixo: ")
                while True:
                    area = input("Área do Quadrado digite 1\n"
                              "Área do Retângulo digite 2\n"
                              "Área do Triângulo digite 3\n"
                              "Área do Circulo digite 4\n"
                              "Área do Trapézio digite 5\n"
                              "Para sair do programa digite 'sair' \n")
                    if area == 'sair':
                        print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                        exit()
                    elif area == '1':
                        print("\t ÁREA DO QUADRADO: \n")
                        inicio = input (" Antes de realizar a conta, deseja uma explicação?\n Se sim, digite '1'\n Se não,digite '2' \n")
                        if inicio == '1':
                            print(" O quadrado é uma figura plana que possui quatro lados iguais, ou seja, quatro lados que possuem a mesma medida.\n Ele também conta com quatro ângulos internos retos (ângulos de 90°).\n O cálculo de área, é feito pela fórmula A = l², sendo l a medida do lado.\n")
                        l = input("Digite um dos lados do quadrado: ")
                        resp = float(l) * float(l)
                        print(" A ÁREA DO QUADRADO É:",resp)
                    elif area == '2':
                        print("\t ÁREA DO RETÂNGULO: ")
                        inicio = input(" Antes de realizar a conta, deseja uma explicação?\n  Se sim, digite '1' \n Se não, digite '2' \n")
                        if inicio == '1':
                            print(" A área do retângulo corresponde ao produto da medida da base pela altura da figura, sendo expressa pela fórmula:A=b.h\n Lembre-se que o retângulo é uma figura geométrica plana formada por quatro lados(quadrilátero).\n Dois lados do retângulo são menores e dois deles são maiores.\n Ele possui quatro ângulos internos de 90° chamados de ângulos retos.\n Assim, a soma dos ângulos internos dos retângulos totalizam 360°.\n")
                        b = input("Digite o lado a do retângulo: ")
                        h = input("Digite a altura b do retângulo: ")
                        resp = float(b) * float(h)
                        print(" A ÁREA DO RETÂNGULO É:",resp)
                    elif area == '3':
                        print("\t ÁREA DO TRIÂNGULO: \n")
                        inicio = input(" Antes de realizar a conta, deseja uma explicação?\n Se sim, digite '1'\n Se não, digite '2'\n")
                        if inicio == '1':
                            print(" A área do triângulo pode ser calculada através das medidas da base e da altura da figura. Lembre-se que o triângulo é uma figura geométrica plana formada por três lados.\n Na maioria das situações, usamos as medidas da base e da altura de um triângulo para calcular a sua área.\n")
                        b = input("Digite o valor da base do triângulo: ")
                        h = input("Digite o valor da altura do triângulo: ")
                        resp = (float(b) * float(h)) / 2
                        print(" A ÁREA DO TRIÂNGULO É:",resp)
                    elif area == '4':
                        print("\t AREA DO CIRCULO: \n")
                        inicio = input(" Antes de realizar a conta, deseja uma explicação?\n  Se sim, digite '1' \n  Se não, digite '2' \n")
                        if inicio == '1':
                            print(" A área do círculo corresponde ao valor da superfície dessa figura, levando em conta a medida de seu raio (r).\n Vale lembrar que o círculo, também chamado de disco, é uma figura geométrica que faz parte dos estudos da geometria plana.\n Essa figura surge na medida em que os polígonos regulares inscritos nela vão aumentando o número dos lados.\n Ou seja, com o aumento do número de lados dos polígonos estes vão se aproximando da forma circular.\n")
                        pi = 3.14
                        r = input("DIGITE O VALOR DO RAIO: ")
                        resp = (float(r) * float(r)) * pi
                        print("\t A ÁREA DO CÍRCULO É:",resp,"\n")
                    elif area == '5':
                        print("\t ÁREA DO TRAPÉZIO: \n")
                        inicio = input(" Antes de realizar a conta, deseja uma explicação?\n Se sim, digite '1'\n Se não, digite '2'\n")
                        if inicio == '1':
                            print(" A área do trapézio mede o valor da superfície dessa figura plana formada por quatro lados.\n O trapézio é um quadrilátero que possui dois lados e duas bases paralelas, sendo que uma é maior e outra menor.\n O trapézio é considerado um quadrilátero notável, de forma que a soma de seus ângulos internos corresponde a 360°.\n")
                        b = input("Digite o valor da base menor: ")
                        B = input("Digite o valor da base maior: ")
                        h = input("Digite o valor da altura: ")
                        resp = ((float(b) + float(B))/2) * float(h)
                        print("\t A ÁREA DO TRAPÉZIO É:",resp,"\n")
                    else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.            
                        print("\t CARACTER INVÁLIDO!!!\n")
            elif geometria == '2':
                print("\t VOLUME \n")
                print("O volume de um sólido geométrico é a medida da região do espaço limitada por sua superfície.")
                print("Para prosseguir, escolha uma das opções abaixo: ")
                while True:
                    volume = input("Volume do Cubo digite 1\n"
                          "Volume do Paralelepípedo digite 2\n"
                          "Volume da Pirâmide digite 3\n"
                          "Volume da Esfera digite 4\n"
                          "Volume do Cilíndro digite 5\n"
                          "Para sair do programa digite 'sair' \n")
                    if volume == 'sair':
                        print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                        exit()
                    if volume == '1':
                        print("\t VOLUME DO CUBO: \n")
                        inicio = input(" Antes de realizar a conta, deseja uma explicação?\n Se sim, digite '1'\n Se não, digite '2'\n")
                        if inicio == '1':
                            print(" Cubo é um prisma regular limitado por 6 quadrados congruentes.\n  No caso do cubo, a base (como todas as faces) é um quadrado de lado L, logo, tem área igual a L².\n A altura será também L. Portanto, o volume do cubo é L³.\n")
                        L = input("Digite o valor dos lados do cubo: ")
                        resp = float(L) **3
                        print(" O VOLUME DO CUBO É:",resp)
                    elif volume == '2':
                        print("\t VOLUME DO PARALELEPÍPEDO: ")
                        inicio = (" Antes de realizar a conta, deseja uma explicação?\n  Se sim, digite '1'\n  Se não, digite '2'\n")
                        if inicio == '1':
                            print(" O paralelepípedo é um prisma cuja base é um paralelogramo.\n No caso de um paralelepípedo reto, o mais importante, temos que o paralelogramo da base é um retângulo.\n A base é um retângulo de lados a e b, logo, tem área igual a ab e a altura mede c.\n Portanto, o volume do paralelepípedo é abc.\n")
                        a = input("Digite o lado a do paralelepipedo: ")
                        b = input("Digite o comprimento do paralelepipedo: ")
                        c = input("Digite o altura do paralelepipedo: ")
                        resp = float(a) * float(b) * float(c)
                        print(" O VOLUME DO PARALELEPÍPEDO É:",resp)
                    elif volume == '3':
                        print("\t VOLUME DA PIRÂMIDE: \n")
                        inicio = input(" Antes de realizar a conta, deseja uma explicação?\n Se sim, digite '1'\n Se não, digite '2'\n")
                        if inicio == '1':
                            print(" Pirâmide é a reunião de todos os segmentos com uma extremidade em V e a outra num ponto qualquer do polígono.\n O ponto V é chamado de vértice da pirâmide.\n O volume da pirâmide é um terço do volume de um prisma com mesma base e altura.\n")
                        a = input("Digite o valor da largura da base da pirâmide: ")
                        b = input("Digite o valor da altura da base da pirâmide: ")
                        h = input("Digite o valor da altura da pirâmede: ")
                        resp = (float(a) * float(b)* float(h))/3
                        print(" O VOLUME DA PIRÂMEDE É:",resp)
                    elif volume == '4':
                        print("\t VOLUME DA ESFERA: \n")
                        inicio = input(" Antes de realizar a conta, deseja uma explicação?\n Se sim, digite '1'\n Se não, diite '2'\n")
                        if inicio == '1':
                            print(" O volume de uma esfera de raio r é dois terços do volume de um cilindro de raio da base r e altura h = 2r (cilindro equilátero).\n Volume de um cilindro equilátero (raio h e altura h = 2r.\n Como o volume do cilíndro é dado por:\n V = pi * r ** 2 * h =\n V = pi * r ** 2 * 2 * r =\n V = 2 * pi * r ** 3\n De acordo com a constatação acima:\n O volume da esfera = 2/3\n O volume do cilindro equilátero = 2 * pi * r ** 3\n Multiplicando a fórmula do volume da esfera com o volume do cilíndro equilátero forma a fórmula do volume da esfera.")
                        pi = 3.14
                        r = input("DIGITE O VALOR DO RAIO: ")
                        resp = ((float(r) ** 3) * pi)*(4/3)
                        print("O VOLUME DA ESFERA É:",resp,"\n")
                    elif volume == '5':
                        print("\t VOLUME DO CILÍNDRO: \n")
                        inicio = input(" Antes de realizar a conta, deseja uma explicação?\n Se sim, digite '1'\n Se não, digite '2'\n")
                        if inicio == '1':
                            print(" O cilíndro é dado pela multiplicação da área da base (Ab)= pi * r ** 2 vezes a altura (h)\n De acordo com o Princípio de Cavalieri:\n As definições de cilindro e prisma têm algo em comum:\n Ambas retratam sólidos geométricos com bases paralelas e congruentes.\n Sabendo disso, suponha que exista um cilíndro e um paralelepípedo (prisma) com mesma altura (h).\n Sendo A1 e A2 as áreas das bases do cilindro e do paralelepípedo, respectivamente.\n Suponha também que A1 = A2,ou seja, que a área das bases também sejam iguais (assim como a altura h).\n Tal princípio nos traz que o prisma e o cilindro podem ser pensados como união de h camadas (polígonos e círculos, respectivamente) de áreas iguais.\n Tudo isso porque juntando esses polígonos ou círculos (figuras 2D), um em cima do outro de determinado modo, formamos um sólido (figura 3D).\n Os polígonos formarão os prismas e os círculos formarão os cilindros.\n Então, que deduzimos que o volume do prisma e do cilindro podem ser obtidos pela área da base (camada) vezes altura (o número de camadas).\n")
                        pi = 3.14
                        r = input("Digite o valor do raio: ")
                        h = input("Digite o valor da altura: ")
                        resp = (pi * float(r) ** 2) * float(h)
                        print("\t O VOLUME DO CILÍNDRO É:",resp,"\n")
                    else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.        
                        ("CARACTER INVÁLIDO!!!\n")
                            
# ALGEBRA
    if inicio == '4':
        print("\t ÁLGEBRA \n")
        print("Para prosseguir, escolha uma das opções abaixo: ")
        while True:
            equacao = input("Equação do 2º grau digite 1\n"
                           "Para sair do programa digite 'sair' \n")
            if equacao == 'sair':
#Sendo digitado pelo usuário 'sair', será automaticamente fechado o programa. 
                print("\t OBRIGADO POR USAR MATH SOLUTION!!!\n")
                exit()
            if equacao == '1':
#Antes de ser feito diretamente a conta, é perguntado ao usuário se ele deseja uma explicação.
#Caso o usuário opte por uma explicação, será pedido que seja indicado a numeração de acordo com o tema de sua opção.
#Logo em seguida, é pedido para que seja inserido os valores para que possa ser feita as contas através da fôrmula especificada.
                print("\t EQUAÇÃO DO 2º GRAU: \n")
                lista = []
                inicio = input(" Antes de realizar a conta, deseja uma explicação?\n Se sim, digite '1'\n Se não, digite '2'\n")
                if inicio == '1':
                    print(" Há duas incógnitas x nessa equação, e uma delas possui expoente 2.\n Essa equação é classificada como do 2º grau.\n A forma de resolução de uma equação do 2º grau  é por meio do método de 'Bhaskara.\n Para determinar a solução de uma equação é o mesmo que descobrir suas raízes, isto é, o valor ou os valores que satisfazem a equação.\n")
                a = int(input("Digite um valor para a: "))
                b = int(input("Digite um valor para b: "))
                c = int(input("Digite um valor para c: "))
                delta = b*b - 4 * a * c
                if delta < 0:
                     print("\t ESTA OPERAÇÃO NÃO POSSUÍ RAÍZES REAIS\n ")
                elif delta == 0:
                    raiz = (-1 * b + math.sqrt(delta)) / (2 * a)
                    lista.append(raiz)
                    print("\t A EQUAÇÃO POSSUÍ APENAS UMA RAIZ REAL",lista)
                elif delta > 0:
                    raiz1 = (-1 * b + math.sqrt(delta)) / (2 * a)
                    raiz2 = (-1 * b - math.sqrt(delta)) / (2 *a)
                    raiz3 = raiz1, raiz2
                    lista.append(raiz3)
                    print("\t AS RAÍZES DA EQUAÇÃO SÃO:",lista)  
            else:
#Caso seja inserido qualquer outro caracter, aparecerá impresso na tela uma frase dizendo que não é possível realizar este tipo de operação.
                print ("\t CARACTER INVÁLIDO!!!\n")
       
