De modo abstrato, o compilador é um programa que converte código de uma
linguagem para outra. Como se fosse uma função do tipo `compilador(str) -> str`.
No caso de compiladores que emitem código de máquina ou bytecode, seria mais
preciso dizer `compilador(str) -> bytes`, mas a idéia básica é a mesma.

De forma geral o processo é dividido em etapas como abaixo

```python
def compilador(x1: str) -> str | bytes:
    x2 = lex(x1)        # análise léxica
    x3 = parse(x2)      # análise sintática
    x4 = analysis(x3)   # análise semântica
    x5 = optimize(x4)   # otimização
    x6 = codegen(x5)    # geração de código
    return x6
```

Defina brevemente o que cada uma dessas etapas realizam e marque quais seriam os
tipos de entrada e saída de cada uma dessas funções. Explique de forma clara o
que eles representam. Você pode usar exemplos de linguagens e/ou compiladores
conhecidos para ilustrar sua resposta. Salve sua resposta nesse arquivo.

# lex(?) -> Meio que essa linguagem lexica serve para dividir o codigo em pedaços menores, divide em palavras chaves como "if", "while", "var" e variaveis, numeros e entre outros, é assim que o compilador consegue ler o codigo
Complete as ? e responda aqui!
 
# parse(?) -> Depois que o léxico separou os pedaços, o parse vai organizar esses pedaços em uma estrutura, como se fosse uma árvore que representa o código. É aqui que o compilador entende a estrutura
Complete as ? e responda aqui!

# analysis(?) -> Agora o compilador olha e vê se o código faz sentido de verdade, verificando, por exemplo, se você está usando uma variável que foi realmente criada ou se não está tentando fazer operações que não fazem sentido, como somar uma string com um número. É nessa etapa que ele encontra erros mais lógicos, coisas que a análise de sintaxe deixou passar, mas que não podem ser feitas no funcionamento do programa.
Complete as ? e responda aqui!

# optimize(?) -> Aqui o compilador melhora seu código automaticamente. Se você escreve algo meio "besta", é como se fosse um “limpa-código”
Complete as ? e responda aqui!

# codegen(?) -> Essa é a parte que o compilador tranforma tudo que ta no codigo e tentar rodar ele em alguma linguagem, como codigo de maquina ou até mesmo outra linguagem como typescript, em algo que realemnte o computador entender
Complete as ? e responda aqui!