# 🚀 Agence Digitale - Site Web Professionnel

Bienvenue! Ce site a été créé pour servir de base professionnelle et moderne à votre agence digitale.

---

## 📋 Contenu du Projet

```
site-belhaj-mohamed/
├── index.html          # Page d'accueil principale
├── .gitignore          # Fichiers à ignorer pour Git
└── README.md           # Ce fichier
```

---

## 🎯 Sections du Site

✅ **Navigation** - Menu fixe et responsive
✅ **Hero Section** - Accroche principale
✅ **Services** - 3 services principaux (à modifier)
✅ **Portfolio** - Showcase de projets
✅ **Contact** - Formulaire de contact
✅ **Footer** - Infos et liens de base

---

## ✏️ À MODIFIER DANS index.html

Voici les éléments à personnaliser avec **Ctrl+F** dans VS Code:

1. **Ligne ~25** - Logo/Nom d'entreprise
   ```html
   <div class="text-2xl font-bold text-blue-600">
       Belhaj Mohamed  <!-- À CHANGER -->
   </div>
   ```

2. **Ligne ~91** - Texte principal (Hero)
   ```html
   <h1>Transformez votre <span>présence digitale</span></h1>
   <p>Créons ensemble des solutions...</p>  <!-- À PERSONNALISER -->
   ```

3. **Ligne ~120-160** - Services
   ```html
   <h3>Sites Web Modernes</h3>
   <p>Créations modernes, responsive...</p>  <!-- À ADAPTER -->
   ```

4. **Ligne ~200-240** - Portfolio/Projets
   - Remplacez les exemples par vos propres projets

5. **Ligne ~270-310** - Formulaire Contact
   ```html
   <input type="email" placeholder="you@example.com" ...>
   <!-- À REMPLACER PAR VOTRE EMAIL -->
   ```

6. **Ligne ~365-390** - Footer
   ```html
   <h3>Belhaj Mohamed</h3>  <!-- À CHANGER -->
   <p>📧 contact@example.com</p>  <!-- À CHANGER -->
   <p>📱 +33 6 12 34 56 78</p>  <!-- À CHANGER -->
   ```

---

## 🔐 SÉCURITÉ - Points Importants

⚠️ **JAMAIS** mettre en dur dans le code:
- Clés API
- Mots de passe
- Tokens
- Informations sensibles

✅ **FAIRE:**
- Variables d'environnement (.env) - NE PAS POUSSER
- Services externes (Formspree, Web3Forms)
- Authentification backend sécurisée

---

## 📧 Formulaire de Contact - Configuration

Le formulaire doit être connecté à un service. **Voici 2 options gratuites:**

### Option 1: Formspree (Recommandé)

1. Allez sur https://formspree.io
2. Créez un compte (gratuit)
3. Créez un nouveau formulaire
4. Dans `index.html`, ligne ~290, remplacez:

```html
<!-- AVANT -->
<form class="bg-white rounded-xl p-8...">

<!-- APRÈS: Utilisez le code Formspree -->
<form action="https://formspree.io/f/VOTRE_FORM_ID" method="POST"
      class="bg-white rounded-xl p-8...">
```

5. Gardez exactement le même `name` pour les inputs:
```html
<input type="text" name="name" placeholder="Jean Dupont" required>
<input type="email" name="email" placeholder="you@example.com" required>
<textarea name="message" placeholder="..."></textarea>
```

### Option 2: Web3Forms

1. Allez sur https://web3forms.com
2. Créez un compte
3. Obtenez votre clé d'accès
4. Modifiez le formulaire de la même manière

---

## 🚀 ÉTAPE 1 - Initialiser Git Localement

Dans VS Code, ouvrez le terminal (Ctrl + J) et exécutez:

```bash
# Vérifier que vous êtes dans le bon dossier
pwd
# Devrait afficher: /Users/hachicha/Desktop/site belhaj mohamed

# Initialiser Git
git init

# Vérifier l'état
git status
```

**Résultat attendu:** Git est initialisé, tous les fichiers apparaissent en rouge (non tracked).

---

## 🐙 ÉTAPE 2 - Créer un Dépôt sur GitHub

