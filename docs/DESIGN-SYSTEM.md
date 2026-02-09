# 🎨 Design System - Miscooter × Artimon Bike

**Date :** 9 février 2026  
**Objectif :** Harmonisation visuelle des deux marques avec identités distinctes

---

## 🎯 Philosophie Design

### Artimon Bike (référence)
**Positionnement :** Location vélos, nature, balades familiales  
**Vibe :** Chaleureux, accueillant, tourisme  
**Couleur signature :** Orange terracotta #FF6B35

### Miscooter (nouvelle identité)
**Positionnement :** Vente vélos électriques, urbain, performance  
**Vibe :** Dynamique, tech, moderne  
**Couleur signature :** Orange électrique + Bleu électrique

---

## 🎨 Palettes Couleurs

### Palette Artimon Bike (référence)

```css
/* Artimon Bike - Existant */
:root {
  --artimon-primary: #FF6B35;      /* Orange terracotta */
  --artimon-primary-dark: #E55A2B; /* Orange foncé */
  --artimon-secondary: #1A1A2E;    /* Bleu marine profond */
  --artimon-accent: #16213E;       /* Bleu marine accent */
  --artimon-dark: #111827;         /* Background sombre */
  --artimon-light: #F7F7F7;        /* Background clair */
}
```

### Palette Miscooter (nouvelle)

```css
/* Miscooter - Nouvelle identité harmonisée */
:root {
  /* Primaires */
  --miscooter-primary: #FF6B35;       /* Orange (lien Artimon) */
  --miscooter-primary-light: #FF8C5A; /* Orange clair */
  --miscooter-primary-dark: #E55A2B;  /* Orange foncé */
  
  /* Secondaires - Bleu électrique (identité propre) */
  --miscooter-secondary: #0EA5E9;     /* Bleu électrique vif */
  --miscooter-secondary-light: #38BDF8; /* Bleu clair */
  --miscooter-secondary-dark: #0284C7; /* Bleu foncé */
  
  /* Neutres */
  --miscooter-dark: #0F172A;          /* Background sombre */
  --miscooter-gray: #1E293B;          /* Gris foncé */
  --miscooter-gray-light: #334155;    /* Gris moyen */
  --miscooter-light: #F8FAFC;         /* Background clair */
  --miscooter-white: #FFFFFF;
  
  /* Accents */
  --miscooter-success: #10B981;       /* Vert (dispo stock) */
  --miscooter-warning: #F59E0B;       /* Jaune (stock limité) */
  --miscooter-error: #EF4444;         /* Rouge (rupture) */
  
  /* Gradient signature Miscooter */
  --miscooter-gradient: linear-gradient(135deg, #0EA5E9 0%, #FF6B35 100%);
  --miscooter-gradient-hover: linear-gradient(135deg, #0284C7 0%, #E55A2B 100%);
}
```

**Différenciation visuelle :**
- **Artimon :** Orange dominant + Marine = Chaleur + Nature
- **Miscooter :** Bleu électrique dominant + Orange accent = Tech + Énergie

---

## 📐 Typographie

### Police principale : Poppins

```css
/* Import Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap');

body {
  font-family: 'Poppins', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
```

### Échelle typographique

```css
/* Headings */
.heading-hero {
  font-size: 3.5rem;      /* 56px */
  font-weight: 800;
  line-height: 1.1;
  letter-spacing: -0.02em;
}

.heading-1 {
  font-size: 2.5rem;      /* 40px */
  font-weight: 700;
  line-height: 1.2;
}

.heading-2 {
  font-size: 2rem;        /* 32px */
  font-weight: 700;
  line-height: 1.3;
}

.heading-3 {
  font-size: 1.5rem;      /* 24px */
  font-weight: 600;
  line-height: 1.4;
}

.heading-4 {
  font-size: 1.25rem;     /* 20px */
  font-weight: 600;
  line-height: 1.4;
}

/* Body text */
.body-large {
  font-size: 1.125rem;    /* 18px */
  font-weight: 400;
  line-height: 1.6;
}

.body-base {
  font-size: 1rem;        /* 16px */
  font-weight: 400;
  line-height: 1.6;
}

.body-small {
  font-size: 0.875rem;    /* 14px */
  font-weight: 400;
  line-height: 1.5;
}

/* Special */
.label {
  font-size: 0.875rem;    /* 14px */
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.caption {
  font-size: 0.75rem;     /* 12px */
  font-weight: 400;
  line-height: 1.4;
}
```

