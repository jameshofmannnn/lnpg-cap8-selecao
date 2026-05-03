a) C

switch (k) {
    case 1:
    case 2:
        j = 2 * k - 1;
        break;
    case 3:
    case 5:
        j = 3 * k + 1;
        break;
    case 4:
        j = 4 * k - 1;
        break;
    case 6:
    case 7:
    case 8:
        j = k - 2;
        break;
}


b) Ruby

case k
when 1, 2
  j = 2 * k - 1
when 3, 5
  j = 3 * k + 1
when 4
  j = 4 * k - 1
when 6, 7, 8
  j = k - 2
end


c) Erlang

J = case K of
    1 -> 2 * K - 1;
    2 -> 2 * K - 1;
    3 -> 3 * K + 1;
    5 -> 3 * K + 1;
    4 -> 4 * K - 1;
    6 -> K - 2;
    7 -> K - 2;
    8 -> K - 2
end.


#### Análise entre as linguagens ####

O C resolve o problema, mas é mais manual e trabalhoso. Tem que ficar colocando case, break e tomar cuidado pra não esquecer nada, senão o código dá problema. Funciona bem, mas dá mais trabalho do que precisava.

O Ruby já é bem mais tranquilo. Dá pra juntar vários valores na mesma linha, tipo 1, 2, e o código fica bem limpo. Dá para entender o que está acontencendo sem tanto esforço assim.

O Erlang é o mais diferente. Ele não deixa fazer essas “junções” tão fácil, então  acaba repetindo mais coisa. Além disso, o jeito dele escrever já é meio estranho pra quem tá acostumado com outras linguagens.

Resumindo bem simples:

C: funciona, mas é meio trabalhoso
Ruby: mais simples, mais limpo e fácil de entender
Erlang: mais complicado e diferente