1. Allez sur https://github.com/new
2. Remplissez les champs:
   - **Repository name:** `site-belhaj-mohamed` (ou votre choix)
   - **Description:** "Site web professionnel de mon agence digitale"
   - **Public** (pour GitHub Pages)
   - NE COCHEZ PAS "Add README" (vous l'avez déjà)

3. Cliquez **"Create repository"**

GitHub vous affichera ensuite les commandes à exécuter. **Suivez les étapes ci-dessous:**

---

## 📤 ÉTAPE 3 - Pousser le Code vers GitHub

Dans VS Code terminal, exécutez ces commandes **dans l'ordre**:

```bash
# 1. Ajouter tous les fichiers
git add .

# 2. Vérifier que c'est correct
git status
# Vous devez voir: index.html, .gitignore, README.md en vert

# 3. Créer le premier commit
git commit -m "Initialisation: site web professionnel"

# 4. Connecter au dépôt GitHub (remplacez USERNAME et REPO)
git remote add origin https://github.com/USERNAME/site-belhaj-mohamed.git

# 5. Pousser le code
git branch -M main
git push -u origin main
```

**Remplacez:**
- `USERNAME` par votre nom d'utilisateur GitHub
- `site-belhaj-mohamed` par le nom exact de votre dépôt

**Résultat:** Votre code est maintenant sur GitHub! ✅

---

## 🌐 ÉTAPE 4 - Activer GitHub Pages

1. Allez sur votre dépôt GitHub: https://github.com/USERNAME/site-belhaj-mohamed
2. Cliquez sur **Settings** (⚙️ en haut à droite)
3. Dans le menu de gauche, cliquez **Pages**
4. Sous "Source", sélectionnez **"main"** et cliquez **"Save"**

GitHub va générer votre URL: `https://USERNAME.github.io/site-belhaj-mohamed`

**Attendez 2-3 minutes** et visitez cette URL. Votre site sera en ligne! 🎉

---

## 🔗 ÉTAPE 5 - Lier Votre Domaine Personnalisé (Optionnel)

Si vous avez acheté un domaine (ex: `monagence.com`):

1. Chez votre registrar (GoDaddy, Namecheap, etc.):
   - Trouvez les paramètres DNS
   - Créez un enregistrement CNAME:
     ```
     CNAME → USERNAME.github.io
     ```

2. Dans GitHub Settings > Pages:
   - Remplissez "Custom domain" avec `monagence.com`
   - Cochez "Enforce HTTPS"
   - Cliquez "Save"

**Attendez 24h** pour que le DNS se propage. Ensuite `monagence.com` affichera votre site! 🚀

---

## 📝 Workflow Futur - Comment Mettre à Jour le Site

À chaque modification:

```bash
# 1. Modifiez vos fichiers dans VS Code
# (ex: index.html)

# 2. Terminal:
git add .
git commit -m "Description de la modification"
git push origin main

# 3. GitHub Pages se mettra à jour automatiquement en quelques secondes
```

---

## ✅ Checklist Sécurité

- ✅ Ne jamais mettre de clés API dans `index.html`
- ✅ Utiliser des services externes pour les formulaires
- ✅ `.gitignore` est en place
- ✅ Pas de fichiers sensibles poussés
- ✅ HTTPS activé sur GitHub Pages (par défaut)
- ✅ Repository en "Public" (nécessaire pour Pages)

---

## 🆘 En Cas de Problème

**"Git command not found"**
- Installez Git: https://git-scm.com/download/mac

**"GitHub Pages ne charge pas"**
- Attendez 2-3 minutes
- Vérifiez que la branche "main" est sélectionnée dans Settings > Pages
- Assurez-vous que le repo est public

**"Le formulaire ne marche pas"**
- Récupérez votre Form ID sur Formspree
- Vérifiez la ligne `action="..."` dans index.html

---

## 📚 Ressources Utiles

- Tailwind CSS Docs: https://tailwindcss.com/docs
- GitHub Pages: https://pages.github.com/
- Formspree: https://formspree.io/
- Web3Forms: https://web3forms.com/

---

## 🎬 Prochaines Étapes (Optionnel)

- Ajouter d'autres pages (À propos, Blog, etc.)
- Intégrer un CMS (GitHub-based ou autre)
- Ajouter analytics (Google Analytics)
- Optimiser le SEO
- Ajouter une newsletter

---

**Créé avec ❤️ par Claude**

Bonne chance pour votre agence digitale! 🚀