---

## 🧩 Composants UI

### Boutons

```css
/* Bouton primaire - Orange (CTA principal) */
.btn-primary {
  background: linear-gradient(135deg, var(--miscooter-primary), var(--miscooter-primary-dark));
  color: var(--miscooter-white);
  padding: 14px 32px;
  border-radius: 8px;
  font-weight: 600;
  font-size: 1rem;
  border: none;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 12px rgba(255, 107, 53, 0.3);
}

.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(255, 107, 53, 0.4);
}

/* Bouton secondaire - Bleu électrique */
.btn-secondary {
  background: linear-gradient(135deg, var(--miscooter-secondary), var(--miscooter-secondary-dark));
  color: var(--miscooter-white);
  padding: 14px 32px;
  border-radius: 8px;
  font-weight: 600;
  font-size: 1rem;
  border: none;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 12px rgba(14, 165, 233, 0.3);
}

.btn-secondary:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(14, 165, 233, 0.4);
}

/* Bouton outline */
.btn-outline {
  background: transparent;
  color: var(--miscooter-primary);
  padding: 14px 32px;
  border-radius: 8px;
  font-weight: 600;
  font-size: 1rem;
  border: 2px solid var(--miscooter-primary);
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn-outline:hover {
  background: var(--miscooter-primary);
  color: var(--miscooter-white);
}

/* Bouton ghost (liens) */
.btn-ghost {
  background: transparent;
  color: var(--miscooter-secondary);
  padding: 8px 16px;
  border: none;
  font-weight: 500;
  cursor: pointer;
  transition: all 0.2s ease;
}

.btn-ghost:hover {
  color: var(--miscooter-secondary-dark);
  text-decoration: underline;
}
```

### Cards produits

```css
.product-card {
  background: var(--miscooter-white);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
  transition: all 0.3s ease;
}

.product-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 12px 24px rgba(0, 0, 0, 0.12);
}

.product-card__image {
  width: 100%;
  aspect-ratio: 4/3;
  object-fit: cover;
}

.product-card__badge {
  position: absolute;
  top: 12px;
  right: 12px;
  background: var(--miscooter-primary);
  color: white;
  padding: 6px 12px;
  border-radius: 6px;
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
}

.product-card__content {
  padding: 20px;
}

.product-card__title {
  font-size: 1.25rem;
  font-weight: 600;
  color: var(--miscooter-dark);
  margin-bottom: 8px;
}

.product-card__price {
  font-size: 1.75rem;
  font-weight: 700;
  color: var(--miscooter-primary);
  margin-bottom: 12px;
}

.product-card__specs {
  display: flex;
  gap: 12px;
  margin-bottom: 16px;
}

.product-card__spec {
  display: flex;
  align-items: center;
  gap: 6px;
  font-size: 0.875rem;
  color: var(--miscooter-gray-light);
}
```

### Badges & Tags

```css
/* Badge disponibilité */
.badge-stock-ok {
  background: #DCFCE7;
  color: #166534;
  padding: 4px 12px;
  border-radius: 6px;
  font-size: 0.75rem;
  font-weight: 600;
}

.badge-stock-low {
  background: #FEF3C7;
  color: #92400E;
  padding: 4px 12px;
  border-radius: 6px;
  font-size: 0.75rem;
  font-weight: 600;
}

.badge-stock-out {
  background: #FEE2E2;
  color: #991B1B;
  padding: 4px 12px;
  border-radius: 6px;
  font-size: 0.75rem;
  font-weight: 600;
}

/* Tags catégories */
.tag {
  display: inline-block;
  background: var(--miscooter-light);
  color: var(--miscooter-dark);
  padding: 6px 14px;
  border-radius: 20px;
  font-size: 0.875rem;
  font-weight: 500;
  transition: all 0.2s ease;
}

.tag:hover {
  background: var(--miscooter-primary);
  color: white;
  cursor: pointer;
}
```

