<p align ="center">
      <img src="https://github.com/Hamza-Bchir/Projet-Bourse/assets/148462421/55eb5184-ed96-45e7-8403-970b6eb908ce" alt="Design sans titre" width="40%">
</p>
<h1 align="center">Projet-Bourse</h1>
<h1>Sujet</h1>

Projet de Simulation de la Bourse

Auteurs: Zaineb Zarrouk / Hamza B'chir

Date: 01/04/2024

<h1>Description</h1>
<h4>Objectif :</h4>
Le but du projet est de créer une mini-application dont le principale but est de visualier des données boursières accompagnés d'indicateurs et de quelques outils graphiques. L'utilisateur pourra donc s'inscrire, puis choisir les actions qu'il voudra visualiser a l'aide du moteur de recherche. Il pourra aussi utiliser des outils graphiques s'appuyant sur des indicateurs statistiques et mathématiques.
<h4>Motivation :</h4>
Nous nous retrouvons dans l'ère de la fintech, un secteur en plein essor qui combien avancées technologiques et services financiers pour améliorer l'efficacité, l'accessibilité et l'innovation dans le domaine financier. Ainsi ce projet nous permettra de mieux comprendre les implications pratiques de ce domaine en développant une application de visualisation des cours d'actions NASDAQ.

<h1>Spécifications du projet</h1>
<h4>Notions de Base et Contraintes du Projet:</h4>
<ul>
  <li>Données: L'application utilisera exclusivement des données historiques des cours d'actions du NASDAQ, couvrant la période des années 2000 aux années 2020.</li>
  <li>Indicateurs Techniques: Les indicateurs techniques disponibles seront limités à ceux standard utilisés dans l'analyse financière, tels que les moyennes mobiles, le RSI (Relative Strength Index), le MACD (Moving Average Convergence Divergence), etc.</li>
  <li>Interface Utilisateur: L'interface utilisateur sera conçue de manière intuitive pour permettre une navigation aisée et une utilisation fluide de toutes les fonctionnalités de l'application.</li>
</ul>

<h4>Acteurs et fonctionnalités attendues du projet</h4>
<ul>
  <li>Visualisation des Cours d'Actions: L'utilisateur pourra visualiser les cours d'actions du NASDAQ sur une période sélectionnée, avec la possibilité de zoomer et dézoomer pour explorer les données à différentes échelles de temps.
Sélection des Indicateurs: L'utilisateur pourra sélectionner et afficher différents indicateurs techniques.</li>
  <li>Recherche d'Actions: Une fonctionnalité de recherche permettra à l'utilisateur de rechercher des actions spécifiques par leur nom ou leur ticker symbol, facilitant ainsi l'accès aux données sur les actions souhaitées.</li>
  <li>Filtrage des Données: L'utilisateur pourra filtrer les données en fonction de critères tels que le volume des transactions, la variation des cours, etc., pour se concentrer sur les actions qui correspondent à ses critères d'investissement.</li>
</ul>
<h1>Cas d'utilisations</h1>
<img src="https://github.com/Hamza-Bchir/Projet-Bourse/assets/148462421/c2db27ee-55ad-47c0-bbff-c7a78137abd2">
<h2>Sprint n°1</h2>

Durant le premier sprint nous choisissons de travailler sur les trois cas d'utilisations : "S'inscrire", "Se connecter" et "Choisir action".

<h4>S'inscrire</h4>
<ul>
      <li>Préconditions :</li>
      Champ du nom d'utilisateur bien formé (¬ null ∧ ¬ vide ∧ unique) ∧ mot de passe (¬ null ∧ ¬ vide)
      <li>Postcondition :</li>
      Le compte existe
