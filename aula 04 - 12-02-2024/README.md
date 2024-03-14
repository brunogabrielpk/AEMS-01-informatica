## Resumo da aula de hoje
Na aula de hoje nós trabalhamos novamente com a fómular `procv` (ou `vlookup` no inglês)
Também vimos as fórmulas `somase` e `cont.se` (`sumif` e `countif` respectivamente).

### Função SOMASE:
A função SOMASE permite somar valores em um intervalo que atendem a um critério específico.
Sua sintaxe é:
```
=SOMASE(intervalo; critério; [intervalo_soma])
``` 
Onde:
- intervalo: Especifica o conjunto de células que serão avaliadas pelo critério.
- critério: Define o teste a ser feito em cada célula do intervalo.
- [intervalo_soma]: Especifica o intervalo que será somado (opcional).

**Exemplo**:

```
=SOMASE(B5:B9; "junho"; C5:C9)
```

Nesse exemplo, a função soma os valores da coluna C quando o critério (na coluna B) é “junho”.

### Função CONT.SE:
A função CONT.SE conta a quantidade de células preenchidas de acordo com um critério específico.
Sua sintaxe é:
```
=CONT.SE(intervalo; "critério")
```

Onde:
- intervalo: Especifica o intervalo que será testado.
- "critério": Define o teste a ser feito em cada célula do intervalo (pode ser um número, texto ou referência de célula).

**Exemplo**:
```
=CONT.SE(idade; ">30")
```

Nesse exemplo, a função conta quantas vezes a idade é maior que 30.