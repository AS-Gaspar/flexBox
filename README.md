Estudos de flexbox para desenvolvimento web responsivo

ANOTAÇÕES: 

AULA 01 - INTRODUÇÃO

- Flex container
- Elementos filhos

----------------------------------/

AULA 02 - Eixos: 

- flex-direction: row;
- flex-direction: column;
- flex-direction: reverse-row;
- flex-direction: reverse-column;

----------------------------------/

AULA 03 - Wrap (enpacotamento):

- flex-wrap: no-wrap; (Encolhe elementos)
- flex-wrap: wrap; (Muda elemento baseado no sentindo do eixo)
- flex-wrap: wrap-reverse; (Muda elemento baseado no sentindo do eixo)

----------------------------------/

Extra: 
- flex-flow: row nowrap;
- flex-flow: auto;
(Junção das duas declarações) 

----------------------------------/

AULA 04 - Alinhamento dos elementos 

JUSTIFY-CONTENT (Eixo main)

- justify-content: flex-start; (itens alinhados, com o espaço em branco ficando ao final do "main start", que é a referência utilizada nos eixos)
- justify-content: flex-end; (O inverso do acima)
- justify-content: center; (centraliza os elementos)
- justify-content: space-between; (Distribui os elementos por igual no conainer)
- justify-content: space-evenly; (Centraliza, com bordas de tamanho igual ao que os elementos possui entre eles)
- justify-content: space-around
(Cada elemento possui espaços próprios, esses espaços acabam se "somando", no resultado final)

ALIGN-ITEMS (Eixo cross)

- align-items: strech;
(Os elementos estivam )

- align-items: flex-start (Items colam no inicio)

- align-items: flex-end; (Items colam no final)

- align-items: center; (Coloca no centro)

----------------------------------/

AULA 5 e 6: Centralizar elementos

ALIGN CONTENT: Alinha os elementos no eixo transversal, quanso eles estão empacotados.

- align-content: stretch; (Estica os elementos proporcionalmente em relação ao tamanho do container)

- align-content: flex-start (Coloca todos agupados no inicio)

- align-content: flex-end (Coloca todos agrupados no fim)

- align-content: center (centraliza de forma agrupada)

- align-content: space between (O espaço livre fica no meio do container, com od elementos no inicio e fim)

- align-content: space-evenly (Espaços distribuidos)

- align-content: space-around (Divide o eixo transversal em dois, e centraliza os elementos nessas divisões)

-------------------------------------/

AULA 07: Propriedades dos elementos

ORDER:(default é 0)

Basicamente o order serve para colocar um index nos elementos, e o CSS ordena esses elementos do menos para o maior.

ALIGN-SELF: 

- align-self: auto; (padrão vertical)

- align-self: start; (Alinhamento cross start)

- align-self: end (Alinhamento cross end);

- align-self: center; (Calcula o centro entre o cross start e cross end)

- align-self: stretch; (Estica, para preencher tudo)

-------------------------------------/

AULA 08: FLEX BASIS

- flex-basis: auto; (A lagura do elemento é dada com base no tamanho do conteúdo)

- flex-basis: 200px; (Pode ser qualquer valor. Será o valor inicial, porém se for necessário aumentar ou diminuir o elemento, ele fará)

-------------------------------------/

AULA 09: Controle de tamanhos

- flex-shrink: 1; ( 1 = pode encolher)
- flex-grow: 0; ( 0 = não pode crescer)

Sobre os valores:

Zero: significa que o tamanho é fixo

Um: Significa que o tamanho altera

Maiores que 1: Será proporcional aos outros valores. Ex: 0 - 1 - 2
 O elemento 2 crescerá o dobro do elemento 1, e o elemento 0 não altera.

 ------------------------------------/

 AULA 10: Propriedades Flex

Simplicação de Basis, Shrink e Grow:

 Ordem: Grow - Shrink - basis
 
 /* flex-basis: 150px;
    flex-grow: 0;
    flex-shrink: 1; */

- flex: 1 1 150px;

/*flex: 0 1 auto;*/

- flex: initial;

 /* flex: 0 0 auto; */
    
- flex: none;

/* flex: 1 1 auto; */

- flex: auto;

*Colocar apenas um número, (Ex: 3), significa que grow será 3, shrink e basis serão default*