</ul>
<table align="center">
      <tr>
            <td colspan ="2"></td>
            <td>1</td>
            <td>2</td>
            <td>3</td>
            <td>4</td>
      </tr>
      <tr>
            <td rowspan ="2">Préconditions</td>
            <td>Champ du nom d'utilisateur bien formé</td>
            <td>F</td>
            <td>T</td>
            <td>F</td>
            <td>T</td>
      </tr>
      <tr>      
            <td>Mot de passe</td>
            <td>F</td>
            <td>F</td>
            <td>T</td>
            <td>T</td>
      </tr>
      <tr>
            <td>Postcondition</td>
            <td>Le compte existe</td>
            <td>F</td>
            <td>F</td>
            <td>F</td>
            <td>T</td>
      </tr>
      <tr>
            <td></td>
            <td>Nombre de jeux de tests</td>
            <td>1</td>
            <td>1</td>
            <td>1</td>
            <td>2</td>
      </tr>
</table>


<h4>Se connecter</h4>
<ul>
      <li>Préconditions :</li>
      Champ du nom d'utilisateur bien formé (¬ null ∧ ¬ vide) ∧ mot de passe (¬ null ∧ ¬ vide) ∧ champ du nom utilisateur correspond a celui enregistré ∧ champ du mot de passe correspond a celui enregistré
      <li>Postcondition :</li>
      L'utilisateur est connecté au système
</ul>
<table align="center">
      <tr>
            <td colspan ="2"></td>
            <td>1</td>
            <td>2</td>
            <td>3</td>
            <td>4</td>
            <td>5</td>
      </tr>
      <tr>
            <td rowspan ="4">Préconditions</td>
            <td>Champ du nom d'utilisateur bien formé</td>
            <td>F</td>
            <td>T</td>
            <td>T</td>
            <td>T</td>
            <td>T</td>
      </tr>
      <tr>      
            <td>Mot de passe</td>
            <td></td>
            <td>F</td>
            <td>T</td>
            <td>T</td>
            <td>T</td>
      </tr>
      <tr>
            <td>Nom d'utilisateur correspond à l'enregistrement</td>
            <td></td>
            <td></td>
            <td>F</td>
            <td>T</td>
            <td>T</td>
      </tr>
      <tr>
            <td>Mot de passe correspond à l'enregistrement</td>
            <td></td>
            <td></td>
            <td></td>
            <td>F</td>
            <td>T</td>
      </tr>
      <tr>
            <td>Postcondition</td>
            <td>L'utilisateur est connecté au système</td>
            <td>F</td>
            <td>F</td>
            <td>F</td>
            <td>F</td>
            <td>T</td>
      </tr>
      <tr>
            <td></td>
            <td>Nombre de jeux de tests</td>
            <td>1</td>
            <td>1</td>
            <td>1</td>
            <td>2</td>
            <td>2</td>
      </tr>
</table>

<h4>Choisir une action</h4>
<ul>
      <li>Préconditions :</li>
      L'utilisateur est connecté au système ∧ code mnémonique (¬ null ∧ ¬ vide) v nom de l'action (¬ null ∧ ¬ vide) ∧ l'action existe
      <li>Postcondition :</li>
      L'action s'affiche
</ul>
<table align="center">
      <tr>
            <td colspan ="2"></td>
            <td>1</td>
            <td>2</td>
            <td>3</td>
            <td>4</td>
      </tr>
      <tr>
            <td rowspan ="2">Préconditions</td>
            <td>Champ du nom d'utilisateur bien formé</td>
            <td>F</td>
            <td>T</td>
            <td>F</td>
            <td>T</td>
      </tr>
      <tr>      
            <td>Mot de passe</td>
            <td>F</td>
            <td>F</td>
            <td>T</td>
            <td>T</td>
      </tr>
      <tr>
            <td>Postcondition</td>
            <td>Le compte existe</td>
            <td>F</td>
            <td>F</td>
            <td>F</td>
            <td>T</td>
      </tr>
      <tr>
            <td></td>
            <td>Nombre de jeux de tests</td>
            <td>1</td>
            <td>1</td>
            <td>1</td>
            <td>2</td>
      </tr>
</table>
