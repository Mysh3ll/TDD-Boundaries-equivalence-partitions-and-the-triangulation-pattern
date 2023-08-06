Limites et partitions d'équivalence
================================================================

Dans cette partie, nous allons nous pencher sur les partitions d'équivalence et les limites. Ce sont des concepts très utiles lorsqu'on réfléchit à la manière de formuler les tests que l'on doit écrire.

Une **partition d'équivalence** est simplement un groupe de valeurs pour lesquelles le comportement du code est le même, ou le comportement que vous voulez dans le code est le même.

Une **limite (ou frontière)** est l'endroit où deux partitions d'équivalence se rencontrent. C'est là que le code passe d'un comportement à un autre.

Si nous examinons un exemple, voici une fonction simple qui prend un nombre et renvoie une chaîne de caractères.


```ts
function print(input: number): string {
    if (input <= 0) { return 'TDD' };
    if (input > 0 && input <= 99) { return 'is' };
    return 'awesome';
}
```

Nous identifions trois partitions d'équivalence dans ce code :

1.  Les nombres inférieurs ou égaux à zéro. **'TDD'**
2.  Les nombres entre 1 et 99 inclus. **'is'**
3.  Les nombres supérieurs à 100. **'awesome'**

'TDD' | 'is' | 'awesome'
--- | --- | ---
..., -2, -1, 0 | 1, 2, 3, ..., 98, 99 | 100, 101, 102, ...


Entre ces partitions, il y a des limites, qui sont des endroits critiques à tester. Les valeurs à gauche et à droite des limites sont les plus précieuses à tester, car elles sont susceptibles de provoquer des erreurs de décalage.

L'exercice **FizzBuzz** est un exemple de partitions d'équivalence non linéaires, où les nombres ne suivent pas un ensemble contigu. Dans ce cas, nous écrivons des tests pour au moins 3 valeurs dans chaque partition d'équivalence pour assurer une couverture adéquate.

'Autre' | 'Fizz' | 'Buzz' | 'FizzBuzz'
--- | --- | --- | ---
1, 2, 4, 7, 8, 11 et tous les nombres qui ne sont pas dans les autres partitions | 3, 6, 9, 12, 18, 21... | 5, 10, 20, 25, 35... | 15, 30, 45, 60, 75...
Nombres non divisibles par 3 ou 5 | Nombres divisibles par 3 mais pas par 5 | Nombres divisibles par 5 mais pas par 3 | Nombres divisibles par 3 et 5

Les partitions d'équivalence et les limites sont essentielles pour une couverture de test complète et une détection précoce de bugs. Nous utiliserons ces concepts dans l'exercice **FizzBuzz**. Voyons cela en action dans la suite du cours. 👩‍💻