# TP02-PHP-HAJJOUCHI-TAHA
TP 02 PHP — Programmation Web 2 — 2026/2027
Taha HAJJOUCHI
Le groupe: G01

# Les 10 exercices

## Consigne commune

* Utiliser la balise `<?php`.
* Choisir des noms de variables explicites.
* Ajouter des commentaires utiles.
* Utiliser un affichage HTML lisible.
* Tester chaque exercice avant de le publier.
* Après chaque exercice terminé, réaliser un commit distinct et un push en suivant la procédure de la partie C.

## Exercice 1 — Balises, HTML/PHP, commentaires et echo

**Fichier :** `ex01.php`

1. Créer une page HTML avec un titre et l'encodage UTF-8.
2. Afficher avec PHP : « Bienvenue dans mon TP PHP ».
3. Afficher un nom et un prénom fictifs ainsi que votre groupe.
4. Ajouter un commentaire sur une ligne et un commentaire sur plusieurs lignes.
5. Afficher une dernière phrase avec la syntaxe courte `<?= ... ?>`.

**Vérification :**

* Les informations apparaissent sur des lignes distinctes.
* Les commentaires ne sont pas affichés.

## Exercice 2 — Variables, casse, concaténation et opérateur .=

**Fichier :** `ex02.php`

1. Déclarer `$nom`, `$prenom`, `$age` et `$formation` avec des données fictives.
2. Construire une phrase de présentation en utilisant la concaténation `.`.
3. Compléter cette phrase avec `.=` pour ajouter « J'apprends PHP ».
4. Déclarer `$note = 12` et `$Note = 16`, puis afficher les deux valeurs.
5. Dans le README, expliquer pourquoi ces deux variables sont différentes.
6. Identifier les noms de variables valides parmi `$a`, `$_a`, `$a_a`, `$AAA`, `$a!`, `$1a` et `$a1`.

**Vérification :**

* Les deux notes sont distinctes.
* Ne pas insérer les noms de variables invalides dans du code exécuté.

## Exercice 3 — Constantes, calculs et affectation composée

**Fichier :** `ex03.php`

1. Définir la constante `TAUX_TVA` à 20.
2. Définir la constante `DEVISE` à `"MAD"`.
3. Déclarer un prix unitaire HT de 60 et une quantité de 3.
4. Calculer le total HT, le montant de TVA et le total TTC.
5. Ajouter 15 MAD de frais de livraison au total TTC avec `+=`.
6. Afficher un récapitulatif HTML.
7. Vérifier l'existence de `TAUX_TVA` avec `defined()`.

**Vérification :**

* Total HT : 180 MAD.
* TVA : 36 MAD.
* Total TTC : 216 MAD.
* Montant final : 231 MAD.
* Le taux est une donnée de l'exercice.

## Exercice 4 — Types de données et conversions

**Fichier :** `ex04.php`

1. Déclarer six variables contenant respectivement `42`, `"42"`, `15.8`, `true`, `false` et `null`.
2. Examiner leurs types et leurs valeurs avec `var_dump()` dans une balise HTML `<pre>`.
3. Convertir `"42"` en entier.
4. Convertir `15.8` en entier.
5. Convertir `42` en chaîne de caractères.
6. Afficher les résultats des conversions avec leurs types.
7. Afficher `true` et `false` avec `echo`, puis avec `var_dump()`.
8. Convertir `0`, `"0"`, `"PHP"` et un tableau vide en booléens.
9. Expliquer dans le README la différence d'affichage de `false` entre `echo` et `var_dump()`.

**Vérification :**

* La conversion de `15.8` en entier donne `15`.
* Chaque conversion est identifiable dans la page.

## Exercice 5 — Conditions if, elseif, else et comparaisons

**Fichier :** `ex05.php`

1. Déclarer une variable `$moyenne`.
2. Vérifier que sa valeur est comprise entre 0 et 20.
3. Si la note est invalide, afficher « Note invalide ».
4. Pour une note valide, afficher la mention correspondante selon les règles suivantes :

| Moyenne                 | Message    |
| ----------------------- | ---------- |
| Inférieure à 10         | Non validé |
| De 10 inclus à 12 exclu | Passable   |
| De 12 inclus à 14 exclu | Assez bien |
| De 14 inclus à 16 exclu | Bien       |
| De 16 à 20 inclus       | Très bien  |

5. Tester successivement les valeurs `-1`, `9`, `10`, `12`, `14`, `16` et `21` en changeant la variable.
6. Consigner dans le README les valeurs testées et les messages obtenus.

**Vérification :**

* Les valeurs limites sont correctement traitées.
* Une note invalide ne reçoit pas de mention.

## Exercice 6 — switch, case, break, default et date()

**Fichier :** `ex06.php`

1. Déclarer `$numeroMois = 3`.
2. Utiliser `switch` pour afficher le nom français correspondant aux nombres de 1 à 12.
3. Prévoir un cas `default` affichant « Numéro de mois invalide ».
4. Tester les valeurs `1`, `3`, `12` et `15`.
5. Remplacer ensuite la valeur fixe par `(int) date("m")` pour afficher le mois courant du serveur.

