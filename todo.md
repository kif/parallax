# TODO — relecture du 8 juillet 2026

Points restants de la relecture (les corrections d'anglais, point A, ont été appliquées).

## B. Forme et cohérence

- [x] **Figure 1 (`fig:peak_profile`) n'est jamais citée dans le texte** — renvoi ajouté
  le 8 juillet 2026 : « …three main consequences …, illustrated in figure
  \ref{fig:peak_profile}: ».
- [x] **Collision de notation** `$z$` : notation finale choisie par Jérôme — image
  brute $r$ (raw), image avec parallaxe $p$ (parallax) : $p = \Phi r$ et
  $\hat{r} = \operatorname{arg\,min}_r \|\Phi r - p\|^2 + \lambda R(r)$ (8 juillet 2026).
- [x] **Équation `eq:inv`** : `\operatorname{arg\,min}_x` et norme au carré (8 juillet 2026).
- [x] Section 4.1 : « ($\delta x$) » orphelin supprimé (8 juillet 2026).
- [x] Titre section 4.4 : `$\rm CeO_2$` corrigé (8 juillet 2026).
- [ ] **Section 4.4 « Application to experimental data » encore vide** — à rédiger
  (données CeO₂ sur détecteurs Si/CdTe à D2AM).
- [x] Titre section 3.1 : « The Beer--Lambert law » (8 juillet 2026).
- [x] Légende figure 2 (`fig:Si-CdTe`) : ligne verte vérifiée sur la nouvelle figure
  composite ; légende réécrite (panneaux gauche/droite, axe en $2\theta$ et non plus en
  distance) le 8 juillet 2026.
- [x] Micromètres : uniformisés sur `$\mu$m` (plus de µ Unicode dans main.tex) (8 juillet 2026).
- [x] Casse de `\cite{Tikhonov}` harmonisée en `\cite{tikhonov}` (8 juillet 2026).
- [ ] Affiliation [b] encore « TBD » (Gudrun Lotze).
- [ ] Abstract : ajouter un résultat quantitatif quand la section 4.4 sera écrite
  (exigence du journal : abstract « as quantitative as possible »).
- [ ] Permission pour la figure 6 reprise d'Acta Cryst A (`resolution_function`) :
  garder la trace écrite (le `images/ActaCrystA/ik5002_j3bincza.pdf` ?).
- [ ] Résolution des figures : minimum 600 dpi à la taille d'impression (8,8 cm de
  colonne). `fig2_comparison` existe en `.tif`/`.svg` ; les autres PNG (994–1200 px)
  sont en dessous — régénérer depuis les notebooks en haute résolution ou en vectoriel.
- [ ] Fournir une image « graphical abstract » pour la page de sommaire (exigence IUCr).
- [ ] Déposer les données de diffraction primaires (intensités numériques vs 2θ) et
  si possible un DOI pour les données brutes (exigence IUCr pour les articles poudre).
- [ ] Section *Funding information* séparée des remerciements si financement à déclarer.

## C. Citations manquantes proposées

- [ ] **Broennimann et al. (2006)** (clé `pilatus`, PDF déjà dans `library/`) — le
  Pilatus 1M appliquait déjà une « parallax back-transformation » par pixel pour ses
  modules inclinés (capteur Si 320 µm). *Insertion en §2.2 tentée puis retirée le
  8 juillet 2026 (jugée inadaptée) — si citée un jour, trouver un meilleur angle ou
  emplacement, à discuter avec l'auteur.*
- [x] **Kuster et al. (2025)** (clé `parallax-CDI`) — entrée mise à jour vers la version
  publiée (*J. Phys. Conf. Ser.* **3010**, 012135) et citée dans l'introduction le
  8 juillet 2026.
- [x] **Hammersley et al. (1994)** (clé `fit2d1994`) — cité en tête de la section 2
  pour appuyer « The parallax effect has been known for a long time » (8 juillet 2026).
- [ ] **NumPy** (Harris et al., 2020, *Nature* **585**, 357–362) et **SciPy**
  (Virtanen et al., 2020, *Nature Methods* **17**, 261–272) — le code utilise `numpy`
  et `scipy.sparse` alors que Python et Cython sont déjà cités.
- [ ] Optionnel : **Dioptas** (Prescher & Prakapenka, 2015, *High Press. Res.* **35**,
  223–230) en §2.2, comme correction d'incidence oblique existante dans les logiciels
  courants.
- [ ] Optionnel : certificats **NIST** pour SRM640 et SRM674.
