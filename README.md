![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# LAB | JS Fonctions & Arrays

<details>
  <summary>
   <h2>Objectifs d'apprentissage</h2>
  </summary>

  Cet exercice vous permet de pratiquer et d'appliquer les concepts et les techniques enseignés en classe.

  À la fin de cet exercice, vous serez capable de :

  - Exécuter des tests prédéfinis dans Jasmine pour vérifier que le programme répond aux exigences techniques.
  - Identifier le comportement attendu du code en lisant et en comprenant les résultats des tests et les erreurs.
  - Déclarer et invoquer des fonctions en utilisant la syntaxe de déclaration de fonction, d'expression de fonction et de fonction fléchée.
  - Utiliser le mot-clé `return` pour renvoyer une valeur à partir d'une fonction.
  - Passer des valeurs primitives en tant qu'arguments aux fonctions.
  - Passer des tableaux en tant qu'arguments aux fonctions.
  - Accéder aux éléments stockés dans les tableaux en utilisant les index.
  - Add, remove and check for items in an array using the index and array methods (`unshift`, `push`, `splice`, `shift`, `pop`, `indexOf`, and `includes`).
  - Ajouter, supprimer et vérifier les éléments dans un tableau en utilisant les méthodes d'index et de tableau (`unshift`, `push`, `splice`, `shift`, `pop`, `indexOf`, et `includes`)
  - Parcourir les tableaux à l'aide des boucles `for` et `forEach`.

  <br>
  <hr> 

</details>

## Introduction

La manipulation de tableaux est une tâche courante en programmation. Que vous calculiez un total pour un panier d'achat, que vous ne récupériez que les prénoms d'une liste de personnes ou que vous déplaciez une pièce sur un échiquier, vous modifiez probablement ou manipulez un tableau quelque part dans le code.
<br>

## Exigences

- Forker ce repo
- Le cloner sur votre machine

## Soumission

- Une fois terminé, exécutez les commandes suivantes :

```bash
git add .
git commit -m "Solved lab"
git push origin master
```

- Créez une Pull Request afin que vos assistants pédagogiques puissent vérifier votre travail.

## Introduction aux tests automatisés

### Qu'est-ce que le test automatisé ?

Le test automatisé de logiciel est le processus d'exécution programmée d'une application pour valider et vérifier qu'elle répond aux besoins commerciaux ainsi qu'aux exigences techniques et qu'elle se comporte comme prévu.

Les tests doivent être considérés comme un processus continu, et non comme une opération distincte ou une activité unique dans le cycle de développement. Concevoir des tests dès le début du cycle de vie du produit peut atténuer les problèmes courants qui surviennent lors du développement de bases de code complexes.

Disposer d'un ensemble de tests solide peut vous donner la tranquillité d'esprit, car vous serez en mesure d'améliorer en toute confiance votre travail tout en sachant que vous ne cassez pas une fonctionnalité déjà développée.
<br>

### Laboratoires de test

Ce laboratoire, ainsi que certains laboratoires sur lesquels vous travaillerez pendant le bootcamp, sont équipés de tests unitaires pour fournir des retours automatisés sur votre progression en laboratoire.
<br>

### Test avec Jasmine

Jasmine est un cadre de test automatisé pour JavaScript. Il est conçu pour être utilisé dans la programmation de développement axée sur le comportement (**BDD**), en mettant davantage l'accent sur la valeur commerciale que sur les détails techniques.

Nous avons déjà inclus Jasmine dans le projet que vous venez de cloner, alors voyons comment l'utiliser pour implémenter notre code.
<br>

### Utilisation

Avant de commencer à coder, nous vous expliquerons la structure du projet que nous vous avons fournie :

```
lab-js-functions-and-arrays
  ├── README.md
  ├── SpecRunner.html
  ├── jasmine
  │   └── ...
  ├── src
  │   └── functions-and-arrays.js
  └── tests
      └── functions-and-arrays.spec.js
```

Nous allons travailler avec le fichier `src/functions-and-arrays.js`. Vous pouvez trouver tous les fichiers dans le dossier `jasmine` nécessaires pour utiliser Jasmine. Tous ces fichiers sont déjà liés avec le fichier `SpecRunner.html`.

Si vous souhaitez vérifier les tests, ils se trouvent dans le fichier `tests/functions-and-arrays.spec.js`.


#### Exécuter les tests

Exécuter des tests automatisés avec Jasmine est très facile. Tout ce que vous avez à faire, c'est ouvrir le fichier `SpecRunner.html` dans votre navigateur. Vous y trouverez quelque chose de similaire à ceci :

[![image](https://user-images.githubusercontent.com/23629340/33389609-c2f3965c-d533-11e7-9a03-e0a89314dd98.png)](https://user-images.githubusercontent.com/23629340/33389609-c2f3965c-d533-11e7-9a03-e0a89314dd98.png)


#### Réussir les tests

Vous devez écrire votre code dans le fichier `src/functions-and-arrays.js`. En suivant les instructions pour chaque itération, vous devez vérifier chaque test et vous assurer qu'il réussit avant de passer à la suite.

Ne vous précipitez pas. Prenez votre temps pour lire attentivement chaque itération et corriger les tests qui échouent au fur et à mesure de l'exercice.

Lorsque vous codez avec des tests, il est très important de lire attentivement et de comprendre les erreurs que vous obtenez. De cette manière, vous saurez ce qui est attendu de votre code.

Pour voir la sortie de votre code JavaScript, ouvrez la [Console dans les Outils de développement](https://developer.chrome.com/docs/devtools/open/#console).

**Important** : Notez que **vous n'avez pas besoin d'exécuter les fonctions vous-même** ; les tests chargeront et exécuteront automatiquement les fonctions à chaque exécution du test. Tout ce que vous avez à faire, c'est déclarer les fonctions, vous assurer qu'elles traitent les paramètres transmis et renvoient ce qui est indiqué dans les instructions de l'itération et la description du test. Nous vous fournissons un tableau d'exemple pour certaines itérations, afin que vous puissiez effectuer des tests **manuels** si vous le souhaitez.

## Instructions

En suivant les instructions pour chaque itération, lisez attentivement les instructions et les descriptions des tests pour bien comprendre les exigences de la tâche. Ne vous précipitez pas. Prenez le temps de lire chaque itération attentivement.

<br>

### Itération n°1 : Trouver le maximum

Implémentez la fonction `maxOfTwoNumbers` qui prend deux nombres en argument et renvoie le nombre le plus grand.

<br>

### Itération n°2 : Trouver le mot le plus long

Implémentez la fonction `findLongestWord` qui prend en argument un tableau de mots et renvoie le plus long. S'il y a deux mots de même longueur, il devrait renvoyer la première occurrence.

Vous pouvez utiliser le tableau suivant pour tester votre solution :

```javascript
const words = ['mystery', 'brother', 'aviator', 'crocodile', 'pearl', 'orchard', 'crackpot'];
```

<br>

### Itération #3 : Calculer la somme

#### Itération #3.1 : Additionner les nombres

Calculer une somme peut être aussi simple que d'itérer sur un tableau et d'ajouter chacun des éléments ensemble.

Implémentez la fonction appelée `sumNumbers` qui prend un tableau de nombres en argument et renvoie la somme de tous les nombres du tableau. Plus tard dans le cours, nous apprendrons comment faire cela en utilisant la méthode `reduce` des tableaux, ce qui rendra votre travail considérablement plus facile. Pour l'instant, pratiquons la façon *"déclarative"* d'ajouter des valeurs en utilisant des boucles.

Vous pouvez utiliser le tableau suivant pour tester votre solution :

```javascript
const numbers = [6, 12, 1, 18, 13, 16, 2, 1, 8, 10];
```

<br>

#### Bonus - Itération n°3.2 : Une fonction `sum()` générique

Dans l'itération 3, vous avez créé une fonction qui retourne la somme d'un tableau de nombres. Mais que se passe-t-il si nous voulons calculer la somme des longueurs des mots dans un tableau ? Et si cela inclut également des valeurs *booléennes* ? Pour y parvenir, nous devons créer une fonction qui permet cette flexibilité.

Vous devez implémenter la fonction `sum()` dans cette itération. La fonction doit prendre un tableau de valeurs mixtes - des nombres, des chaînes de caractères et des booléens. La fonction doit ajouter toutes les longueurs des chaînes de caractères, les valeurs numériques et les valeurs numériques des booléens à la somme totale et retourner cette somme. Consultez les tests pour plus de détails.

Vous pouvez utiliser le tableau suivant pour tester votre solution :

```javascript
const mixedArr = [6, 12, 'miami', 1, true, 'barca', '200', 'lisboa', 8, 10];

// should return: 57
```

<br>

### Itération n°4 : Calculer la moyenne

Calculer une moyenne est une tâche courante. Pratiquons un peu.

**La logique derrière cela :**

1. Trouver la somme comme nous l'avons fait dans le premier exercice (ou pourquoi ne pas réutiliser la fonction `sumNumbers()` ?)
2. Diviser cette somme par le nombre d'éléments dans le tableau.

<br>

#### Itération n°4.1 : Tableau de nombres

Implémentez la fonction `averageNumbers` qui prend en paramètre un tableau de nombres et renvoie la moyenne des nombres.

Vous pouvez utiliser le tableau suivant pour tester votre solution :

```javascript
const numbers = [2, 6, 9, 10, 7, 4, 1, 9];
```
<br>

#### Itération #4.2 : Tableau de chaînes de caractères

Implémentez la fonction appelée `averageWordLength` qui reçoit en argument unique un tableau de mots et renvoie la longueur moyenne des mots :

Vous pouvez utiliser le tableau suivant pour tester votre solution :

```javascript
const words = ['seat', 'correspond', 'linen', 'motif', 'hole', 'smell', 'smart', 'chaos', 'fuel', 'palace'];
```

<br>

#### Bonus - Itération #4.3 : Une fonction `avg()` générique

Créez une fonction `avg(arr)` qui reçoit un tableau mixte quelconque et calcule la moyenne. Par exemple, considérez un tableau rempli de nombres et/ou de chaînes de caractères et/ou de booléens en tant que tableau mixte.

Les valeurs non numériques doivent être comptées comme suit :

- Booléens : `true` est compté comme `1` et `false` est compté comme `0`.
- Chaînes de caractères : utilisez la `length` de la chaîne de caractères comme valeur numérique.

```javascript
const mixedArr = [6, 12, 'miami', 1, true, 'barca', '200', 'lisboa', 8, 10];

// should return: 5.7
```

<br>

### Itération n°5 : Tableaux uniques

Prenez le tableau suivant, supprimez les doublons et renvoyez un nouveau tableau. Il est fort probable que vous souhaitiez consulter les méthodes du tableau [`indexOf`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf) et [`includes`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/includes).

Faites ceci sous la forme d'une fonction `uniquifyArray` qui reçoit un tableau de mots en argument.

Vous pouvez utiliser le tableau suivant pour tester votre solution :

```javascript
const words = [
  'crab',
  'poison',
  'contagious',
  'simple',
  'bring',
  'sharp',
  'playground',
  'poison',
  'communion',
  'simple',
  'bring'
];
```

<br>

### Itération n°6 : Trouver des éléments

Créons une recherche simple dans un tableau.

Déclarez une fonction nommée `doesWordExist` qui prendra en argument un tableau de mots et un mot à rechercher. Renvoyez `true` si le mot existe dans le tableau ; sinon, renvoyez `false`.

Vous pouvez utiliser le tableau suivant pour tester votre solution :

```javascript
const words = ['machine', 'subset', 'trouble', 'starting', 'matter', 'eating', 'truth', 'disobedience'];
```

<br>

### Itération n°7 : Compter les répétitions

Déclarez une fonction nommée `howManyTimes` qui prendra en premier argument un tableau de mots et en deuxième argument un mot à rechercher. La fonction renverra le nombre de fois où le mot apparaît dans le tableau.

Vous pouvez utiliser le tableau suivant pour tester votre solution :

```javascript
const words = [
  'machine',
  'matter',
  'subset',
  'trouble',
  'starting',
  'matter',
  'eating',
  'matter',
  'truth',
  'disobedience',
  'matter'
];
```

<br>



### Bonus - Itération n°8



#### Bonus - Itération n°8.1 : Produit de nombres adjacents

Étant donné plusieurs tableaux, trouvez le produit le plus grand de quatre nombres adjacents.

Nous considérons comme adjacents quatre nombres qui se suivent horizontalement ou verticalement. Par exemple, si nous avons une matrice 5x5 comme suit :

```bash
[ 1,  2, 3, 4, 5]
[ 1, 20, 3, 4, 5]
[ 1, 20, 3, 4, 5]
[ 1, 20, 3, 4, 5]
[ 1,  4, 3, 4, 5]
```

Le plus grand produit sera le `20`x`20`x`20`x`4` = `32000`.

<br>

Déclarez une fonction nommée `greatestProduct(matrix)` pour la trouver dans la grille 20×20 ci-dessous !

```javascript
const matrix = [
  [08, 02, 22, 97, 38, 15, 00, 40, 00, 75, 04, 05, 07, 78, 52, 12, 50, 77, 91, 08],
  [49, 49, 99, 40, 17, 81, 18, 57, 60, 87, 17, 40, 98, 43, 69, 48, 04, 56, 62, 00],
  [81, 49, 31, 73, 55, 79, 14, 29, 93, 71, 40, 67, 53, 88, 30, 03, 49, 13, 36, 65],
  [52, 70, 95, 23, 04, 60, 11, 42, 69, 24, 68, 56, 01, 32, 56, 71, 37, 02, 36, 91],
  [22, 31, 16, 71, 51, 67, 63, 89, 41, 92, 36, 54, 22, 40, 40, 28, 66, 33, 13, 80],
  [24, 47, 32, 60, 99, 03, 45, 02, 44, 75, 33, 53, 78, 36, 84, 20, 35, 17, 12, 50],
  [32, 98, 81, 28, 64, 23, 67, 10, 26, 38, 40, 67, 59, 54, 70, 66, 18, 38, 64, 70],
  [67, 26, 20, 68, 02, 62, 12, 20, 95, 63, 94, 39, 63, 08, 40, 91, 66, 49, 94, 21],
  [24, 55, 58, 05, 66, 73, 99, 26, 97, 17, 78, 78, 96, 83, 14, 88, 34, 89, 63, 72],
  [21, 36, 23, 09, 75, 00, 76, 44, 20, 45, 35, 14, 00, 61, 33, 97, 34, 31, 33, 95],
  [78, 17, 53, 28, 22, 75, 31, 67, 15, 94, 03, 80, 04, 62, 16, 14, 09, 53, 56, 92],
  [16, 39, 05, 42, 96, 35, 31, 47, 55, 58, 88, 24, 00, 17, 54, 24, 36, 29, 85, 57],
  [86, 56, 00, 48, 35, 71, 89, 07, 05, 44, 44, 37, 44, 60, 21, 58, 51, 54, 17, 58],
  [19, 80, 81, 68, 05, 94, 47, 69, 28, 73, 92, 13, 86, 52, 17, 77, 04, 89, 55, 40],
  [04, 52, 08, 83, 97, 35, 99, 16, 07, 97, 57, 32, 16, 26, 26, 79, 33, 27, 98, 66],
  [88, 36, 68, 87, 57, 62, 20, 72, 03, 46, 33, 67, 46, 55, 12, 32, 63, 93, 53, 69],
  [04, 42, 16, 73, 38, 25, 39, 11, 24, 94, 72, 18, 08, 46, 29, 32, 40, 62, 76, 36],
  [20, 69, 36, 41, 72, 30, 23, 88, 34, 62, 99, 69, 82, 67, 59, 85, 74, 04, 36, 16],
  [20, 73, 35, 29, 78, 31, 90, 01, 74, 31, 49, 71, 48, 86, 81, 16, 23, 57, 05, 54],
  [01, 70, 54, 71, 83, 51, 54, 69, 16, 92, 33, 48, 61, 43, 52, 01, 89, 19, 67, 48]
];
```

<br>



#### Bonus - Itération #8.2 : Produit des diagonales

En suivant la logique que vous avez utilisée dans l'itération #8.1, déclarez une fonction appelée `greatestProductOfDiagonals(matrix)`. Elle prend une matrice en paramètre et renvoie le produit le plus grand de quatre valeurs disposées en diagonale, dans n'importe quelle direction.

<br>

**Joyeux codage!** :heart:

<br>

## FAQs

<br>

<details>
  <summary>
Je suis bloqué dans l'exercice et je ne sais pas comment résoudre le problème ni par où commencer</summary>
  <br>

  Si vous êtes coincé dans votre code et que vous ne savez pas comment résoudre le problème ou par où commencer, vous devriez prendre du recul et essayer de formuler une question claire sur le problème spécifique auquel vous êtes confronté. Cela vous aidera à cibler le problème et à trouver des solutions potentielles.

  Par exemple, est-ce un concept que vous ne comprenez pas, ou recevez-vous un message d'erreur que vous ne savez pas comment corriger ? Il est généralement utile d'essayer d'exprimer le problème le plus clairement possible, en incluant les éventuels messages d'erreur que vous recevez. Cela peut vous aider à communiquer le problème à d'autres personnes et éventuellement obtenir de l'aide de camarades de classe ou de ressources en ligne.

  Une fois que vous avez une compréhension claire du problème, vous pourrez commencer à travailler vers la solution.

  [Retour en haut](#faqs)

</details>

<details>
  <summary>Tous les tests Jasmine échouent et sont en rouge. Pourquoi cela s'est-il produit ?</summary>
  <br>

  Une raison possible pour laquelle tous les tests Jasmine échouent est qu'il y a une erreur de syntaxe dans le code testé. Si le code contient une erreur de syntaxe, il ne se chargera pas correctement et aucun des tests ne pourra s'exécuter. Cela entraînera l'échec de tous les tests.

  Pour résoudre ce problème, vous devrez examiner le code testé à la recherche d'erreurs de syntaxe. Recherchez des crochets manquants, des points-virgules ou d'autres problèmes de syntaxe qui pourraient être à l'origine du problème. Si vous trouvez une erreur de syntaxe, corrigez-la et essayez de lancer à nouveau les tests.

  Une autre possibilité est qu'il y ait un problème avec les tests eux-mêmes. Il est possible que vous ayez modifié le fichier de test et causé un problème. Si vous avez apporté des modifications au fichier de test, essayez de copier et coller le fichier de test original, puis exécutez à nouveau les tests pour voir si cela résout le problème.

  [Retour en haut](#faqs)

</details>

<details>
  <summary>Comment trouver la longueur d'une chaîne de caractères en JavaScript ?</summary>
  <br>

  Pour trouver la longueur d'une chaîne de caractères, utilisez la propriété `length`. Voici un exemple :

  ```javascript
  const str = "Hello, world!";
  console.log(str.length); // 13
  ```
  La propriété `length` renvoie le nombre de caractères dans la chaîne, y compris les espaces et les caractères spéciaux.

  [Retour en haut](#faqs)

</details>

<details>
  <summary>Comment puis-je boucler sur un tableau ?</summary>
  <br>

  Les boucles vous permettent de répéter un bloc de code un certain nombre de fois. Il existe plusieurs façons de boucler sur un tableau en JavaScript :

<br>

  #### Boucle "for"

  La boucle `for` est la manière la plus traditionnelle de boucler à travers un tableau en JavaScript. Elle se compose de trois parties : *l'initialisation, la condition et l'incrémentation/décrémentation* :

  ```js
  const animals = ['cat', 'dog', 'bird'];

  // initialize counter variable (let i = 0)
  // set condition (i < animals.length)
  // increment counter (i++)
  for (let i = 0; i < animals.length; i++) {
    console.log(animals[i]);
  }
  ```

  À l'initialisation, vous déclarez une variable de compteur et vous lui donnez sa valeur initiale.

  La condition est une expression booléenne qui est évaluée avant chaque itération de la boucle. Si la condition est vraie (`true`), la boucle continue. Une fois que la condition devient fausse (`false`), la boucle se termine.

  L'incrémentation/décrémentation est l'endroit où vous mettez à jour la variable de compteur et cela se produit à la fin de chaque itération.

  Le bloc de code à l'intérieur de la boucle est répété à chaque itération.

<br>

  #### Boucle while

  La boucle `while` est une autre façon de parcourir un tableau en JavaScript. Elle se compose d'une condition et d'un bloc de code qui est exécuté tant que la condition est `true` (vrai).

  Comme la boucle `for`, la boucle `while` nécessite une variable de compteur pour suivre la position actuelle dans le tableau. La variable de compteur doit être initialisée avant la boucle et incrémentée ou décrémentée à la fin de chaque itération.

  ```js
  const animals = ['cat', 'dog', 'bird'];

  // initialize a counter variable (i)
  let i = 0;

  // set condition (i < animals.length)
  while (i < animals.length) {
    console.log(animals[i]);
    
    // increment counter (i++)
    i++;
  }
  ```

  [Retour en haut](#faqs)

</details>

<details>
  <summary>Comment puis-je parcourir une boucle sur un tableau en utilisant la méthode <code>forEach()</code>?</summary>
  <br>

  La méthode `forEach()` exécute une fonction fournie une fois pour chaque élément du tableau. Elle ne renvoie pas un nouveau tableau, mais exécute plutôt la fonction sur chaque élément du tableau.

  La syntaxe de la méthode `forEach()` est la suivante:

  ```js
  array.forEach( function(element) {
    // code to be executed for each element
  });
  ```

  <br>

  Voici un exemple qui utilise la méthode `forEach()` pour enregistrer chaque élément et son index dans un tableau dans la console :

  ```js
  const fruits = ['apple', 'banana', 'cherry'];

  fruits.forEach( function(element, index) {
    console.log(`${index}: ${element}`);
  });
  ```

<br>

  Vous pouvez également utiliser une fonction fléchée en tant que fonction de rappel pour `forEach()` :

  ```js
  fruits.forEach((element, index) => {
    console.log(`${index}: ${element}`);
  });
  ```

  [Retour en haut](#faqs)

</details>

<details>
  <summary>Qu'est-ce qui pourrait faire en sorte que <code>array.length</code> renvoie <code>undefined</code> ?</summary>
  <br>

  Si vous essayez d'accéder à la propriété `.length` sur un tableau (par exemple, `array.length`) mais obtenez `undefined`, cela signifie que la variable à laquelle vous accédez n'est pas réellement un tableau.

  <br>

  **Comment puis-je réparer cela ?**

  Vérifiez que la variable que vous essayez d'accéder est effectivement un tableau.

  [Retour en haut](#faqs)

</details>

<details>
  <summary>Pourquoi ma fonction renvoie-t-elle le dernier élément du tableau au lieu du plus long ?</summary>
  <br>

  Votre fonction pourrait ne pas vérifier correctement le plus long élément du tableau. En d'autres termes, il peut y avoir un problème avec la logique des déclarations conditionnelles dans la fonction ou avec la comparaison utilisée dans les conditions.

  Pour résoudre ce problème, vous devriez vérifier la logique des déclarations conditionnelles dans la fonction.

  [Retour en haut](#faqs)

</details>

<details>
  <summary>Comment puis-je comparer la longueur de chaque mot dans un tableau en JavaScript ?</summary>
  <br>

  Pour comparer la longueur de chaque mot dans un tableau en JavaScript, vous pouvez utiliser une boucle pour parcourir le tableau et comparer la longueur de chaque élément à l'aide de la propriété `.length`.

  Voici un exemple de comment vous pouvez boucler sur un tableau :

  ```js
  function findLongestWord(words) {
    for (let i = 0; i < words.length; i++) {
      console.log(words[i]);
    }
  }
  ```

  <br>

  Pour comparer la longueur de chaque élément, vous devriez utiliser une déclaration conditionnelle de la manière suivante :

  ```js
    if ( words[i].length > longestWord.length) {
      console.log(`${words[i].length} is longer than ${longestWord.length}`);
    }
  ```

  [Retour en haut](#faqs)

</details>

<details>
  <summary>Je ne peux pas pousser les modifications vers le repo. Que dois-je faire ?</summary>
  <br>

Il existe quelques raisons possibles pour lesquelles vous pourriez ne pas être en mesure de *push* (pousser) des modifications vers un dépôt Git :

1. **Vous n'avez pas validé vos modifications** : Avant de pouvoir pousser vos modifications vers le dépôt, vous devez les valider en utilisant la commande `git commit`. Assurez-vous d'avoir validé vos modifications et essayez de pousser à nouveau. Pour ce faire, exécutez les commandes suivantes dans votre terminal à partir du dossier du projet :
  ```bash
  git add .
  git commit -m "Your commit message"
  git push
  ```
2. **Vous n'avez pas la permission de pousser vers le dépôt** : Si vous avez cloné le dépôt directement à partir du dépôt principal d'Ironhack sans effectuer un *Fork* au préalable, vous n'avez pas les droits d'écriture sur le dépôt.
Pour vérifier quel dépôt distant vous avez cloné, exécutez la commande suivante dans votre terminal à partir du dossier du projet :
  ```bash
  git remote -v
  ```
Si le lien affiché est le même que celui du dépôt principal d'Ironhack, vous devrez d'abord faire un Fork du dépôt vers votre compte GitHub, puis cloner votre Fork sur votre machine locale pour pouvoir pousser les modifications.

**Note** : Vous devriez faire une copie de votre code local pour éviter de le perdre lors du processus.

  [Retour en haut](#faqs)

</details>