# TODO — relecture du 8 juillet 2026

Points restants de la relecture (les corrections d'anglais, point A, ont été appliquées).

## B. Forme et cohérence

- [ ] **Figure 1 (`fig:peak_profile`) n'est jamais citée dans le texte** — le journal exige
  que les figures soient numérotées dans l'ordre de citation. Ajouter un renvoi, par
  exemple ligne ~139 : « …three main consequences (figure \ref{fig:peak_profile}): ».
- [ ] **Collision de notation** : `$z$` désigne à la fois l'image floutée
  (équation `eq:blur`) et la profondeur dans le capteur (section 4.1). Renommer
  l'image floutée `$y$` dans `eq:blur` et `eq:inv`.
- [ ] **Équation `eq:inv`** : `argmin` en italique mathématique →
  `\operatorname{arg\,min}_x` ; remplacer la valeur absolue par une norme,
  typiquement au carré : `\hat{x} = \operatorname{arg\,min}_x \|\Phi x - z\|^2 + \lambda R(x)`.
- [ ] Section 4.1 : « ($\delta x$) » introduit mais jamais réutilisé (le texte emploie
  `$\langle x \rangle$`) — supprimer ou harmoniser.
- [ ] Titre section 4.4 : `$\rm CeO2$` → `$\rm CeO_2$` (indice manquant).
- [ ] **Section 4.4 « Application to experimental data » encore vide** — à rédiger
  (données CeO₂ sur détecteurs Si/CdTe à D2AM).
- [ ] Titre section 3.1 : « Beer-Lambert Law » → « The Beer--Lambert law »
  (tiret demi-cadratin, minuscule à law).
- [ ] Légende figure 2 (`fig:Si-CdTe`) : vérifier que `fig2_comparison.png` montre bien
  une « green line » (sur le transparent 3, la ligne de coupe était jaune).
- [ ] Micromètres : usage mixte `$450 \mu$m` / « µm » Unicode — uniformiser sur `$\mu$m`.
- [ ] Harmoniser la casse de la clé de citation `\cite{Tikhonov}` vs `tikhonov` dans
  `biblio.bib` (BibTeX est insensible à la casse, mais fragile si changement d'outil).
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
- [ ] **Hammersley et al. (1994)** (clé `fit2d1994`, PDF dans `library/`) — pour appuyer
  « The parallax effect has been known for a long time » (§2) : ce papier nomme
  explicitement la parallaxe (fenêtre d'entrée des XRII) et fonde les corrections de
  distorsion spatiale.
- [ ] **NumPy** (Harris et al., 2020, *Nature* **585**, 357–362) et **SciPy**
  (Virtanen et al., 2020, *Nature Methods* **17**, 261–272) — le code utilise `numpy`
  et `scipy.sparse` alors que Python et Cython sont déjà cités.
- [ ] Optionnel : **Dioptas** (Prescher & Prakapenka, 2015, *High Press. Res.* **35**,
  223–230) en §2.2, comme correction d'incidence oblique existante dans les logiciels
  courants.
- [ ] Optionnel : certificats **NIST** pour SRM640 et SRM674.
