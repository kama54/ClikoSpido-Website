# ClikoSpido Launcher — livraison V3 multilingue

## Point de sécurité prioritaire : anciennes pages légales Google Play
Cette archive est une **mise à jour additive** du dépôt `kama54/ClikoSpido-Website` :
- `confidentialite.html`, `conditions.html` et `contact.html` **ne figurent pas dans cette archive**, afin d'éviter toute réécriture de ces documents.
- Lors de l'intégration, **fusionner** les nouveaux fichiers avec le dépôt actuel sans supprimer ces trois pages.
- Contrôler les URL exactes enregistrées dans Google Play Console, et leur réponse HTTP, avant toute mise en ligne. URL présumées :
  - https://kama54.github.io/ClikoSpido-Website/confidentialite.html
  - https://kama54.github.io/ClikoSpido-Website/conditions.html
  - https://kama54.github.io/ClikoSpido-Website/contact.html
- L'accès et les URL Google Play Console ne sont pas vérifiés dans cette livraison. Aucune mise en ligne n'a été réalisée.

## Installation / essai local
Ouvrir `index.html` pour le français ou `en/index.html` pour l'anglais. Le lecteur HTML5 peut nécessiter un petit serveur local pour les fichiers MP4 (exemple `python -m http.server 8000`).

## Structure
- `index.html` : accueil français et conservation de la racine du site
- `xx/index.html` : dix pages d'accueil HTML statiques (`xx` = fr,en,es,it,de,nl,pt,ar,ja,ko)
- `xx/guides/index.html` et 3 guides localisés par langue
- `assets/promo/xx/01.webp` à `08.webp` : 80 visuels localisés
- `assets/videos/xx.mp4` et `assets/video-posters/xx.webp` : 10 vidéos et couvertures
- `assets/site.css`, `assets/site.js` : CSS et interactions
- `sitemap.xml`, `robots.txt`, `favicon.png`

## Prépublication obligatoire
1. Comparer avec `main` et vérifier les URL légales.
2. Vérifier le prix Premium et les fonctions sur l'AAB final / Google Play Billing.
3. Vérifier la politique de confidentialité et les permissions réelles Android.
4. Contrôler le statut Play Store : le site indique **test fermé** (sans fausse disponibilité).
5. Contrôler base d'URL et `canonical`/`hreflang` si domaine personnalisé.
6. Tester manuellement sur Android, iOS, Windows et lecteurs intégrés.
7. Tester toutes les langues, notamment la mise en page RTL arabe.
8. Relire les traductions avec des locuteurs natifs avant publication internationale.
9. Tester Lighthouse et Core Web Vitals **sur le site hébergé** (non mesurés dans cette archive).
10. Intégration dans une branche dédiée uniquement après autorisation, puis fusion sur `main` après validation finale.

## SEO
- 50 URL indexables (5 par langue) + accueil racine duplicata canonique du français.
- Balises title, description, canonical, hreflang et Open Graph par page.
- Données structurées SoftwareApplication sur les accueils, sans fausse note, avis ou date de sortie.
- Les volumes Google Ads Keyword Planner et Google Trends **ne sont pas disponibles** : aucune mesure n'a été inventée.
- Thèmes prioritaires : simplifier un smartphone Android, grandes icônes Android, launcher pour seniors, configurer un téléphone pour un parent. Pas de promesse de classement SEO.

## Limitations
- Les visuels promotionnels fournis ne sont pas présentés comme des captures authentiques d'écrans de l'APK : contrôler leurs différences avec les interfaces finales.
- Les vidéos sont réencodées pour le Web ; les originaux 1080p restent dans le ZIP envoyé initialement par le propriétaire.
- La cible Google Play officielle ne peut pas encore être activée sans vérification de sa disponibilité publique.
