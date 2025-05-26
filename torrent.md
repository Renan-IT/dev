# Torrents

## 1. Installation de qBittorrent

- Téléchargez qBittorrent sur le site officiel : [qBittorrent](https://www.qbittorrent.org/)
- Lancez l'installation et suivez les instructions.

## 2. Configuration du port

- Ouvrez qBittorrent > `Outils` > `Options` > `Connexion`.
- Choisissez un port manuel entre 49160 et 65534.

## 3. Bloquer le port dans le pare-feu Windows

- Ouvrez `Panneau de configuration` > `Système et sécurité` > `Pare-feu Windows Defender` > `Paramètres avancés`.
- Créez une nouvelle règle pour bloquer le port TCP configuré.
- Appliquez la règle à tous les profils (Domaine, Privé, Public).
- Nommez la règle (ex. "Bloquer qBittorrent") et validez.

## 4. Supprimer le tracker YggTorrent d’un torrent

- Dans qBittorrent, faites clic droit sur le torrent > `Propriétés` > onglet `Trackers`.
- Sélectionnez le tracker YggTorrent et supprimez-le.
- Répétez pour chaque torrent YggTorrent pour protéger votre ratio.

## 5. Installer et utiliser Ratio Master

- Téléchargez Ratio Master sur GitHub : [Ratio Master GitHub](https://github.com/NikolayIT/RatioMaster.NET)
- Extrayez et lancez-le.
- Dans votre client torrent, commencez le téléchargement du torrent.
- Dans Ratio Master, sélectionnez le torrent et votre client.
- Activez `Memory Reader` dans `Advanced`.
- Cochez `Upload Speed Randomization` (150-180 KB/s toutes les 30 min).
- Réglez la vitesse d’upload à 1 MB/s, puis cliquez sur `Start`.
- Surveillez votre ratio, ne dépassez pas 2.
- Ne laissez pas Ratio Master uploader trop longtemps pour éviter la détection.