**Vérification :**

* La valeur `3` donne « Mars ».
* La valeur `12` donne « Décembre ».
* La valeur `15` donne le message d'erreur.

## Exercice 7 — Boucles for et boucles imbriquées

**Fichier :** `ex07.php`

1. Déclarer `$nombre = 7`.
2. Afficher la table de multiplication de 7, de 1 à 10.
3. Utiliser deux boucles `for` imbriquées pour produire une pyramide de six lignes.
4. La pyramide doit comporter respectivement 1, 2, 3, 4, 5 et 6 étoiles.
5. Présenter les deux résultats dans deux sections HTML distinctes.

**Vérification :**

* La table se termine par `7 × 10 = 70`.
* La pyramide comporte exactement six lignes.
* Utiliser `<br>` ou `<pre>` pour conserver les retours à la ligne dans le navigateur.

## Exercice 8 — Boucles et contrôle des itérations

**Fichier :** `ex08.php`

### Partie 1 — Boucle while

1. Utiliser `while` pour afficher les nombres pairs de 0 à 20 inclus.
2. Mettre uniquement le nombre `10` en gras.

### Partie 2 — Comparaison de while et do-while

3. Initialiser un compteur à 5.
4. Utiliser la condition « compteur inférieur à 5 ».
5. Comparer une boucle `while` et une boucle `do-while`.
6. Réinitialiser le compteur avant chaque boucle.
7. Compter et afficher le nombre d'exécutions du corps de chaque boucle.

### Partie 3 — Utilisation de continue et break

8. Parcourir les entiers de 1 à 20.
9. Utiliser `continue` pour ignorer les multiples de 3.
10. Utiliser `break` pour arrêter la boucle dès que le compteur atteint 16, avant son affichage.

**Vérification :**

* La boucle `while` réalise 0 exécution dans la partie 2.
* La boucle `do-while` réalise 1 exécution dans la partie 2.
* Dans la partie 3, aucun multiple de 3 n'est affiché.
* Les valeurs supérieures ou égales à 16 ne sont pas affichées.

## Exercice 9 — Tableaux associatifs, foreach et calculs

**Fichier :** `ex09.php`

Utiliser le jeu de données fictives suivant :

```php
$notes = [
    "Amine" => 12,
    "Sara" => 16,
    "Youssef" => 8,
    "Lina" => 14,
    "Adam" => 10
];
```

1. Afficher les étudiants et leurs notes dans un tableau HTML avec `foreach`.
2. Ajouter une colonne « Validé » ou « Non validé », avec un seuil de 10.
3. Calculer la somme des notes.
4. Calculer la moyenne de la classe.
5. Compter les étudiants ayant validé.
6. Déterminer la meilleure note et le nom de l'étudiant correspondant en parcourant le tableau.

**Vérification :**

* Moyenne : 12.
* Nombre d'étudiants ayant validé : 4.
* Meilleure note : 16.
* Étudiante ayant obtenu la meilleure note : Sara.

## Exercice 10 — Formulaires HTML et traitement PHP avec GET et POST

**Fichiers :**

* `ex10_get.html`
* `ex10_get.php`
* `ex10_post.html`
* `ex10_post.php`

### Partie A — Méthode GET

1. Créer un formulaire avec les champs `nom` et `prenom`.
2. Ajouter un menu `groupe` proposant les choix G1, G2, G3 et G4.
3. Envoyer les données à `ex10_get.php` avec la méthode `GET`.
4. Récupérer les données avec `$_GET`.
5. Afficher un message de bienvenue contenant les trois informations.
6. Observer l'URL après l'envoi.
7. Expliquer dans le README où apparaissent les valeurs transmises.

### Partie B — Méthode POST

8. Créer un second formulaire avec les mêmes champs.
9. Envoyer les données à `ex10_post.php` avec la méthode `POST`.
10. Récupérer les données avec `$_POST`.
11. Afficher le même message de bienvenue.
12. Comparer l'URL obtenue avec celle de la partie GET.

### Partie C — Vérifications et sécurité

13. Vérifier côté PHP la présence des trois champs.
14. Refuser les valeurs vides.
15. Ouvrir directement les deux pages de traitement sans soumettre de formulaire.
16. Afficher un message explicatif sans avertissement « Undefined array key ».
17. Tester un formulaire complet.
18. Tester un formulaire incomplet.
19. Avant d'afficher une donnée saisie dans la page HTML, l'échapper avec `htmlspecialchars()`.

Aides : isset() vérifie la présence d'une clé ; trim() permet de repérer une chaîne composée seulement d'espaces ; htmlspecialchars($valeur, ENT_QUOTES, 'UTF-8') protège l'affichage HTML. Utiliser des noms de champs identiques dans le formulaire et dans le traitement. 

Vérification : les deux méthodes fonctionnent ; les champs vides sont signalés ; les pages de traitement restent lisibles lorsqu'elles sont ouvertes directement. 
