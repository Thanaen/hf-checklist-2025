# 🎪 Festival Check-List 2025

Une application web moderne pour organiser parfaitement votre festival ! Cette check-list interactive vous aide à ne rien oublier pour votre prochaine aventure musicale.

## ✨ Fonctionnalités

- **Interface moderne** : Design sombre avec thème rouge élégant
- **Persistance locale** : Vos cases cochées sont sauvegardées automatiquement
- **Responsive** : Fonctionne parfaitement sur mobile, tablette et desktop
- **Catégories organisées** : 7 catégories essentielles avec icônes Lucide
- **Performance optimale** : Construit avec Astro pour un chargement ultra-rapide
- **Thème personnalisé** : Palette de couleurs soigneusement choisie

## 🎨 Thème et couleurs

Le projet utilise une palette de couleurs soigneusement choisie :

- **Couleur principale** : `#b5252a` (rouge) - Titres et éléments actifs
- **Arrière-plan** : `#1d1d1b` (noir profond) - Arrière-plan principal
- **Textes secondaires** : `#f5efef` (blanc cassé) - Textes de contenu
- **Cartes** : `#2a2a28` (gris foncé) - Arrière-plan des catégories

Ces couleurs offrent un excellent contraste et une lisibilité optimale tout en conservant une esthétique moderne et professionnelle.

## 🏗️ Technologies utilisées

- **[Astro](https://astro.build/)** - Framework web moderne
- **[Tailwind CSS v4](https://tailwindcss.com/)** - Framework CSS utility-first avec thème CSS
- **[Lucide Icons](https://lucide.dev/)** - Icônes SVG modernes et élégantes
- **[TypeScript](https://www.typescriptlang.org/)** - Typage statique
- **[Biome](https://biomejs.dev/)** - Linter et formatter
- **[Bun](https://bun.sh/)** - Runtime et gestionnaire de paquets rapide
- **Google Fonts** - Polices Inter et Orbitron

## ⚙️ Configuration Tailwind v4

Le projet utilise la nouvelle approche de configuration Tailwind CSS v4 avec des thèmes CSS. Au lieu d'un fichier `tailwind.config.js`, le thème est défini directement dans le CSS avec la directive `@theme` :

```css
@theme {
  /* Couleurs personnalisées */
  --color-primary: #b5252a;
  --color-primary-dark: #9a1f23;
  --color-primary-light: #c7484d;
  
  --color-background: #1d1d1b;
  --color-background-card: #2a2a28;
  
  --color-secondary: #f5efef;
  --color-secondary-muted: #e0d5d5;
  
  /* Polices personnalisées */
  --font-sans: "Inter", sans-serif;
  --font-display: "Orbitron", sans-serif;
}
```

Cette approche offre plusieurs avantages :
- **Performance** : Variables CSS natives, plus rapides
- **Flexibilité** : Possibilité de modifier les valeurs dynamiquement
- **Simplicité** : Pas de configuration JavaScript séparée
- **Modern** : Utilise les dernières fonctionnalités CSS

## 🚀 Installation et développement

### Prérequis
- bun

### Installation
```bash
# Cloner le projet
git clone <url-du-repo>
cd hf-checklist-2025

# Installer les dépendances
bun install
# ou
npm install
```

### Développement
```bash
# Lancer le serveur de développement
bun run dev
```

Le site sera accessible sur `http://localhost:4321`

### Build de production
```bash
# Construire pour la production
bun run build

# Prévisualiser la build
bun run preview
```

## 📁 Structure du projet

```
src/
├── components/
│   ├── ChecklistCategory.astro  # Composant catégorie
│   └── Icon.astro       # Gestionnaire d'icônes Lucide
├── data/
│   └── checklist.json   # Données de la checklist
├── pages/
│   └── index.astro      # Page principale
├── scripts/
│   └── checklist.js     # Logique de persistance
└── styles/
    └── global.css       # Styles globaux
```

## 🎯 Catégories incluses

1. **🏕️ Camping** - Matériel de camping et équipements
2. **👕 Vêtements** - Tenues pour tous les temps
3. **✨ Hygiène** - Produits d'hygiène et soins
4. **🚗 Trajet** - Organisation du voyage
5. **🏥 Santé** - Matériel médical et de protection
6. **🎫 Concert** - Préparation pour les shows
7. **💰 Budget** - Planification financière

## 🔧 Personnalisation

### Modifier les données
Éditez le fichier `src/data/checklist.json` pour :
- Ajouter/supprimer des catégories
- Modifier les éléments des listes
- Changer les icônes associées

### Ajouter de nouvelles icônes
1. Consultez la [documentation Lucide](https://lucide.dev/icons/) pour trouver l'icône souhaitée
2. Importez l'icône dans `src/components/Icon.astro`
3. Ajoutez-la dans le mapping `iconComponents`
4. Utilisez le nom dans vos données JSON

### Modifier les styles
Les styles principaux se trouvent dans `src/styles/global.css` et utilisent les classes Tailwind CSS.

## 📝 License

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- Ouvrir une issue pour signaler un bug
- Proposer de nouvelles fonctionnalités  
- Soumettre une pull request

---

**Bon festival ! 🎉🎵**
