# 🚀 Refonte Miscooter.fr - Plan Complet
**Client:** Artimon Bike (même propriétaire)  
**Deadline:** 9 février 2026  
**Objectif:** Ajouter vente vélos électriques + harmoniser avec artimonbike.com

---

## 📊 PHASE 1 - Audit & Analyse (EN COURS)

### Site actuel Miscooter.fr
- **Platform:** Shopify
- **Focus actuel:** Pièces détachées trottinettes électriques
- **Services:** E-commerce + Réparation physique
- **Multi-langue:** FR/EN (mal configuré, redirige EN par défaut)

### Site référence Artimon Bike
- **Platform:** React SPA (static build)
- **Focus:** Location vélos électriques Marseillan
- **Points forts:**
  - SEO local exemplaire (Schema.org complet)
  - Note 4.6/5 (89 avis)
  - Performance optimisée (Vercel)
  - Identité visuelle forte (orange #FF6B35, bleu marine)

---

## 🎨 PHASE 2 - Design System Unifié

### Objectif
Créer une identité visuelle commune pour Artimon Bike + Miscooter tout en gardant leur personnalité propre.

### Livrables
1. **Charte graphique harmonisée**
   - Palette couleurs commune
   - Typographie unifiée (Poppins)
   - Composants partagés (boutons, cards, forms)

2. **Guide Shopify**
   - Code Liquid pour thème custom
   - CSS snippets prêts à injecter
   - Assets visuels optimisés

3. **Mockups sections clés**
   - Header/navigation
   - Page produit vélo électrique
   - Cross-selling Artimon ↔ Miscooter
   - Footer avec liens croisés

---

## 🛒 PHASE 3 - Section Vélos Électriques

### Structure e-commerce
**Collections Shopify à créer:**
- Vélos électriques urbains
- VTT électriques
- VTC électriques
- Accessoires vélos
- Packs location longue durée

### Fiches produits optimisées
**Template standard par vélo:**
- Photos HD multiples (lifestyle + détails techniques)
- Specs techniques (autonomie, poids, moteur, batterie)
- Schema.org Product complet
- Reviews intégrés
- Cross-sell vers pièces détachées Miscooter
- CTA "Essayer en location chez Artimon Bike"

### SEO local vélos
**Mots-clés cibles:**
- "vente vélo électrique Marseillan"
- "acheter vélo électrique Hérault"
- "vélo électrique Agde Sète"
- "VAE étang de Thau"
- "boutique vélo électrique 34"

---

## 🔗 PHASE 4 - Intégration Artimon ↔ Miscooter

### Cross-selling stratégique

**Sur Artimon Bike:**
- Ajout section "Boutique en ligne" pointant Miscooter
- CTA "Acheter votre vélo" après location
- Lien vers pièces détachées/accessoires

**Sur Miscooter:**
- Bandeau "Essayez avant d'acheter chez Artimon Bike Marseillan"
- Page dédiée "Location vélo" avec iframe/embed Artimon
- Section "Notre showroom" (adresse Artimon Bike)

### Parcours client unifié
```
Location Artimon → Achat Miscooter → SAV Artimon
     ↓                    ↓                ↓
  Essai réel      Livraison France    Atelier local
```

---

## 📈 PHASE 5 - SEO & Performance

### Optimisations techniques Shopify
1. **Schema.org LocalBusiness** (même niveau qu'Artimon)
   - Adresse Marseillan
   - Horaires atelier
   - Téléphone/email
   - Zone livraison

2. **Schema.org Product** pour chaque vélo
   - Prix, disponibilité
   - Reviews
   - Images optimisées
   - Variantes (couleurs, tailles)

3. **Performance**
   - Lazy loading images
   - WebP + fallback
   - Critical CSS inline
   - Preconnect fonts/CDN

4. **Multi-langue fixé**
   - FR par défaut
   - EN accessible via sélecteur
   - hreflang correct

### Contenu SEO
**Blog articles à créer:**
1. "Choisir son vélo électrique pour l'Étang de Thau"
2. "Location vs Achat : quel vélo électrique pour vous ?"
3. "Entretenir son vélo électrique : nos conseils d'experts"
4. "Les meilleurs parcours cyclables autour de Marseillan"
5. "Pièces détachées vélo électrique : guide complet"

---

## 🎯 PHASE 6 - Prompt Emergent

### Template site complet
**Générer avec Emergent:**
- Landing page vélos électriques
- Pages catégories (urbain/VTT/VTC)
- Template fiche produit
- Page "Notre atelier Marseillan"
- FAQ achat/livraison/garantie

### Spécifications prompt
- Intégration Shopify Liquid
- Design inspiré Artimon Bike
- SEO local pré-optimisé
- Schema.org inclus
- Mobile-first
- Accessibilité WCAG AA

---

## 📦 LIVRABLES FINAUX

### Documents
1. ✅ `AUDIT-MISCOOTER.md` - Analyse complète site actuel
2. ✅ `DESIGN-SYSTEM.md` - Charte graphique unifiée
3. ✅ `GUIDE-SHOPIFY.md` - Code Liquid + CSS custom
4. ✅ `STRUCTURE-VELOS.md` - Architecture collections/produits
5. ✅ `SEO-STRATEGY.md` - Mots-clés + contenu
6. ✅ `PROMPT-EMERGENT.md` - Prompt complet prêt à l'emploi

### Code
- `/templates/` - Templates Liquid Shopify
- `/assets/` - CSS custom + JS
- `/sections/` - Sections réutilisables
- `/snippets/` - Components

### Assets
- Logo Miscooter harmonisé
- Palette couleurs exportée (CSS variables)
- Mockups Figma/PNG
- Photos produits optimisées

---

## ⏱️ PLANNING

**Ce soir (8 fév 20h-00h):**
- ✅ Audit Miscooter complet
- ✅ Design system base
- ✅ Structure collections

**Demain matin (9 fév 8h-12h):**
- ✅ Templates Liquid
- ✅ Prompt Emergent
- ✅ Guide implémentation

**Demain après-midi (9 fév 14h-18h):**
- ✅ Review avec Cyril
- ✅ Ajustements
- ✅ Livraison finale

---

## 🚨 POINTS D'ATTENTION

### À valider avec le client
1. **Localisation physique Miscooter** - Même adresse qu'Artimon Bike ?
2. **Marques vélos** - Quelles marques vendre ?
3. **Prix cibles** - Gamme 800-3000€ ?
4. **Zone livraison** - France entière ou Occitanie d'abord ?
5. **Stock physique** - Showroom sur place ou dropshipping ?

### Dépendances techniques
- Accès admin Shopify nécessaire
- Thème Shopify actuel (quel thème ?)
- Budget Shopify Apps (reviews, SEO, etc.)
- Compte Google Business Miscooter

---

## 📞 PROCHAINE ÉTAPE

**Action immédiate:** Commencer Phase 1 - Audit approfondi

**Questions pour Cyril:**
1. URL admin Shopify ?
2. Thème Shopify actuel ?
3. Catalogues vélos existants ?
4. Budget apps Shopify mensuels ?

---

*Document créé le 8 février 2026 20:27 UTC*  
*Agent: Clawdbot Main*  
*Projet: Miscooter × Artimon Bike*
