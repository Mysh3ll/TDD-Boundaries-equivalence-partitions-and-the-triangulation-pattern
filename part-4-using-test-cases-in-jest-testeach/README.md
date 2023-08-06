Utilisation des cas de test dans Jest
=====================================

**Ressources**: [Jest test.each](https://jestjs.io/fr/docs/api#testeachtablename-fn-timeout)

Dans cette partie, nous explorons une fonctionnalité de Jest appelée `test.each` qui permet d'écrire un seul test avec plusieurs entrées, souvent appelées cas de test dans d'autres frameworks de tests unitaires. Avec `test.each`, vous pouvez fournir un tableau de données en tant que paramètre et spécifier les valeurs d'entrée pour chaque exécution du test, une fois pour chaque élément du tableau. 📝

Cette fonctionnalité est utile lorsque vous avez plusieurs scénarios de test qui couvrent une même règle ou fonctionnalité. Au lieu d'écrire des tests distincts pour chaque scénario, vous pouvez les combiner en un seul test avec des entrées différentes.

Un exemple est donné en utilisant le jeu "Pierre-Papier-Ciseaux". Les scénarios où le papier bat la pierre et le papier perd contre les ciseaux sont combinés en un seul test à l'aide de `test.each`. Cela permet de maintenir un ensemble clair de règles de test tout en couvrant différents cas de test pour une même règle. 🎲

Cependant, il est important de ne pas abuser des cas de test pour ne pas surcharger un seul test avec trop de scénarios. Si vous avez des règles très distinctes, il est préférable de les maintenir dans des blocs de description séparés pour une meilleure lisibilité et maintenabilité.

Le kata fizzbuzz sera abordé dans la prochaine partie où nous mettrons en pratique les concepts que nous avons appris, y compris l'utilisation des cas de test pour écrire des tests plus efficaces et lisibles. Restez à l'écoute ! 🚀