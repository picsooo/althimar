# CLAUDE.md — Présentation visuelle du projet « Site Pépinière Ethimar Algérie »

## Contexte

WebMinds (agence digitale, Alger) répond au cahier des charges Réf. 038/2026 du **Groupe Ethimar Algérie** (EURL Mouassassat Ethimar Aldjazaria, Zone SEQUIAA El Khemis, Djelfa) pour la conception du site officiel de la **Pépinière Ethimar Algérie** — Phase 1 de leur écosystème digital.

## Mission

Produire une **présentation visuelle de restitution** que WebMinds enverra au client. Objectif : montrer qu'on a compris le cahier des charges, poser notre lecture du projet, et donner envie de signer. Ce n'est pas un document technique — c'est un support de vente.

Public : la direction d'Ethimar (M. BOURRADA Mohamed Amine). Français uniquement.

## Livrable attendu

Un **fichier HTML unique et autonome** : `presentation-ethimar.html`

- Aucune dépendance externe, aucun CDN, aucune police à télécharger — tout doit s'ouvrir hors ligne par double-clic
- Navigation clavier (flèches ← →) + molette + boutons visibles + indicateur de progression
- Format paysage 16:9, adapté à une projection et à un envoi par email
- Doit s'imprimer proprement en PDF depuis le navigateur (`@media print` : une slide par page A4 paysage)
- CSS et JS inline dans le même fichier

## Direction artistique

Le client demande « premium mais authentiquement agricole, sobre et contemporain » et refuse explicitement les thèmes génériques recolorés. La présentation doit incarner ce niveau, pas juste le décrire.

**Palette** (à définir en variables CSS) :
- Vert olive profond `#2D4A2B` — couleur dominante, fonds de slides fortes
- Vert Ethimar `#4A8B3A` — accents, traits, puces (repris du logo client)
- Crème `#F7F4ED` — fond des slides claires
- Terre `#8B6F3E` — accent secondaire, chiffres clés
- Anthracite `#1C1C1A` — texte courant
- Bleu marine `#1B3A5C` — réservé UNIQUEMENT à la signature WebMinds en pied de slide

**Typographie** : polices système en pile (`Georgia, 'Times New Roman', serif` pour les titres — les serifs donnent le côté institutionnel/agricole ; `system-ui, -apple-system, 'Segoe UI', sans-serif` pour le corps). Aucun webfont.

