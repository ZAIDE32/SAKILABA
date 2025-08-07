# Cinéma Mali Production

Un site web moderne et élégant pour promouvoir l'excellence cinématographique malienne.

## 🌟 À propos

Ce projet présente une société de production cinématographique malienne, spécialisée dans la création de films d'auteur et la promotion du cinéma africain. Le site met en valeur les réalisateurs maliens, leurs œuvres et les récompenses obtenues sur la scène internationale.

## 🎬 Fonctionnalités

### Pages principales
- **Accueil** : Section hero avec vidéo, présentation de la mission
- **À propos** : Histoire et mission de la société
- **Films** : Catalogue des productions
- **Réalisateurs** : Profils des cinéastes maliens
- **Hommage** : Tribute aux grands réalisateurs
- **Prix** : Récompenses et distinctions
- **Projets** : Productions en cours
- **Galerie** : Photos et vidéos
- **Blog** : Actualités du cinéma malien
- **Investisseurs** : Opportunités d'investissement
- **Contact** : Formulaire de contact

### Fonctionnalités techniques
- ✅ Design responsive (mobile-first)
- ✅ Animations fluides et modernes
- ✅ Navigation sticky avec effet de transparence
- ✅ Carousel interactif pour les films
- ✅ Modal vidéo pour les bandes-annonces
- ✅ Lazy loading des images
- ✅ Formulaire de contact avec validation
- ✅ Effets parallax
- ✅ Optimisation des performances
- ✅ Accessibilité améliorée

## 🛠️ Technologies utilisées

- **HTML5** : Structure sémantique
- **CSS3** : Styles modernes avec Grid et Flexbox
- **JavaScript ES6+** : Interactions et animations
- **Font Awesome** : Icônes
- **Google Fonts** : Typographie (Montserrat, Open Sans)

## 📁 Structure du projet

```
cinema-mali-production/
├── index.html              # Page d'accueil
├── assets/
│   ├── css/
│   │   └── style.css      # Styles principaux
│   ├── js/
│   │   └── main.js        # JavaScript principal
│   ├── images/
│   │   ├── logo/          # Logos et branding
│   │   ├── films/         # Affiches de films
│   │   ├── directors/     # Photos de réalisateurs
│   │   ├── blog/          # Images d'actualités
│   │   └── partners/      # Logos des partenaires
│   └── videos/
│       └── hero-cinema.mp4 # Vidéo d'arrière-plan
├── films/                 # Pages des films
├── directors/             # Pages des réalisateurs
├── gallery/               # Galerie photos
├── blog/                  # Articles d'actualités
└── README.md             # Documentation
```

## 🚀 Installation et utilisation

### Prérequis
- Navigateur web moderne (Chrome, Firefox, Safari, Edge)
- Serveur web local (optionnel pour le développement)

### Installation
1. Clonez le repository :
```bash
git clone https://github.com/votre-username/cinema-mali-production.git
cd cinema-mali-production
```

2. Ouvrez le fichier `index.html` dans votre navigateur

### Développement local
Pour un serveur de développement local :

```bash
# Avec Python
python -m http.server 8000

# Avec Node.js (si vous avez http-server installé)
npx http-server

# Avec PHP
php -S localhost:8000
```

Puis ouvrez `http://localhost:8000` dans votre navigateur.

## 🎨 Design et UX

### Palette de couleurs
- **Rouge principal** : `#e74c3c` (Cinéma, passion)
- **Rouge foncé** : `#c0392b` (Hover states)
- **Gris foncé** : `#2c3e50` (Footer)
- **Gris clair** : `#f8f9fa` (Sections alternées)
- **Blanc** : `#fff` (Contenu principal)

### Typographie
- **Titres** : Montserrat (700, 600)
- **Corps de texte** : Open Sans (400, 300)

### Responsive Design
- **Desktop** : 1200px+
- **Tablet** : 768px - 1199px
- **Mobile** : < 768px

## 📱 Compatibilité

### Navigateurs supportés
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Fonctionnalités modernes
- CSS Grid et Flexbox
- Animations CSS
- Intersection Observer API
- Local Storage
- Service Workers (préparé)

## 🔧 Personnalisation

### Modifier les couleurs
Éditez les variables CSS dans `assets/css/style.css` :

```css
:root {
    --primary-color: #e74c3c;
    --secondary-color: #c0392b;
    --dark-color: #2c3e50;
    --light-color: #f8f9fa;
}
```

### Ajouter du contenu
1. **Nouveau film** : Ajoutez une entrée dans la section "Films en vedette"
2. **Nouvelle actualité** : Créez un article dans la section "Actualités"
3. **Nouveau réalisateur** : Ajoutez un profil dans la section "Hommage"

### Modifier les animations
Les animations sont définies dans `assets/css/style.css` avec les keyframes :
- `fadeInUp` : Apparition des éléments
- `bounce` : Indicateur de scroll

## 📊 Performance

### Optimisations incluses
- Images optimisées et lazy loading
- CSS et JS minifiés
- Préchargement des ressources critiques
- Compression des assets
- Cache des ressources statiques

### Métriques cibles
- **First Contentful Paint** : < 1.5s
- **Largest Contentful Paint** : < 2.5s
- **Cumulative Layout Shift** : < 0.1

## 🔒 Sécurité

- Validation côté client et serveur
- Protection XSS dans les formulaires
- Headers de sécurité recommandés
- HTTPS obligatoire en production

## 📈 SEO

### Optimisations incluses
- Meta tags complets
- Structure HTML sémantique
- Schema.org markup
- Sitemap XML
- Robots.txt
- Open Graph tags
- Twitter Cards

### Mots-clés cibles
- Cinéma malien
- Production cinématographique
- Réalisateurs maliens
- Films africains
- Cinéma d'auteur

## 🤝 Contribution

Les contributions sont les bienvenues ! Voici comment contribuer :

1. Fork le projet
2. Créez une branche feature (`git checkout -b feature/AmazingFeature`)
3. Committez vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrez une Pull Request

### Guidelines
- Respectez les conventions de nommage
- Testez sur différents navigateurs
- Optimisez les performances
- Documentez les nouvelles fonctionnalités

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## 👥 Équipe

- **Design** : [Votre nom]
- **Développement** : [Votre nom]
- **Contenu** : Équipe Cinéma Mali Production

## 📞 Contact

- **Email** : contact@cinemamali.ml
- **Téléphone** : +223 XX XX XX XX
- **Adresse** : Bamako, Mali

## 🙏 Remerciements

- Souleymane Cissé pour son inspiration
- L'équipe de développement
- La communauté du cinéma malien
- Tous les partenaires et investisseurs

---

**Cinéma Mali Production** - Excellence cinématographique malienne depuis 1980 