### Navigation & Header

```css
/* Header principal */
.header {
  background: var(--miscooter-white);
  border-bottom: 1px solid rgba(0, 0, 0, 0.08);
  position: sticky;
  top: 0;
  z-index: 1000;
  backdrop-filter: blur(10px);
  background: rgba(255, 255, 255, 0.95);
}

.nav-link {
  color: var(--miscooter-dark);
  font-weight: 500;
  padding: 8px 16px;
  border-radius: 6px;
  transition: all 0.2s ease;
}

.nav-link:hover {
  background: rgba(14, 165, 233, 0.1);
  color: var(--miscooter-secondary);
}

.nav-link.active {
  background: var(--miscooter-secondary);
  color: white;
}
```

### Formulaires

```css
/* Input text */
.input {
  width: 100%;
  padding: 12px 16px;
  border: 2px solid #E2E8F0;
  border-radius: 8px;
  font-size: 1rem;
  font-family: 'Poppins', sans-serif;
  transition: all 0.2s ease;
}

.input:focus {
  outline: none;
  border-color: var(--miscooter-secondary);
  box-shadow: 0 0 0 3px rgba(14, 165, 233, 0.1);
}

.input:disabled {
  background: #F1F5F9;
  cursor: not-allowed;
}

/* Select */
.select {
  width: 100%;
  padding: 12px 16px;
  border: 2px solid #E2E8F0;
  border-radius: 8px;
  font-size: 1rem;
  font-family: 'Poppins', sans-serif;
  background: white;
  cursor: pointer;
  transition: all 0.2s ease;
}

.select:focus {
  outline: none;
  border-color: var(--miscooter-secondary);
  box-shadow: 0 0 0 3px rgba(14, 165, 233, 0.1);
}

/* Checkbox */
.checkbox {
  appearance: none;
  width: 20px;
  height: 20px;
  border: 2px solid #CBD5E1;
  border-radius: 4px;
  cursor: pointer;
  position: relative;
  transition: all 0.2s ease;
}

.checkbox:checked {
  background: var(--miscooter-secondary);
  border-color: var(--miscooter-secondary);
}

.checkbox:checked::after {
  content: '✓';
  position: absolute;
  color: white;
  font-size: 14px;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

---

## 📱 Responsive Design

### Breakpoints

```css
/* Mobile first approach */
:root {
  --breakpoint-sm: 640px;   /* Mobile landscape */
  --breakpoint-md: 768px;   /* Tablet portrait */
  --breakpoint-lg: 1024px;  /* Tablet landscape */
  --breakpoint-xl: 1280px;  /* Desktop */
  --breakpoint-2xl: 1536px; /* Large desktop */
}

/* Usage */
@media (min-width: 768px) {
  .container {
    max-width: 720px;
  }
}

@media (min-width: 1024px) {
  .container {
    max-width: 960px;
  }
}

