# Guide de Configuration GitHub Pages

Ce guide vous explique comment déployer votre site Cinéma Mali Production sur GitHub Pages.

## 📋 Prérequis

1. **Compte GitHub** : Créez un compte sur [GitHub.com](https://github.com)
2. **Git installé** : Téléchargez et installez Git depuis [git-scm.com](https://git-scm.com)
3. **Éditeur de code** : VS Code, Sublime Text, ou autre

## 🚀 Étapes de déploiement

### 1. Créer un nouveau repository

1. Allez sur [GitHub.com](https://github.com)
2. Cliquez sur le bouton "+" en haut à droite
3. Sélectionnez "New repository"
4. Nommez-le `cinema-mali-production`
5. Laissez-le public
6. **Ne cochez PAS** "Initialize this repository with a README"
7. Cliquez sur "Create repository"

### 2. Initialiser Git localement

Ouvrez votre terminal/command prompt et naviguez vers votre dossier de projet :

```bash
cd chemin/vers/cinema-mali-production
git init
git add .
git commit -m "Initial commit: Site Cinéma Mali Production"
```

### 3. Connecter au repository GitHub

```bash
git remote add origin https://github.com/VOTRE_USERNAME/cinema-mali-production.git
git branch -M main
git push -u origin main
```

**Remplacez `VOTRE_USERNAME` par votre nom d'utilisateur GitHub.**

### 4. Activer GitHub Pages

1. Allez sur votre repository GitHub
2. Cliquez sur "Settings" (onglet)
3. Dans le menu de gauche, cliquez sur "Pages"
4. Dans "Source", sélectionnez "Deploy from a branch"
5. Dans "Branch", sélectionnez "main" et "/ (root)"
6. Cliquez sur "Save"

### 5. Configurer le domaine personnalisé (optionnel)

Si vous avez un nom de domaine :

1. Dans les paramètres Pages, ajoutez votre domaine
2. Créez un fichier `CNAME` à la racine du projet avec votre domaine
3. Configurez les DNS de votre domaine

## 🔧 Configuration avancée

### Workflow GitHub Actions

Le projet inclut déjà des workflows GitHub Actions pour le déploiement automatique. Ils se trouvent dans `.github/workflows/`.

### Variables d'environnement

Si nécessaire, configurez des variables d'environnement dans Settings > Secrets and variables > Actions.

## 📱 Test local

Avant de déployer, testez votre site localement :

```bash
# Avec Python
python -m http.server 8000

# Avec Node.js
npx http-server

# Avec PHP
php -S localhost:8000
```

Puis ouvrez `http://localhost:8000` dans votre navigateur.

## 🔄 Mise à jour du site

Pour mettre à jour votre site :

```bash
git add .
git commit -m "Mise à jour du site"
git push origin main
```

GitHub Pages se mettra à jour automatiquement.

## 🐛 Dépannage

### Problèmes courants

1. **Site ne se charge pas** :
   - Vérifiez que GitHub Pages est activé
   - Attendez quelques minutes pour le déploiement
   - Vérifiez les logs dans l'onglet Actions

2. **Images ne s'affichent pas** :
   - Vérifiez les chemins des images
   - Assurez-vous que les images sont dans le repository

3. **CSS/JS ne fonctionne pas** :
   - Vérifiez les chemins dans les fichiers HTML
   - Assurez-vous que les fichiers sont dans le repository

### Logs de déploiement

1. Allez dans l'onglet "Actions" de votre repository
2. Cliquez sur le workflow "Deploy Static Site"
3. Vérifiez les logs pour identifier les erreurs

## 📊 Analytics et monitoring

### Google Analytics

Ajoutez votre ID Google Analytics dans le fichier `index.html` :

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Google Search Console

1. Allez sur [Google Search Console](https://search.google.com/search-console)
2. Ajoutez votre propriété
3. Vérifiez la propriété via le fichier HTML ou DNS
4. Soumettez votre sitemap

## 🔒 Sécurité

### HTTPS

GitHub Pages fournit automatiquement HTTPS. Assurez-vous que tous vos liens utilisent HTTPS.

### Headers de sécurité

Le fichier `netlify.toml` inclut des headers de sécurité. Pour GitHub Pages, ajoutez-les dans votre HTML :

```html
<meta http-equiv="X-Frame-Options" content="DENY">
<meta http-equiv="X-XSS-Protection" content="1; mode=block">
<meta http-equiv="X-Content-Type-Options" content="nosniff">
```

## 📈 Performance

### Optimisations incluses

- Images optimisées
- CSS et JS minifiés
- Lazy loading
- Cache des ressources statiques

### Tests de performance

Utilisez ces outils pour tester votre site :

- [Google PageSpeed Insights](https://pagespeed.web.dev/)
- [GTmetrix](https://gtmetrix.com/)
- [WebPageTest](https://www.webpagetest.org/)

## 🌐 Domaines personnalisés

### Configuration DNS

Si vous utilisez un domaine personnalisé :

1. **A Record** : Point vers `185.199.108.153`
2. **CNAME** : Point vers `votre-username.github.io`

### Certificat SSL

GitHub Pages fournit automatiquement un certificat SSL pour les domaines personnalisés.

## 📞 Support

Si vous rencontrez des problèmes :

1. Consultez la [documentation GitHub Pages](https://docs.github.com/en/pages)
2. Vérifiez les [forums GitHub](https://github.community/)
3. Ouvrez une issue dans votre repository

## 🎉 Félicitations !

Votre site Cinéma Mali Production est maintenant en ligne ! 

**URL de votre site** : `https://votre-username.github.io/cinema-mali-production`

N'oubliez pas de :
- Tester toutes les pages
- Vérifier les liens
- Optimiser les images
- Configurer les analytics
- Partager votre site !

---

**Cinéma Mali Production** - Excellence cinématographique malienne depuis 1980 