<div align="center">

# ⚛️ The Elements

### Interactive Periodic Table & Chemistry Laboratory

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://github.com/gunout/physique-chimie)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://github.com/gunout/physique-chimie)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://github.com/gunout/physique-chimie)
[![License](https://img.shields.io/badge/license-MIT-00ff9d?style=for-the-badge)](https://github.com/gunout/physique-chimie/blob/main/LICENSE)
[![Stars](https://img.shields.io/github/stars/gunout/physique-chimie?style=for-the-badge&color=00e5ff&labelColor=0D001A)](https://github.com/gunout/physique-chimie/stargazers)
[![Forks](https://img.shields.io/github/forks/gunout/physique-chimie?style=for-the-badge&color=a855f7&labelColor=0D001A)](https://github.com/gunout/physique-chimie/network)
[![Issues](https://img.shields.io/github/issues/gunout/physique-chimie?style=for-the-badge&color=ff3b6b&labelColor=0D001A)](https://github.com/gunout/physique-chimie/issues)
[![Last Commit](https://img.shields.io/github/last-commit/gunout/physique-chimie?style=for-the-badge&color=ffd93b&labelColor=0D001A)](https://github.com/gunout/physique-chimie/commits)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-gunout.github.io-FF2D95?style=for-the-badge&logo=githubpages&logoColor=white)](https://gunout.github.io/physique-chimie/)

</div>

---

## 📋 Aperçu

**The Elements** est un laboratoire de chimie interactif 100 % autonome, packagé dans un seul fichier HTML. Il combine un tableau périodique complet (118 éléments), un moteur d'équilibrage redox, des diagrammes de Latimer et Frost, un analyseur VSEPR/Lewis, des calculs thermodynamiques (Hess, ΔG°, Nernst), un calculateur de pH, et un lecteur audio intégré — le tout dans une interface cyberpunk néon avec un atome 3D animé.

> ⚠️ **Outil pédagogique** — Ne remplace pas un cours de chimie ou un manuel de référence.

---

## ✨ Fonctionnalités

**⚛️ Tableau périodique & atome 3D**
- 118 éléments (H → Og) avec masse, protons, neutrons, configuration électronique
- Atome 3D animé (noyau protons+neutrons, orbites électroniques)
- Configurations complètes (1s² 2s² 2p⁶…) et couches K-Q
- Familles : alcalins, transition, halogènes, gaz nobles, lanthanides, actinides

**🎨 Spectre atomique interactif**
- Mode Émission : raies colorées sur fond noir (spectres réels 40+ éléments)
- Mode Absorption : raies noires sur gradient physique
- Mode Gradient : raies blanches sur dégradé 380-750 nm
- Conversion longueur d'onde → RGB (algorithme physique)

**⚖️ Équilibrage d'équations redox**
- Réactions simples et complexes (KMnO4 + HCl -> …)
- Support des parenthèses, charges ioniques, hydrates
- Méthode : Gauss-Jordan sur matrice éléments + charge
- Vérification conservation masse ET charge
- Coefficients entiers positifs normalisés par PGCD

**⚡ Diagrammes Redox**
- Latimer : espèces oxydées → réduites avec E° (Fe, Mn, Cr, Cu, N, S, Cl, O, Ag, Pb)
- Frost : nE° vs nombre d'oxydation (SVG interactif)

**🔬 Outils avancés**
- Loi de Hess : ΔH°r via enthalpies de formation (100+ composés)
- Thermodynamique : ΔG°, constante K, spontanéité
- Nernst : E = E° − (RT/nF)·ln(Q)
- VSEPR/Lewis : géométrie, hybridation, angle (13 géométries)
- pH et Henderson-Hasselbalch
- Exercice d'équilibrage avec vérification

**🎵 Lecteur audio**
- Bande-son d'ambiance (mashup.mp3)
- Waveform animée, volume, seek

---

## 🚀 Lancement rapide

```bash
git clone https://github.com/gunout/physique-chimie.git
cd physique-chimie
python3 -m http.server 8080
```

Ouvrir **http://localhost:8080** dans ton navigateur.

Ou directement : `open index.html` (macOS) / `start index.html` (Windows) / `xdg-open index.html` (Linux).

> 💡 **Note** : serveur HTTP recommandé pour la lecture audio.

---

## 🎮 Contrôles

| Action | Description |
|--------|-------------|
| **Clic élément** | Charge l'élément (symbole, atome, spectre, réactions, Latimer) |
| **Clic réaction** | Envoie l'équation vers le Solver |
| **Clic mode spectre** | Bascule Émission / Absorption / Gradient |
| **Enter dans le Solver** | Équilibre l'équation |
| **Clic waveform** | Seek audio |

---

## 📁 Structure

```
physique-chimie/
├── index.html      # Application complète (~2000 lignes)
├── mashup.mp3      # Bande-son
├── LICENSE         # MIT
└── README.md
```

**Aucune dépendance. Aucun build.**

---

## 🛠️ Stack technique

| Composant | Technologie |
|-----------|-------------|
| Structure | HTML5 |
| Style | CSS3 (variables, grid, 3D transforms) |
| Logique | JavaScript ES6+ vanilla |
| Graphiques | SVG inline |
| Audio | audio HTML5 |
| Algèbre | Gauss-Jordan |
| Data | 118 éléments, 40+ spectres, 100+ ΔHf° |

---

## 📊 Métriques

| Métrique | Valeur |
|----------|--------|
| Éléments | **118** |
| Spectres réels | **40+** |
| Composés ΔHf° | **100+** |
| Diagrammes Latimer | **10** |
| Géométries VSEPR | **13** |
| Lignes de code | **~2000** |
| Taille | **~100 Ko** |
| Dépendances | **0** |

---

## 🎯 Public cible

Lycéens scientifiques, étudiants prépa/licence/BTS chimie, enseignants, curieux.

---

## 🗺️ Roadmap

- [x] **v1.0** — Tableau, atome 3D, spectre, redox, Latimer/Frost, VSEPR, thermo, pH, audio
- [ ] **v1.1** — Toggle sombre/clair
- [ ] **v1.2** — Export PDF fiches éléments
- [ ] **v1.3** — Simulateur titrage acide-base
- [ ] **v1.4** — Mécanismes organiques
- [ ] **v2.0** — Backend progression

---

## 🤝 Contribution

```bash
git checkout -b feature/ma-contribution
git commit -m "feat: ajout de ma contribution"
git push origin feature/ma-contribution
```

**Convention** : `feat:` / `fix:` / `docs:` / `style:` / `refactor:` / `content:`

---

## ⚠️ Avertissement

**Outil pédagogique.** Ne remplace pas un cours. Les valeurs (E°, ΔHf°, spectres) sont approximatives. Pour des calculs critiques, consultez NIST ou manuels de référence.

---

## 📄 Licence

Distribué sous **MIT**. Voir [LICENSE](https://github.com/gunout/physique-chimie/blob/main/LICENSE).

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-gunout-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/gunout)

Fait avec ❤️ et ⚗️ en France — Octobre 2026

</div>

---

<div align="center">

### 🇫🇷 Gunout · 2026

![Made in France](https://img.shields.io/badge/Made_in-France-002395?style=flat-square&labelColor=FFFFFF&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA5MDAgNjAwIj48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjYwMCIgZmlsbD0iIzAwMjM5NSIvPjxyZWN0IHdpZHRoPSI5MDAiIGhlaWdodD0iNDAwIiB5PSIxMDAiIGZpbGw9IiNmZmYiLz48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjIwMCIgeT0iNDAwIiBmaWxsPSIjZWQyOTM5Ii8+PC9zdmc+)
![GitHub](https://img.shields.io/badge/GitHub-gunout-181717?style=flat-square&logo=github&logoColor=white)
![Year](https://img.shields.io/badge/2026-ED2939?style=flat-square&labelColor=FFFFFF)

<sub>© 2026 <strong>Gunout</strong> — Tous droits réservés.</sub>

</div>