**Règles** :
- Alternance de slides sombres (fond vert olive) et claires (fond crème) pour rythmer
- Beaucoup de blanc, hiérarchie typographique forte, un seul message par slide
- Formes organiques discrètes en SVG inline (feuille d'olivier, courbe de branche) en filigrane à très faible opacité — jamais de décoration bruyante
- Pas de photos (on n'a pas encore la banque média du client) : utiliser typographie, aplats de couleur, pictogrammes SVG dessinés à la main en code, et espaces négatifs
- Animations d'apparition sobres (fade + translation légère), jamais plus de 400 ms
- Zéro emoji

## Structure des slides

**1. Couverture**
« Pépinière Ethimar Algérie — Site web officiel ». Sous-titre : « Phase 1 — Écosystème digital du Groupe Ethimar Algérie ». Mention « Proposition WebMinds — Août 2026 ». Réf. 038/2026.

**2. Notre lecture du projet**
Reprendre le principe directeur du CDC : le visiteur doit comprendre en quelques secondes qui est Ethimar, ce qu'il maîtrise, pourquoi ses plants méritent confiance, et comment démarrer son projet. Poser la phrase clé : ce n'est pas un site vitrine, c'est une plateforme de référence sur le plant d'olivier en Algérie.

**3. L'architecture de marque**
Schéma SVG : deux blocs distincts (Pépinière / KITAF) reliés par une barre institutionnelle « Groupe Ethimar Algérie ». Message : identités séparées, clientèles séparées, connexion narrative et non commerciale. Phase 1 = Pépinière uniquement, architecture préparée pour KITAF.

**4. La chaîne de valeur**
Frise horizontale SVG : Pépinière → Plantation → Production → Huilerie → Conditionnement → KITAF. Le premier maillon en surbrillance. Message : la pépinière est le point de départ de toute la filière, c'est ce qui crédibilise le reste.

**5. Les 5 publics cibles**
Grille de 5 cartes : Agriculteur / Investisseur agricole / Grand projet ou société / Bureau d'études / Institution. Pour chacun, son besoin principal en une ligne et la réponse du site en une ligne. Contenu tiré du tableau §4 du CDC.

**6. L'arborescence**
Les 13 rubriques du sitemap, présentées visuellement (colonnes ou arbre SVG), pas en liste plate. Accueil, La Pépinière, Notre savoir-faire, Nos variétés, Qualité & Traçabilité, Votre projet oléicole, Services & Accompagnement, Nos projets, Conseils & Expertise, Galerie, Actualités, Groupe Ethimar, Contact.

**7. La page d'accueil — le parcours**
Wireframe schématique de la home en SVG ou CSS : les 11 blocs empilés du §8 du CDC, avec le nom de chaque bloc et une phrase sur sa fonction de conversion. Faire ressortir les deux CTA du hero : « Découvrir nos variétés » et « Demander une étude de projet ».

**8. Le parcours de production**
Les 8 étapes du §10 en frise : matériel végétal → boutures → enracinement → développement racinaire → transplantation → croissance et soins → contrôle et sélection → préparation livraison. C'est le cœur de la démonstration de savoir-faire.

**9. Le catalogue variétal**
Message : chaque variété = une URL, une page autonome, optimisée SEO. Afficher les 6 variétés de la base initiale (Arbequina, Picual, Arbosana, Koroneiki, Sigoise, Chemlal) en cartes. Montrer le principe du statut administrable : Disponible / Réservation ouverte / Prochaine campagne / Non disponible — sous forme de badges colorés.

**10. Le formulaire de qualification**
Le point de conversion du site. Représenter visuellement les 15 champs regroupés en 3 blocs : Identification (nom, téléphone, e-mail) / Projet (wilaya, commune, surface, date, variété, quantité, système de plantation) / Technique (source d'eau, analyse eau, analyse sol, observations, pièces jointes). Mention : structuré, exportable, CRM-ready via API/webhook.

**11. Bilingue FR / AR**
Deux mockups côte à côte d'une même page, l'un en LTR l'autre en RTL miroir complet. Message : RTL natif, pas une inversion partielle. URLs distinctes, hreflang, métadonnées SEO par langue, architecture prête pour l'anglais.

**12. SEO et performance**
Deux colonnes. À gauche le SEO technique (structure sémantique, sitemap, Schema.org, pages variétales indexables par langue, blog d'autorité). À droite la performance (Core Web Vitals mobile, WebP/AVIF, lazy loading, accessibilité). Ajouter les axes de mots-clés cibles du CDC.

**13. Le déroulement du projet**
Les 8 phases A→H en timeline : Cadrage, UX, UI, Contenus, Développement, Recette, Mise en ligne, Formation. Indiquer un délai global de 8 à 10 semaines et les 3 jalons de validation client (arborescence, wireframes, maquettes UI).

**14. Qui fait quoi**
Tableau à deux colonnes Ethimar / WebMinds, repris du §23 du CDC. Message à faire passer : le succès dépend des contenus et médias réels fournis par Ethimar — c'est notre principal facteur de risque planning, à poser dès maintenant.

**15. Ce que nous livrons**
Les 14 livrables du §24 en grille dense et lisible : arborescence validée, wireframes, maquettes desktop + mobile, système graphique, préproduction, back-office, versions FR + AR, formulaires testés, SEO technique, analytics, mise en production, documentation, formation, remise des accès.

**16. Clôture**
Reprendre le principe directeur du CDC en grand, sur fond vert olive. Coordonnées WebMinds : Rue Saïd Hamdine, Haouche Mustapha n° 03 — Bir Mourad Raïs, Alger · 0797 37 24 52 · wsaoudi@webminds.dz · www.webminds.dz

## Ce qu'il ne faut PAS faire

- Ne mets **aucun prix, aucun montant, aucun devis** dans cette présentation — le devis est un document séparé
- Ne mentionne **aucun chiffre sur Ethimar** (capacité, surfaces, nombre de plants, années d'expérience) : le CDC interdit explicitement toute donnée non validée par la direction
- N'invente aucun contenu produit, aucune donnée agronomique sur les variétés
- Ne parle pas de e-commerce, de paiement en ligne, de catalogue d'huile ni de fiches produits KITAF : explicitement hors Phase 1
- N'écris pas « certifié » ou « garanti » à propos d'Ethimar
- Pas de stack technique détaillée, pas de jargon de développeur : le public est une direction d'entreprise agricole

## Vérifications avant de rendre

- [ ] Le fichier s'ouvre seul, sans réseau, et toutes les slides s'affichent
- [ ] Navigation flèches, molette et boutons fonctionnelles, compteur de slides correct
- [ ] Aucun débordement de texte, aucune slide surchargée
- [ ] Impression PDF propre : une slide par page, couleurs conservées
- [ ] Relecture orthographique et typographique française (espaces insécables avant : ; ! ?, guillemets « »)
- [ ] Aucun montant, aucun chiffre inventé sur Ethimar
