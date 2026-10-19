# Iron Log

Carnet de musculation personnel, inspiré d'Épilogue. Une seule page web (`index.html`), sans compte, sans serveur, sans pub, sans suivi. Tes données restent sur ton appareil.

**Application en ligne : https://krad-max.github.io/iron-log/**

## Installer sur le téléphone

- **iPhone (Safari)** : ouvre le lien, touche le bouton Partager, puis « Sur l'écran d'accueil ».
- **Android (Chrome)** : ouvre le lien, menu ⋮, puis « Installer l'application » ou « Ajouter à l'écran d'accueil ».

Une fois installée, l'app fonctionne sans connexion. Appui long sur l'icône (Android) : raccourcis « Séance du jour », « Progrès » et « Coach ».

## Sauvegarder et restaurer

Tout est stocké dans le navigateur de l'appareil. Si tu changes de téléphone ou effaces les données du navigateur, tu perds tout : **exporte une sauvegarde de temps en temps**.

- Profil, **Exporter une sauvegarde** : fichier `.json` complet (séances, programme, objectifs, mesures, réglages).
- Profil, **Importer une sauvegarde** : restaure ce fichier sur un autre appareil.
- Profil, **Exporter l'historique (CSV)** : tableau lisible dans Excel, une ligne par série.
- Les **photos de progression** restent sur l'appareil et ne sont pas incluses dans la sauvegarde.

## Coach IA (facultatif)

L'onglet Coach fonctionne sans rien configurer (règles locales, hors-ligne). Pour discuter avec le coach IA, colle ta clé d'API Claude dans l'onglet Coach. Elle reste dans ce navigateur et n'est envoyée qu'à l'API d'Anthropic.

## Rappels

Profil, **Rappels** : heures de séance, pesée, sauvegarde. Les notifications ne s'affichent que si l'app est ouverte ou en arrière-plan. Pour des rappels fiables écran verrouillé, exporte le fichier `.ics` et ouvre-le dans ton agenda.

## Héberger sa propre copie (GitHub Pages)

1. Crée un dépôt public sur GitHub et dépose les fichiers de ce dossier à la racine.
2. Réglages du dépôt, Pages, branche `main`, dossier `/ (root)`.
3. L'app est en ligne quelques minutes plus tard à `https://<ton-compte>.github.io/<dépôt>/`.

Pour publier une mise à jour, remplace `index.html` et change le nom du cache dans `sw.js` (`il-vN`) pour que les téléphones rechargent la nouvelle version.

## Limites connues

- Pas d'unités en livres (tout est en kg).
- Pas de synchronisation entre appareils hors sauvegarde manuelle.
- 250 exercices dans la bibliothèque (extensible avec tes exercices perso), sans illustrations.
