### Comment cloner un repository GitHub en local, modifier des fichiers, pousser les changements et récupérer les mises à jour depuis GitHub

Voici une explication **très simple et détaillée**, étape par étape, pour des débutants. Imagine que tu veux copier un dossier en ligne sur ton ordinateur, le modifier, puis renvoyer tes changements sur Internet. C'est exactement ce que nous allons faire.

---

#### **Pré-requis**

Avant de commencer, tu as besoin de :

1. **Git** installé sur ton ordinateur.  
   👉 [Télécharge Git ici](https://git-scm.com/downloads) et installe-le.
2. Un compte GitHub et les accès au repository (si demandé).
3. Ton terminal ou un outil comme Git Bash ouvert (par exemple, sur Windows, cherche "Git Bash").
4. Un éditeur de texte comme **VS Code** pour modifier les fichiers.

---

#### **Étape 1 : Cloner le repository en local**

1. Ouvre ton terminal.
2. Copie ce lien : `https://github.com/MoiseAganze/ex_gg.git`.
3. Ouvre le terminal dans un repertoire où tu veux mettre le projet.
4. Tape cette commande dans le terminal pour **copier le repository sur ton ordinateur** :
   ```bash
   git clone https://github.com/MoiseAganze/ex_gg.git
   ```
5. Tu verras un dossier nommé `ex_gg` apparaître sur ton ordinateur (dans le même répertoire où tu as exécuté la commande).

---

#### **Étape 2 : Naviguer dans le dossier cloné**

1. Dans le terminal, entre dans le dossier que tu viens de cloner :
   ```bash
   cd ex_gg
   ```

---

#### **Étape 3 : Modifier les fichiers**

1. Ouvre le dossier `ex_gg` avec ton éditeur de texte (par exemple, VS Code) ou directement depuis ton explorateur de fichiers.
2. Fais les modifications nécessaires dans les fichiers que tu veux.
3. Dans le cas de vos exercices, par exemple si tu apprends les bases du js, tu entre dans le dossier "bases_js" tu verras
   il y a un fichier pour le cours et un fichier pour les exercices, tu peux juste les lire mais n'y ecris rien,
   ensuite apres avoir lu le cours, tu entre dans les fichiers pour les exercices,
   et tu mets ta resolution dans un fichiers que tu vas créé,ce fichier que tu vas créé doit contenir ton prenom,
   par exemple "patrick_bases_js.js",tu peux modifier ce fichier pour resoudre les exercices, faire des testes,
   executer.... Et quand tu as finis avec les exercices.....

---

#### **Étape 4 : Préparer et pousser les modifications sur GitHub**

1. Une fois les modifications terminées, retourne dans le terminal et **vérifie l’état des fichiers modifiés** :

   ```bash
   git status
   ```

   👉 Cette commande montre quels fichiers ont été modifiés.

2. **Ajouter les fichiers modifiés** pour dire à Git qu'ils doivent être pris en compte :

   ```bash
   git add .
   ```

   ⚠️ Le `.` signifie "ajoute tous les fichiers modifiés".

3. **Enregistrer les modifications localement** avec un message clair :

   ```bash
   git commit -m "Description des modifications"
   ```

   Exemple :

   ```bash
   git commit -m "Ajout d'une nouvelle fonction dans le fichier X"
   ```

4. **Pousser les modifications sur la branche principale (par défaut appelée 'main')** :
   ```bash
   git push origin main
   ```
   👉 Cette commande renvoie les changements que tu as faits vers le repository sur GitHub.

---

#### **Étape 5 : Récupérer les dernières modifications**

Si quelqu’un d’autre a modifié le repository sur GitHub entre-temps,par exemple si j'ai ajouté des cours
voici comment **mettre à jour ton dossier local** :

1. Tape cette commande dans le terminal :
   ```bash
   git pull origin main
   ```
   👉 Cela met à jour ton dossier local avec les dernières modifications depuis GitHub.

---

### **Ce que tout cela implique**

1. **Cloner** : Tu copies le dossier et tout son contenu depuis Internet sur ton ordinateur.
2. **Modifier** : Tu peux travailler sur les fichiers de ton côté.
3. **Pousser (push)** : Cela envoie tes modifications sur GitHub pour que tout le monde puisse les voir ou travailler dessus.
4. **Récupérer (pull)** : Cela te permet de t’assurer que tu as les dernières modifications faites par d’autres avant de continuer.

---
