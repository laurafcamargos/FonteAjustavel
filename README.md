# Trabalho 1 - Fonte de Tensão Ajustável
Projeto realizado para a disciplina '[SSC0180] – Eletrônica para Computação', ministrada pelo professor Eduardo do Valle Simões. Neste projeto, busca-se projetar uma fonte de tensão ajustável entre 3v e 12v, com uma corrente de 100mA. 


# Integrantes - Grupo 17

| **Nome**              | **N°USP**|
|--------------------------------|----------|
| Bruna Izabel da Silva Pereira| 15635441 | 
| Camilli Gabrielli Ramos Muniz| 15635722 |
| [Laura Fernandes Camargos](https://github.com/laurafcamargos)| 13692334 |
| [Sandy da Costa Dutra](https://github.com/sandycdutra)| 12544570 |



# Objetivo
Projetar e montar uma fonte de tensão ajustável (corrente contínua) entre 3v e 12v, com capacidade de 100mA. Ela deve ser capaz de receber uma corrente alternada de tensão eficaz de 127v e fornecer uma corrente contínua.

# Diagrama da Fonte
![Diagrama da fonte no software Falstad](img/circuit-20240626-0729.png "Diagrama da fonte no software Falstad")

[Link para o circuito no Falstad](https://tinyurl.com/2ehnnvpj)


# Escolha de Componentes

| Quantidade  | Componente  | Especificações   | Valor  |
|---|---|---|---|
| 1 | Protoboard | BB-01 400P |R$21,70|
| 10 | Diodo Retificador | Ponte de Diodo 1N4007 |R$2,00| 
| 1 | Capacitor | 470µF, 35V |R$2,80|
| 1 | LED | Vermelho 5mm |R$0,50|
| 1 | Diodo Zener |1N4743 13V, 1W |R$0,50|
| 1 | Potenciômetro | 1W B5K B-16 |R$7,00|
| 10 | Resistor CR25 100 | 100Ω |R$0,70|
| 10 | Resistor CR25 820 | 820Ω |R$0,70|
| 10 | Resistor CR25 1k | 1000Ω |R$0,70|
| 10 | Resistor CR25 1.8k | 1800Ω |R$0,70|
| 1 | Transistor 2N3904 | 60V, 0,2A 0,650W |R$1,60|
| Total | | |R$38,90|

#### Transformador
> * O transformador é o componente responsável por abaixar a tensão da tomada (110 V) para uma tensão mais próxima da que será trabalhada (3-12V). O transformador, emprestado pelo professor Simões, leva 110V para 24.2V.

>  ![](img/transformador.gif)
#### Ponte de Diodos
> * Os diodos são usados para formar a ponte retificadora. Essa ponte é responsável por proporcionar o maior aproveitamento da energia, abastecendo o circito com a corrente em ambos os ciclos da corrente alternada. Sua função é garantir que a corrente apenas flua em um sentido. Ela segue sendo alternada, porém não "desce" abaixo do "zero".
> * No gráfico, ela funciona como se fosse um módulo. Ou seja, quando aplicada em uma corrente alternada (senoide), ela "joga" os pontos "negativos" para o 'positivo'.

>  ![](img/ponte.gif)

#### Capacitor
> * O capacitor serve para armazenar temporariamente uma certa carga durante um período crescente da tensão e descarrega no período subsequente. Além disso, é responsável por carregar o sistema quando a tensão (vinda da ponde de diodos) está em declínio, estabilizando a tensão que vai para o restante do circuito e criando o "ripple". O capacitor escolhido é um de 470uF, para criar um ripple de até 10%, como foi exigido pelo professor na especificação do trabalho.

>  ![](img/capac.gif)

#### Zener
> * Serve para "filtrar" o excesso de corrente. Escolhe-se um valor abaixo da tensão mínima para assim eliminar ou mitigar o ripple - isto é, tornar a corrente de fato contínua. 
> * O Zener é usado como limitador de tensão no circuito. O diodo escolhido tem tensão de regulação de 13V, ou seja, ele limita a tensão na saida dele em 13V constantes. Ele será usado para causar uma tensão de referência para o transistor.

#### Led
> * Apenas serve para indicar a passagem de corrente para o usuário. Se trata de um componente facultativo.

#### Potenciômetro 
> * Serve para regular a voltagem que passará pelo transistor. Dessa forma, é possível ajustar a tensão de acordo com o dispositivo conectado (entre 3v e 12v).
> * O potenciômetro recebe a corrente em paralelo com o diodo Zener, e portanto tem potencial fixo em aprimadamente 13V (ocorre uma pequena queda do potencial devido as conexões do componente no resto do circuito). Assim, ele controla a tensão mínima (~3V) e máxima (~12V) que vai para o transistor de controle.

#### Resistores
> * Servem para limitar a quantidade de corrente que passam pelo circuito.

#### Transistor 
> * Serve para ajustar a corrente que será alimentada ao dispositivo. Ele aplifica a corrente sem exigir que uma grande corrente passe pelo resistor ligado ao Zener. 
> * Como é possível ter um resistor grande o suficiente para evitar que o Zener queime e pequeno o bastante para alimentar o dispositivo com a corrente necessária? > Utilize um transistor NPN!
> * Um "defeito" natural desse tipo de transistor é que ele não pode passar mais tensão do que a tensão da base - 0.7. Porém, nesse caso, isso é uma vantagem, pois mesmo com uma corrente muito pequena, a base do transistor será capaz de estabelecer uma tensão máxima.
> * Utilizando a corrente que passa pela base como referência, ele amplifica essa em 100 vezes. No pior caso (12V) ele recebe 1mA na base, e emite 100mA pelo emissor.

>  ![](img/transistor.gif) 

# Projeto Esquemático do PCB no Software Eagle
![Esquema do Eagle](img/photo_2024-06-27_01-11-25.jpg "Esquema do Eagle")

![Esquema do Eagle](img/photo_2024-06-27_01-11-38.jpg "Esquema do Eagle")

# [Link para o vídeo da fonte sendo testada no laboratório :)](https://youtu.be/FP3eQh2uglU) 


