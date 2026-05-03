a) Java

int k = (j + 13) / 27;

while (k <= 10) {
    k = k + 1;
    int i = 3 * k - 1;
}


b) Python

k = (j + 13) // 27

while k <= 10:
    k = k + 1
    i = 3 * k - 1


c) Haskell

loop k =
    if k > 10
    then ()
    else
        let k' = k + 1
            i = 3 * k' - 1
        in loop k'

main = do
    let k = (j + 13) `div` 27
    loop k


d) Swift

var k = (j + 13) / 27

while k <= 10 {
    k = k + 1
    let i = 3 * k - 1
}



#### Análise entre as linguagens ####

O Python é o mais tranquilo de usar. É necessário escrever menos coisa, não precisa ficar se preocupando com muitos detalhes, e o código fica bem parecido com o que pensamos. É tipo “pensou, escreveu”.

O Java e o Swift já são um pouco mais “certinhos”. É preciso colocar mais coisas no código, como tipo de variável, chaves, essas coisas. Dá um pouco mais de trabalho pra escrever e fica mais “carregado” de olhar.

Agora o Haskell é o mais diferente de todos. Ele não usa aquele jeito normal de fazer repetição com while. Em vez disso, usa recursão, que é tipo uma função chamando ela mesma. Pra quem tá começando, isso costuma confundir bastante.

Resumindo bem simples:

Python: mais fácil de escrever e entender
Java e Swift: mais organizados, mas mais “burocráticos”
Haskell: mais complicado nesse caso

Se fosse pra escolher o melhor pra esse código, o Python ganha fácil, porque resolve tudo de um jeito mais rápido e direto.
