Introduction au Kata Fizz Buzz
================================================================

Bienvenue dans cette section consacrée aux limites, aux partitions d'équivalence et au pattern de triangulation. L'exercice que nous allons 
utiliser pour mettre en pratique une partie de la théorie est le **Kata Fizz Buzz**. Encore une fois, cet exercice est très simple parce que nous pratiquons le cycle du **TDD**. Nous n'essayons pas de vous poser des problèmes difficiles à résoudre.

Nous essayons de rendre les problèmes faciles. Et même familiers, mais nous allons utiliser le **TDD** pour les résoudre et spécifiquement quelques concepts théoriques que nous allons couvrir dans cette section. Pour cet exercice, vous devez créer une fonction qui accepte un nombre naturel et renvoie une chaîne de caractères en utilisant les règles suivantes.

*   Le nombre est divisible par trois, retourner "Fizz".
*   S'il est divisible par 5, retourner "Buzz".
*   S'il est divisible par 3 et 5, retourner "FizzBuzz".
*   Sinon, le nombre lui-même est retourné sous forme de chaîne de caractères.

Nous aurons à nouveau des cas de test.

Cas de test :
-------------

|  Input N°  |  Output String  |
|:-------------:|:---------------:|
|  1  |  "1"  |
|  2  |  "2"  |
|  3  |  "Fizz"  |
|  4  |  "4"  |
|  5  |  "Buzz"  |
|  6  |  "Fizz"  |
|  9  |  "Fizz"  |
|  10  |  "Buzz"  |
|  15  |  "FizzBuzz"  |
|  16  |  "16"  |
|  20  |  "Buzz"  |
|  30  |  "FizzBuzz"  |
|  75  |  "FizzBuzz"  |
|  77  |  "77"  |

Vous pouvez voir que pour une entrée de 1, la sortie devrait être "1". Avec une entrée de 2, la sortie doit être "2". Pour 3, "Fizz". Pour 4, "4". Pour 5, "Buzz", et ainsi de suite.

Il existe donc un ensemble de cas de test que vous pouvez utiliser pour faire ce kata, et nous y reviendrons. Encore une fois, il ne s'agit que d'exemples. Ils sont là pour vous aider à trouver le prochain test à écrire, mais vous n'êtes pas obligé de les suivre tels que nous les avons donnés.

Si vous souhaitez aborder le problème dans un ordre différent, n'hésitez pas à le faire. Il y a un bonus ici où vous pouvez retourner "Whiz" si le nombre est premier, et c'est quelque chose que vous pouvez faire si vous voulez vous mettre un peu au défi. Maintenant que nous avons examiné le problème, voyons quelle théorie nous allons utiliser pour le résoudre, puis nous ferons la mise en route pour vous permettre de commencer à travailler sur le problème. 👩‍💻