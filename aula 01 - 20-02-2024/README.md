# Introdução
A aula de hoje foi um simples introdução do nosso conteúdo e que será melhor trabalhado mais adiante
Uma vez definido o ponto inicial, nós começamos falando de editores de planilhas

## Planilhas
Um ponto importante que foi descrito é a definição do que é uma planilha.

> Um planilha é uma coleção de células endereçadas.
> Uma célula é intersecção de uma linha com uma coluna.

Também é importante frizar que ascolunas são nomeadas (definidas por letras)
e as linhas são numeradas (definidas por números) e que o endereço de cada célula, que é uma valor fixo,
é definido a partir da junção de sua coluna com sua linha (A1,C37, h89, ...).

**Microsoft Excel**, **Apple Numbers**, **Planilhas Google**, **LibreOffice Calc** são alguns exemplos de softwares editores de planilhas. 

Embora a interface de usuário de cada um desses softwares sejam diferentes, a maneira como as células se comportam em cada um deles
é bastante similar.

Em suma, nós podemos inserir valores em uma célula e fazê-la interagir com outras células a depender desses valores.
> O valor a ser armazenado é uma célula por ser um valor vazio, númerico, de caractes, datas, etc. Esse valor também pode ser alterado, poré o endereço da célula será sempre o mesmo.
Essas interações vão depender do tipo do valor armazenado em cada uma das células envolvidas.

## Funções
As interações entre as células são, na maioria das vezes, resultados de uma função.
A maneira como nós sinalizamos para nosso software editor de planilhas que ele deve resolver uma função e retornar o resultado
eé através do sinal de `=`
> Por questões de praticidade, daqui em diante, eu vou chamar o software editor de planilhas de Excel ou Sheets

Uma vez que o valor armazenado em uma célula começe com o sinal de `=`, o Excel, ou o Sheets, 'entende' que aquela célula contém uma função.
Considere a tabela abaixo
|**A** | **B** |**C**|**D**|
|:---:|:---:|:---:|:---:|
|Aluno | Nota1 | Nota2 | Média|
|Ana| 10 | 5 | 7,5|

Assim temos os seguintes valores nas suas respectivas células, A2 (Ana), B2 (10), C2 (5), D2 (7,5).
Os números 10 e 5 são valores que foram adicionados manualmente mas o valor 7,5 é o resultado de uma função (que no case é uma função de calcular média).

### Função Soma
A função **SOMA** no Excel é utilizada para **adicionar valores**. Ela pode somar valores individuais, referências de células, intervalos ou uma combinação dos três. Por exemplo:
- **=SOMA(A2:A10)** Soma todos os valores presentes nas células de A2 até A10
- **=SOMA(A2:A10;C2:C10)** Soma todos os valores presentes nas células de A2 até A10 bem como valores presentes nas células de C2 até C10

Destrinchando o exemplo para facilitar o entendimento:
- **=** Sinal de igual no início para indicar que se trada de uma função
- **SOMA** É o nome da função, que nesse caso realiza a operação de somar. Em geral o nome da função coincide com o que de fato ela realiza mas isso não é um regra.
- **(XXXXXXXX)** As funções veem acompahandas de parênteses `()` que podem conter informações dentro deles ou não. Essas informações são chamadas de parâmetros da função. 
- **A2:10** São os parâmetros da função(as vezes chamados de argumentos) no exemplo acima. Note que o sinal de dois pontos `:` indica um intervalo de células, ou seja, todas as células entre A2 e A10.
Uma outra observação é o sinal deponto e vírguls `;`, que é um separador de parâmetros. Ele pode separar intervalos de células ou células individuais. Por fim é importante de mencionar que a função **SOMA** não possui um número fixo de parâmetros, assim, você somar múltiplas células e intervalos. existem funções que contém número de parâmetros definidos.

### Função MÉDIA
 A função MÉDIA no Excel e no Planilhas Google é utilizada para calcular a média aritmética simples de um conjunto de valores.
 Por exemplo, se você tiver um intervalo de células A1:A20 com valores, a fórmula =MÉDIA(A1:A20) retornará a média desses valores.

### Função SE
A função **SE** é amplamente utilizada no **Excel** e no **Google Sheets** para definir condições lógicas. Ela permite que você especifique o que deve acontecer com base em uma expressão verdadeira ou falsa. Vou explicar como usar essa função em ambos os softwares:
- A sintaxe da função **SE** é a seguinte:
- ```=SE(expressão_lógica; valor_se_verdadeiro; valor_se_falso)```

Aqui estão os argumentos:
- **expressão_lógica**: Uma expressão ou referência a uma célula que avalia como verdadeira ou falsa.
- **valor_se_verdadeiro**: O valor que será retornado se a expressão lógica for verdadeira.
- **valor_se_falso**: O valor que será retornado se a expressão lógica for falsa.