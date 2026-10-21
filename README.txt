# ADEBA — Site de l’association

## Ce dossier contient
- `index.html` : site vitrine animé et responsive.
- `README.txt` : instructions de mise en ligne gratuite et limites actuelles.

## Tester le site
Ouvrez `index.html` dans Chrome, Edge ou Firefox. Les photos et vidéos ajoutées depuis les boutons sont uniquement visibles dans l'aperçu local. Le tableau de cotisations contient des données fictives. Le modèle CSV se télécharge et s'ouvre avec Excel.

## Mise en ligne gratuite du site public avec GitHub Pages
1. Créez un compte sur https://github.com/ si vous n'en avez pas.
2. Créez un nouveau dépôt nommé `adeba-site`.
3. Envoyez `index.html` dans ce dépôt (bouton Add file > Upload files).
4. Dans Settings > Pages, choisissez la branche `main` et le dossier `/ (root)`, puis enregistrez.
5. GitHub affichera l'adresse publique du site après publication. L'adresse exacte dépendra de votre compte.

## Pour rendre l'espace membres réel
Le site actuel est une maquette publique : il n'a pas encore d'authentification, de base de données ni de stockage partagé. Ne mettez pas de vraies cotisations confidentielles dans le tableau public.
Une option de départ consiste à créer un projet Supabase gratuit, puis à configurer :
- authentification par e-mail et mot de passe ;
- tables des membres, cotisations et documents ;
- stockage pour photos, vidéos et fichiers ;
- règles de sécurité Row Level Security (RLS), pour que chaque membre ne voie que ce qui lui est autorisé.
Il faut ensuite ajouter les clés publiques du projet dans le code et les règles de sécurité côté base de données. Ne jamais mettre une clé `service_role` dans un site public. La version actuelle n'est pas encore connectée à Supabase.

## À personnaliser avant publication
- Présentation officielle et objectifs d'ADEBA.
- Nom du village, téléphone, e-mail et liens sociaux.
- Photos et vidéos autorisées par les personnes concernées.
- Règles de cotisation et liste exacte des membres.
- Qui peut voir, modifier ou télécharger chaque type de document.