@media (min-width: 1280px) {
  .container {
    max-width: 1140px;
  }
}
```

### Grid System

```css
/* Container */
.container {
  width: 100%;
  max-width: 1280px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Grid 12 colonnes */
.grid {
  display: grid;
  gap: 24px;
}

.grid-cols-1 { grid-template-columns: repeat(1, 1fr); }
.grid-cols-2 { grid-template-columns: repeat(2, 1fr); }
.grid-cols-3 { grid-template-columns: repeat(3, 1fr); }
.grid-cols-4 { grid-template-columns: repeat(4, 1fr); }

/* Responsive grid */
@media (min-width: 768px) {
  .md\:grid-cols-2 { grid-template-columns: repeat(2, 1fr); }
  .md\:grid-cols-3 { grid-template-columns: repeat(3, 1fr); }
}

@media (min-width: 1024px) {
  .lg\:grid-cols-3 { grid-template-columns: repeat(3, 1fr); }
  .lg\:grid-cols-4 { grid-template-columns: repeat(4, 1fr); }
}
```

---

## 🎭 Animations

### Transitions standard

```css
/* Vitesses */
:root {
  --transition-fast: 150ms;
  --transition-base: 250ms;
  --transition-slow: 350ms;
  --transition-slower: 500ms;
}

/* Easings */
:root {
  --ease-in: cubic-bezier(0.4, 0, 1, 1);
  --ease-out: cubic-bezier(0, 0, 0.2, 1);
  --ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
  --ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
}
```

### Animations clés

```css
/* Fade in up */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-fade-in-up {
  animation: fadeInUp 0.6s ease-out forwards;
}

/* Slide in */
@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateX(-30px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.animate-slide-in {
  animation: slideIn 0.5s ease-out forwards;
}

/* Scale in */
@keyframes scaleIn {
  from {
    opacity: 0;
    transform: scale(0.95);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

.animate-scale-in {
  animation: scaleIn 0.4s ease-out forwards;
}

/* Pulse (pour badges "nouveau") */
@keyframes pulse {
  0%, 100% {
    opacity: 1;
  }
  50% {
    opacity: 0.7;
  }
}

.animate-pulse {
  animation: pulse 2s ease-in-out infinite;
}

/* Hover lift effect */
.hover-lift {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.hover-lift:hover {
  transform: translateY(-8px);
  box-shadow: 0 12px 24px rgba(0, 0, 0, 0.12);
}
```

---

## 🌈 Gradients & Effets

### Gradients signature

```css
/* Gradient principal Miscooter */
.gradient-miscooter {
  background: linear-gradient(135deg, #0EA5E9 0%, #FF6B35 100%);
}

/* Gradient overlay sur images */
.gradient-overlay {
  position: relative;
}

.gradient-overlay::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(180deg, transparent 0%, rgba(15, 23, 42, 0.8) 100%);
}

/* Gradient text */
.gradient-text {
  background: linear-gradient(135deg, #0EA5E9, #FF6B35);
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}
```

### Ombres (shadows)

```css
:root {
  /* Ombres élévation */
  --shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  --shadow-base: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  --shadow-md: 0 4px 12px rgba(0, 0, 0, 0.08);
  --shadow-lg: 0 12px 24px rgba(0, 0, 0, 0.12);
  --shadow-xl: 0 20px 40px rgba(0, 0, 0, 0.15);
  
  /* Ombres colorées */
  --shadow-primary: 0 8px 20px rgba(255, 107, 53, 0.3);
  --shadow-secondary: 0 8px 20px rgba(14, 165, 233, 0.3);
}
```

### Glass effect (optionnel)

```css
.glass {
  background: rgba(255, 255, 255, 0.8);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.3);
}

.glass-dark {
  background: rgba(15, 23, 42, 0.8);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.1);
}
```

---

## 🖼️ Iconographie

### Icon system

**Bibliothèque recommandée :** [Lucide Icons](https://lucide.dev/) (open source, cohérentes)

**Tailles standard :**
```css
.icon-xs { width: 16px; height: 16px; }
.icon-sm { width: 20px; height: 20px; }
.icon-base { width: 24px; height: 24px; }
.icon-lg { width: 32px; height: 32px; }
.icon-xl { width: 40px; height: 40px; }
```

**Couleurs icons :**
- Primaire : `var(--miscooter-primary)`
- Secondaire : `var(--miscooter-secondary)`
- Neutre : `var(--miscooter-gray-light)`

### Illustrations

**Style :** Flat, moderne, minimaliste  
**Palette :** Utiliser les couleurs Miscooter  
**Usage :** Pages vides, erreurs, onboarding

---

## 🔗 Lien avec Artimon Bike

### Points de cohérence (famille visuelle)

1. **Typographie commune :** Poppins (reconnaissance immédiate)
2. **Orange #FF6B35 :** Couleur pont entre les deux marques
3. **Border radius :** 8-12px (arrondis doux)
4. **Spacing system :** Identique (4px base)
5. **Animation style :** Smooth, professionnel

### Points de différenciation (identité propre)

1. **Couleur dominante :**
   - Artimon : Orange chaud (nature)
   - Miscooter : Bleu électrique (tech)

2. **Visuels :**
   - Artimon : Photos nature, balades, familles
   - Miscooter : Produits, specs techniques, urbain

3. **Ton :**
   - Artimon : Chaleureux, invitation à l'aventure
   - Miscooter : Dynamique, performance, innovation

---

## 📦 Export CSS Variables (prêt à l'emploi)

```css
/* miscooter-variables.css */
:root {
  /* Couleurs primaires */
  --miscooter-primary: #FF6B35;
  --miscooter-primary-light: #FF8C5A;
  --miscooter-primary-dark: #E55A2B;
  
  /* Couleurs secondaires */
  --miscooter-secondary: #0EA5E9;
  --miscooter-secondary-light: #38BDF8;
  --miscooter-secondary-dark: #0284C7;
  
  /* Neutres */
  --miscooter-dark: #0F172A;
  --miscooter-gray: #1E293B;
  --miscooter-gray-light: #334155;
  --miscooter-gray-lighter: #94A3B8;
  --miscooter-light: #F8FAFC;
  --miscooter-white: #FFFFFF;
  
  /* Statuts */
  --miscooter-success: #10B981;
  --miscooter-warning: #F59E0B;
  --miscooter-error: #EF4444;
  --miscooter-info: #3B82F6;
  
  /* Gradients */
  --miscooter-gradient: linear-gradient(135deg, #0EA5E9 0%, #FF6B35 100%);
  --miscooter-gradient-hover: linear-gradient(135deg, #0284C7 0%, #E55A2B 100%);
  
  /* Ombres */
  --shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  --shadow-base: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  --shadow-md: 0 4px 12px rgba(0, 0, 0, 0.08);
  --shadow-lg: 0 12px 24px rgba(0, 0, 0, 0.12);
  --shadow-xl: 0 20px 40px rgba(0, 0, 0, 0.15);
  --shadow-primary: 0 8px 20px rgba(255, 107, 53, 0.3);
  --shadow-secondary: 0 8px 20px rgba(14, 165, 233, 0.3);
  
  /* Transitions */
  --transition-fast: 150ms;
  --transition-base: 250ms;
  --transition-slow: 350ms;
  --transition-slower: 500ms;
  
  /* Easings */
  --ease-in: cubic-bezier(0.4, 0, 1, 1);
  --ease-out: cubic-bezier(0, 0, 0.2, 1);
  --ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
  --ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
  
  /* Spacing (système 4px) */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-5: 20px;
  --space-6: 24px;
  --space-8: 32px;
  --space-10: 40px;
  --space-12: 48px;
  --space-16: 64px;
  --space-20: 80px;
  --space-24: 96px;
  
  /* Border radius */
  --radius-sm: 4px;
  --radius-base: 8px;
  --radius-md: 12px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;
  
  /* Breakpoints (référence, usage dans @media) */
  --breakpoint-sm: 640px;
  --breakpoint-md: 768px;
  --breakpoint-lg: 1024px;
  --breakpoint-xl: 1280px;
  --breakpoint-2xl: 1536px;
}
```

---

## ✅ Checklist implémentation

### Phase 1 - Variables & Base
- [ ] Importer `miscooter-variables.css`
- [ ] Importer Google Fonts (Poppins)
- [ ] Reset CSS de base

### Phase 2 - Composants core
- [ ] Boutons (primary, secondary, outline, ghost)
- [ ] Cards produits
- [ ] Navigation header
- [ ] Footer

### Phase 3 - Composants avancés
- [ ] Formulaires (input, select, checkbox)
- [ ] Badges & tags
- [ ] Modals
- [ ] Toasts/notifications

### Phase 4 - Pages
- [ ] Homepage
- [ ] Page collection (listing produits)
- [ ] Page produit (single)
- [ ] Page panier
- [ ] Page showroom Marseillan

### Phase 5 - Responsive
- [ ] Test mobile (320px - 767px)
- [ ] Test tablet (768px - 1023px)
- [ ] Test desktop (1024px+)

---

## 🎬 Prochaines étapes

1. **Implémenter dans Shopify** → Voir `GUIDE-SHOPIFY.md`
2. **Créer templates Liquid** → Voir `GUIDE-SHOPIFY.md`
3. **Intégrer catalogue vélos** → Voir `STRUCTURE-VELOS.md`
4. **Optimiser SEO** → Voir `SEO-STRATEGY.md`

---

*Design System créé le 9 février 2026*  
*Harmonisation Miscooter × Artimon Bike*  
*Prêt pour implémentation Shopify*