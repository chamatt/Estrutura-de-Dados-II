# Insertion Sort

Pseudocódigo:

```
InsertionSort(array, n)
    for i <-- 2 to n
        aux <-- array[i]
        j <-- i - 1
        while(j > 0 and array[j] > aux) do
            array[j + 1] <-- array[j]
            j <-- j - 1
        array[j +  1] <-- aux
```

Javascript:

```javascript
function insertSort(array) {
  const n = array.length;
  for (let i = 1; i < n; i++) {
    let aux = array[i];
    let j = i - 1;
    while (j >= 0 && array[j] > aux) {
      array[j + 1] = array[j];
      j = j - 1;
    }

    array[j + 1] = aux;
  }
}

const list = [10, 3, 5, 1, 2, 9, 6];
insertSort(list);
console.log("Lista Ordenada", list);
// Lista Ordenada: [1, 2, 3, 5, 6, 9, 10]
```

O que devemos utilizar para medir o tempo de execução dos algorítmos? Comparações e atribuições.

### Quantas comparações o Insertion Sort faz para n elementos no melhor caso? **n-1**

### Quantas comparações o Insertion Sort faz para n elementos no melhor caso? **Σ <sup>(n)</sup> <sub>(i = 2)</sub> i - 1**

### Quantas comparações o Insertion Sort faz para n elementos no caso médio? **Fica para a próxima aula**
