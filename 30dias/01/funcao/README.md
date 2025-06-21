# leetcode

### Visão geral

Esta questão pretende ser uma introdução às funções JavaScript. Este editorial abordará sua sintaxe e tópicos como _**fechamentos**_ e _**funções de ordem superior**_ .

Se você é iniciante em JavaScript, é recomendável seguir os exemplos de código. Você pode fazer isso colando o código no [playground](https://leetcode.com/playground/) LeetCode .

Uma coisa incrível sobre JavaScript é que seu navegador tem um ambiente de execução integrado. Você pode ler mais sobre como executar código no seu navegador (e visualizar o código de um site) [aqui](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Tools_and_setup/What_are_browser_developer_tools) .

#### Sintaxe da função

Em JavaScript, há duas maneiras principais de declarar uma função. Uma delas é usar a `function`palavra-chave .

##### Sintaxe [ básica ](https://github.com/GersonESantos/leetcode/tree/main/30dias/01/funcao/basica)
Neste exemplo, fé o nome da função. (a, b)são os argumentos. Você pode escrever qualquer lógica no corpo e, por fim, returnum resultado. Você não pode retornar nada, e, em vez disso, retornará implicitamente undefined.

Função Anônima
Você pode, opcionalmente, excluir o nome da função após a functionpalavra-chave.

Expressão de Função [ Invocada ] (https://github.com/GersonESantos/leetcode/tree/main/30dias/01/funcao/Invocada)Imediatamente (IIFE)
Você pode criar uma função e executá-la imediatamente em Javascript.
Por que você escreveria um código assim? Ele lhe dá a oportunidade de encapsular uma variável dentro de um novo escopo . Por exemplo, outro desenvolvedor pode ver imediatamente que sumela não pode ser usada em nenhum lugar fora do corpo da função.

[Funções dentro de funções](https://github.com/GersonESantos/leetcode/tree/main/30dias/01/funcao/func%20dentro%20de%20funcao)
Um recurso poderoso do JavaScript é que você pode criar funções dentro de outras funções e até mesmo retorná-las!
Neste exemplo, createFunction()retorna uma nova função. Essa função pode ser usada normalmente.

[Função de elevação](https://github.com/GersonESantos/leetcode/tree/main/30dias/01/funcao/eleva%C3%A7%C3%A3o)
JavaScript possui um recurso chamado hoisting , no qual uma função pode, às vezes, ser usada antes de ser inicializada. Você só pode fazer isso se declarar funções com a functionsintaxe .
Neste exemplo, a função é retornada antes de ser inicializada. Embora seja uma sintaxe válida, às vezes é considerada uma prática ruim, pois pode reduzir a legibilidade.

[Fechamentos](https://github.com/GersonESantos/leetcode/tree/main/30dias/01/funcao/Fechamentos)
Um tópico importante em JavaScript é o conceito de closures . Quando uma função é criada, ela tem acesso a uma referência para todas as variáveis ​​declaradas ao seu redor, também conhecido como seu ambiente léxico . A combinação da função e seu ambiente é chamada de closure . Este é um recurso poderoso e frequentemente utilizado da linguagem.
Neste exemplo, createAdderpassa o primeiro parâmetro ae a função interna tem acesso a ele. Dessa forma, createAdderserve como uma fábrica de novas funções, com cada função retornada tendo um comportamento diferente.

Sintaxe de [seta](https://github.com/GersonESantos/leetcode/tree/main/30dias/01/funcao/seta)
A outra maneira comum de declarar funções é com a sintaxe de seta. Aliás, em muitos projetos, essa é a sintaxe preferida.

Sintaxe básica
Neste exemplo, fé o nome da função. (a, b)são os argumentos. Você pode escrever qualquer lógica no corpo e, por fim, returnum resultado. Você não pode retornar nada, e, em vez disso, retornará implicitamente undefined.

[Omitir retorno](https://github.com/GersonESantos/leetcode/tree/main/30dias/01/funcao/Omitir%20retorno)
Se você conseguir escrever o código em uma única linha, pode omitir a returnpalavra-chave. Isso pode resultar em um código muito curto.
Diferenças
Há três diferenças principais entre a sintaxe de seta e a sintaxe de função.

Sintaxe mais minimalista. Isso é especialmente verdadeiro para funções anônimas e funções de linha única. Por esse motivo, essa abordagem é geralmente preferida ao passar funções anônimas curtas para outras funções.
Sem elevação automática. Você só pode usar a função depois que ela for declarada. Isso geralmente é considerado bom para a legibilidade.


Não pode ser vinculado a `this`, `super`e `arguments`ou ser usado como construtor. Todos esses são tópicos complexos por si só, mas a conclusão básica é que as funções de seta são mais simples em seu conjunto de recursos. Você pode ler mais sobre essas diferenças [aqui](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) .




A escolha entre sintaxe de seta e sintaxe de função depende principalmente da preferência e dos padrões de estilo do seu projeto.

#### Argumentos de descanso

Você pode usar a sintaxe _**REST**_ para acessar todos os argumentos passados ​​como um array. Isso não é necessário para este problema, mas será um conceito crítico para muitos outros. Você pode ler mais sobre `...`sintaxe [aqui](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax) .

##### Sintaxe básica

A sintaxe é:




