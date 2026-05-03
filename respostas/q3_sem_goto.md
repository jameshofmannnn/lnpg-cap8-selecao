a) Python

j = -3
i = 0

while i < 3 and j <= 0:
    if j + 2 == 3 or j + 2 == 2:
        j -= 1
    elif j + 2 == 0:
        j += 2
    else:
        j = 0

    if j <= 0:
        j = 3 - i

    i += 1


    b) Java

    int j = -3;
int i = 0;

while (i < 3 && j <= 0) {
    if (j + 2 == 3 || j + 2 == 2) {
        j--;
    } else if (j + 2 == 0) {
        j += 2;
    } else {
        j = 0;
    }

    if (j <= 0) {
        j = 3 - i;
    }

    i++;
}


c) JavaScript

let j = -3;
let i = 0;

while (i < 3 && j <= 0) {
    if (j + 2 === 3 || j + 2 === 2) {
        j--;
    } else if (j + 2 === 0) {
        j += 2;
    } else {
        j = 0;
    }

    if (j <= 0) {
        j = 3 - i;
    }

    i++;
}