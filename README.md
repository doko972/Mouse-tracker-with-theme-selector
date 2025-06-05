# 👻 Ghost Mouse Tracker

Un mouse-tracker interactif avec des effets visuels magiques et plusieurs thèmes saisonniers.

## ✨ Fonctionnalités

### 🎮 Interaction
- **Suivi de souris fluide** : Un personnage suit votre curseur en temps réel
- **Traînée estompée** : 8 copies du personnage suivent avec opacité décroissante
- **Animation de flottement** : Mouvement organique et naturel
- **Particules magiques** : Effets visuels qui tourbillonnent autour du curseur

### 🎨 Thèmes Disponibles
1. **👻 Fantôme** (par défaut)
   - Fantôme blanc classique
   - Fond bleu nuit mystérieux
   - Particules blanches scintillantes

2. **🎃 Halloween**
   - Citrouille orange effrayante
   - Fond violet mystique
   - Yeux et bouche agrandis

3. **🎄 Noël**
   - Sapin vert en forme d'étoile
   - Fond bleu hivernal
   - **Effet de neige animée** qui tombe en continu

### 🛠️ Caractéristiques Techniques
- **Pure Vanilla JS** : Aucune dépendance externe
- **SVG personnalisés** : Graphiques vectoriels optimisés
- **Animations CSS** : Performances optimales avec GPU
- **RequestAnimationFrame** : Animation fluide 60fps
- **Responsive** : S'adapte à toutes les tailles d'écran

## 🚀 Installation et Utilisation

### Installation Simple
1. Clonez le repository :
```bash
git clone https://github.com/votre-username/ghost-mouse-tracker.git
cd ghost-mouse-tracker
```

2. Ouvrez `index.html` dans votre navigateur

### Intégration dans un Projet
Copiez simplement le fichier HTML complet ou intégrez les parties CSS/JS dans votre projet existant.

## 🎯 Structure du Code

```
ghost-mouse-tracker/
├── index.html          # Fichier principal (tout-en-un)
├── README.md           # Documentation

```

### Architecture du Code
- **HTML** : Structure SVG modulaire avec sélecteur de thèmes
- **CSS** : Animations keyframes, thèmes et effets visuels
- **JavaScript** : Logique de suivi, gestion des thèmes et animations

## 🔧 Personnalisation

### Ajouter un Nouveau Thème
1. **CSS** : Ajoutez les styles de fond et bouton
```css
body.theme-monnouvealtheme {
    background: linear-gradient(135deg, #couleur1, #couleur2);
}

.theme-button.btn-monnouvealtheme {
    background: linear-gradient(135deg, #couleur1, #couleur2);
}
```

2. **HTML** : Ajoutez le bouton de sélection
```html
<div class="theme-button btn-monnouvealtheme" data-theme="monnouvealtheme" title="Mon Thème"></div>
```

3. **JavaScript** : Définissez les propriétés du thème
```javascript
const themes = {
    monnouvealtheme: {
        shape: 'M50 20 L...',
        fill: 'rgba(r, g, b, 0.9)',
        eye1: { cx: 40, cy: 40, r: 4 },
        eye2: { cx: 60, cy: 40, r: 4 },
        mouth: { cx: 50, cy: 55, rx: 8, ry: 6 }
    }
};
```

### Modifier les Paramètres
```javascript
const trailLength = 8;
const particleInterval = 8;
const snowInterval = 300;
```

## 🎨 Capture d'Écran

### Thème Fantôme


### Thème Halloween


### Thème Noël


## 🔍 Détails Techniques

### Performance
- **Optimisé GPU** : Utilisation de `transform` plutôt que `left/top`
- **Gestion mémoire** : Nettoyage automatique des particules
- **Animation fluide** : RequestAnimationFrame pour 60fps

### Compatibilité
- **Navigateurs modernes** : Chrome, Firefox, Safari, Edge
- **Mobile** : Fonctionne sur tablettes et smartphones
- **Responsive** : S'adapte à toutes les résolutions

### Accessibilité
- **Curseur masqué** : Remplacé par l'élément personnalisé
- **Effets non-épileptiques** : Animations douces et progressives
- **Performance** : Léger et optimisé

