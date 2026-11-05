# NIKO ANALOG 37 — Studio Niko

**Synthétiseur virtuel et station de production techno (v1.1).**

> Le dépôt conserve son nom historique **N8V**, mais son contenu sur la branche **main** est maintenant l'application NIKO ANALOG 37. L'ancien projet expérimental de codec n'est plus dans les fichiers actuels de cette branche ; l'historique Git reste conservé.

## Ouvrir l'application

Ouvrir `index.html` dans Chrome, Edge ou Firefox, ou publier le dossier sur un hébergement statique HTTPS (GitHub Pages, Vercel, etc.). Sur Android, le navigateur doit permettre l'activation audio après une interaction utilisateur.

## Modules

- Synthèse numérique Web Audio inspirée de l'architecture d'un synthétiseur analogique : deux oscillateurs, sub-oscillateur, bruit, filtre résonant, enveloppes, LFO et saturation.
- Clavier virtuel 37 notes, contrôle tactile et clavier d'ordinateur.
- Arpégiateur principal et séquenceur mélodique de 64 pas.
- Boîte à rythmes 8 instruments × 16 pas : kick, snare, clap, hats, tom, rim et ride.
- **DRUMS ONLY** pour jouer la batterie seule ; **TEST 8 SONS** pour vérifier les pistes ; **RESET BATTERIE** pour restaurer un rythme.
- Basse indépendante avec séquenceur et deuxième arpégiateur.
- Mixeur trois bus, filtres, égalisation 3 bandes et effets.
- Enregistrement du mix et export WAV stéréo 16 bits ; import/export de presets JSON.

## Démarrage et dépannage audio

1. Cliquer sur **ACTIVER AUDIO**.
2. Pour contrôler la batterie, cliquer sur **TEST 8 SONS**, puis **DRUMS ONLY**.
3. Si le son est absent, cliquer sur **RESET BATTERIE**, vérifier le volume du bus batterie, le volume média et la sortie Bluetooth/casque.
4. Pour jouer tous les instruments, utiliser **PLAY**.
5. Cliquer sur **REC WAV**, puis sur **FIN REC** pour télécharger le mix.

Sur mobile, éviter les prévisualiseurs de fichiers qui bloquent parfois Web Audio. Préférer l'ouverture depuis un site HTTPS.

## Installation PWA

L'application contient `manifest.webmanifest`, `service-worker.js` et des icônes. Elle peut être servie depuis un site HTTPS. Une fois GitHub Pages activé pour la branche **main** et le dossier **/**, la page devrait être accessible à l'adresse `https://nikoju1977.github.io/N8V/`, sous réserve du déploiement. L'installation dépend du navigateur et de son support PWA.

## Portée des tests

La version v1.1 a été testée dans Chromium pour la lecture, la séquence de batterie, les tests des 8 instruments et la production d'un WAV non silencieux. **Aucune validation sur le téléphone réel de l'utilisateur n'est revendiquée.**

## Attribution

Création : **Studio Niko**. Projet indépendant, non affilié à Moog Music. Inspiré par l'ergonomie et l'architecture de synthétiseurs analogiques, **sans reproduction identique des circuits analogiques ni du produit commercial Moog Subsequent 37**.

## Code source

https://github.com/Nikoju1977/N8V
