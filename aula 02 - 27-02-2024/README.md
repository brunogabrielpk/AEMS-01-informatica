# Resumo da aula de hoje 
Hoje nós trabalhamos exercícios adicionais baseados nas fórmulas já mencionadas na aula passada.
Reforçamos o funcionamento das fórmulas **SOMA** e **MÉDIA** e vimos uma rápida introdução a fórmula **SE**

A função **SE** permite que você faça comparações lógicas entre um valor e o que você espera. Ela tem a seguinte sintaxe:

```
=SE(teste_lógico; valor_se_verdadeiro; valor_se_falso)
```

aqui estão os argumentos(Ou Parâmetros):

- **teste_lógico** (obrigatório): A condição que você deseja testar.
- **valor_se_verdadeiro** (obrigatório): O valor que será retornado se o resultado do teste_lógico for VERDADEIRO.
- **valor_se_falso** (opcional): O valor que será retornado se o resultado do teste_lógico for FALSO.


Exemplos simples de uso da função **SE**:

`=SE(C2="Sim"; 1; 2)`: Se o valor em C2 for igual a “Sim”, retorna 1; caso contrário, retorna 2.

`=SE(C2=1; "Sim"; "Não")`: Se o valor em C2 for igual a 1, retorna “Sim”; caso contrário, retorna “Não”.


## Arrastando fórmulas
Também conversamos a respeito do recurso de "arrasto" de funções sobre a planilha.
Tanto no Excel quanto no google Sheets,é possível arrastar funções de modo que o programa vai ajustar os endereços das células de acordo com a quantidade de células deslocadas.
Por exemplo: se você arrastar uma fórmula horizontalmente, os valores das colunas existentes na célula irão ser alterados de acordo com o número de células deslocados. Assim, se na sua célula você possuir o seguinte valor, `=F5` e então arrastar a célula para direita por três células, o novo valor será `=I5`. Isso porquê a coluna I está a três colunas da coluna F.
O mesmo vale para deslocamento vertical, coma diferença de, no caso das linhas, quem irá variar será o número ao invés da letra.

Por fim, é possível "travar" os endereços de célula para evitar o recurso do 'arrasto'. Para isso basta adicionar um cifão `$` antes da letra para travar a coluna e um cifrão `$` antes do número para travar a linha. 