<div align="center">

# 📁 Fichiers 6b

### L'explorateur de fichiers Android **100 % sans publicité**

**🚫 Aucune publicité · 🚫 Aucun pistage · 🚫 Aucun compte à créer · 🚫 Aucun abonnement**

Gratuit, complet et respectueux de votre vie privée — édité par [6bernova](https://www.6bernova.fun)

### 👉 [Télécharger Fichiers 6b](https://github.com/alexter13/fichiers-6b/releases/latest/download/Fichiers6b.apk) 👈

*Lien direct, toujours la dernière version (actuellement **2.0.1**) · Android 8.0 ou plus récent · 7,7 Mo · [toutes les versions](https://github.com/alexter13/fichiers-6b/releases)*

</div>

---

## 🆕 Nouveautés de la version 2.0.1

Corrections de la sauvegarde du téléphone, trouvées en revérifiant la 2.0 de bout en bout :

- 🕒 **Dates d'origine restaurées sur tous les serveurs**, y compris WebDAV / Nextcloud (qui datent les fichiers du jour de l'envoi) : la sauvegarde contient désormais la liste des dates d'origine
- 📏 **Taille de la sauvegarde exacte** dans le bandeau « Restaurer » (la 2.0 affichait la taille envoyée lors de la dernière sauvegarde) ; **l'espace libre est vérifié avant de commencer**, en ne comptant que ce qui manque sur le téléphone
- 🧩 Un fichier refusé par le serveur n'empêche plus la sauvegarde d'être restaurable (le nombre de fichiers non envoyés est indiqué)
- ⏹️ Google Drive et WebDAV : « Arrêter » est immédiat et ne laisse plus de fichier tronqué sur la destination
- 🔐 Coffre-fort ou configuration momentanément illisibles : les photos et documents sont sauvegardés quand même, et la configuration de la sauvegarde n'est jamais remplacée par une version vide
- 📱 Android 12 et plus : l'assistant Google de copie vers un nouveau téléphone ne transfère plus les données de l'appli (mots de passe liés au téléphone, illisibles ailleurs) ; passez par la sauvegarde ou par « Changer de téléphone »

### Version 2.0

- 💾 **Sauvegarde complète du téléphone** (Accueil → *Sauvegarde du téléphone*) vers **Google Drive**, votre NAS (SMB), un serveur SFTP / FTPS ou WebDAV (Nextcloud...) : dossiers choisis (appareil photo, images, documents, enregistrements, WhatsApp...), **connexions, favoris et réglages**, **coffre-fort**. Configuration et coffre partent **chiffrés par votre mot de passe** (AES-256)
- 🔁 **Seules les nouveautés sont envoyées**, automatiquement chaque jour ou chaque semaine (en Wi-Fi, pendant la charge si vous le souhaitez), ou à la demande. Rien n'est jamais effacé de la sauvegarde
- 📲 **Restauration sur un autre téléphone** : ouvrez le dossier de la sauvegarde dans Fichiers 6b, un bandeau **« Restaurer »** apparaît. Chaque fichier retrouve son dossier et **sa date d'origine** (galerie dans le bon ordre) ; rien de ce qui est déjà sur le téléphone n'est écrasé ; connexions et coffre-fort sont réimportés avec le mot de passe
- 🕒 **Dates conservées en SMB et FTPS** : les fichiers envoyés vers un NAS ou un serveur FTPS (sauvegardes automatiques comprises) gardent désormais leur date de modification
- ☁️ Google Drive : si l'autorisation expire (7 jours tant que l'appli est en test chez Google), la sauvegarde se met en pause et repart d'elle-même dès que vous touchez « Renouveler »

### Version 1.9

- 📄 **PDF vraiment nettoyés avant partage** (« Partager sans métadonnées ») : le fichier est réécrit, ce qui atteint aussi les informations rangées dans les parties compressées. Sont retirés : titre, auteur, sujet, mots-clés, logiciels, dates, champs personnalisés (société...), **toutes les métadonnées XMP**, données privées des logiciels de mise en page (Illustrator, Photoshop...), **auteurs des commentaires et surlignages** (remplacés par « Auteur ») ; l'identifiant interne du fichier est renouvelé. Texte, pages, champs de formulaire et pièces jointes sont conservés
- 📷 **Photos intégrées aux PDF** (applis de numérisation, exports d'images) : position GPS, appareil, numéros de série et dates de prise de vue retirés de chaque photo, **sans recompression**
- 🔒 **PDF protégé par mot de passe** : il n'est jamais envoyé sans avoir été nettoyé ; un message explique pourquoi et propose le partage normal si vous le souhaitez
- 📦 **Toutes les versions sur la page [Releases](https://github.com/alexter13/fichiers-6b/releases)** : notes, APK et empreinte de chaque version. L'appli y télécharge ses mises à jour, avec repli automatique sur le dépôt si la page est indisponible ; lien « Toutes les versions » dans *À propos*
- 🧪 **Qualité** : plus de 325 vérifications automatiques contre de vrais serveurs (SMB, SFTP, FTPS, WebDAV, SNMP, DNS, MQTT...) et sur des fichiers de référence contrôlés par des outils indépendants (exiftool, qpdf, pdfinfo, LibreOffice, 7-Zip), plus des tests de l'interface
- ℹ️ *À propos* : liens cliquables et liste complète des composants libres utilisés

### Version 1.8

- 🛡️ **Audit de sécurité du réseau local** (depuis la découverte du réseau) : Telnet et FTP en clair, FTP anonyme, **SMBv1**, signature SMB non exigée, **partages accessibles sans mot de passe** (et modifiables), SNMP « public », bureau à distance sans NLA, VNC, Redis, MQTT, Elasticsearch et API Docker sans authentification, TLS 1.0/1.1, certificats expirés, SHA-1 ou RSA 1024. Gravité, correction proposée et **rapport partageable**. Vérifications en lecture seule, sans essai de mot de passe
- 🧰 **Outils réseau de terrain** : ping, test de ports avec bannières, **DNS** (A, AAAA, MX, TXT, NS, CNAME, PTR, SRV, CAA, sur le serveur de votre choix), **informations Wi-Fi** (canal, signal, norme, sécurité, réseaux voisins et canal le moins encombré), **réveil à distance des PC** (Wake-on-LAN)
- 📍 **Partager sans métadonnées** : position GPS, appareil, numéro de série, dates et auteur retirés des photos (JPEG, PNG, WebP, HEIC) **sans recompression**, auteur, société et auteurs des commentaires retirés des documents Word, Excel, PowerPoint, LibreOffice et PDF. L'original reste intact
- 🔍 **Analyse d'un APK avant installation** : éditeur et certificat de signature, autorisations sensibles, capacités à risque (accessibilité, administrateur, lecture des SMS...), **alerte si la signature diffère de l'appli déjà installée** (contrefaçon), comparaison avec l'empreinte publiée par l'éditeur
- 📱 **Changer de téléphone** : connexions, favoris, réglages, sauvegardes auto, **coffre-fort** (chiffrés) et dossiers choisis (photos, documents, WhatsApp...) transférés par QR code ; sur le nouveau téléphone chaque fichier retrouve son dossier et sa date, les fichiers déjà présents sont ignorés
- 🧹 **Rangement automatique** : règles simples (dossier, type, ancienneté, nom) pour trier les Téléchargements par type, envoyer à la corbeille les vieilles captures d'écran ou APK, etc. Aperçu avant de lancer, exécution quotidienne en option, rien n'est supprimé définitivement
- ⚡ **Raccourcis** : tuiles des réglages rapides (Partage Wi-Fi, Recevoir par QR, Coffre-fort) et raccourcis par appui long sur l'icône
- ☁️ **Google Drive** : l'expiration de l'autorisation (7 jours tant que l'appli est en test chez Google) est détectée ; une notification et un bouton « Renouveler » relancent les sauvegardes en un geste
- ✅ L'empreinte d'un fichier est vérifiée automatiquement si vous avez copié celle publiée par l'éditeur

### Version 1.7

- 📲 **Envoyer des fichiers d'un téléphone à l'autre par QR code** : sélectionnez, l'écran affiche un QR code, l'autre téléphone le scanne et reçoit tout par le Wi-Fi, sans Internet, sans compte et sans câble. Fonctionne aussi vers un **iPhone** ou un téléphone sans l'appli (une page de téléchargement s'ouvre, avec un bouton « Tout télécharger »)
- 🗜️ **Parcourir les 7z, RAR et TAR comme un dossier** : ouvrir une photo ou un document sans tout extraire (7z, RAR, TAR, TAR.GZ, TAR.BZ2, TAR.XZ, GZ, BZ2, XZ)
- 📦 **RAR 5 et RAR 7 pris en charge** (format par défaut de WinRAR depuis des années), y compris les archives à mot de passe et à noms chiffrés
- 🗜️ **Créer des archives 7z et TAR.GZ** en plus du ZIP (compatibles 7-Zip, WinRAR, macOS et Linux ; noms accentués conservés)
- 🧹 **Libérer de l'espace après la sauvegarde automatique** (option) : les photos déjà sauvegardées depuis plus de 30, 90, 180 ou 365 jours sont retirées du téléphone, **uniquement après vérification sur le serveur** (même taille, fichier inchangé depuis l'envoi)

### Version 1.6

- 🎬 **Vidéos et musiques du NAS lues en continu** (SMB, SFTP, FTPS, WebDAV, Google Drive, coffre-fort) : lecture immédiate et avance rapide, sans télécharger le fichier
- 🖼️ **Miniatures des photos du NAS, de Nextcloud ou du serveur SFTP**, gardées en cache (150 Mo max)
- ✏️ **Modifier un fichier du serveur avec Word, Excel ou toute autre appli** : à votre retour, Fichiers 6b propose de renvoyer la nouvelle version (sans jamais écraser une version modifiée entre-temps sur le serveur)
- 📂 **Accès à `Android/data` et `Android/obb` sans root** grâce à Shizuku (sauvegardes de jeux, fichiers d'applications)
- 📡 **Détection du réseau local améliorée** : noms des PC et NAS (NetBIOS et Bonjour/mDNS), box identifiée, type d'appareil reconnu (NAS, Proxmox, PC Windows, Mac, imprimante, serveur Linux...), accès direct à l'interface d'administration, balayage beaucoup plus rapide
- 🔋 **Sauvegardes fiables sur Xiaomi, Huawei, Samsung, Oppo, Vivo** : détection de l'économie de batterie et accès direct aux bons réglages
- 🧾 **Journal d'erreurs local** : en cas de problème, le rapport reste sur le téléphone ; vous le lisez et décidez de l'envoyer ou non

### Version 1.5

- 💾 **Sauvegarde automatique** de vos photos et documents vers votre **NAS, Nextcloud, serveur SFTP ou Google Drive** : en Wi-Fi seulement, en charge si vous voulez, toutes les 1 à 24 h ; seuls les fichiers nouveaux ou modifiés partent, rien n'est supprimé sur le serveur
- 🧹 **Nettoyeur** : dossiers vides, caches de miniatures, fichiers temporaires, APK déjà installés, vieux téléchargements — avec aperçu avant suppression
- 📲 **Changement de téléphone facilité** : export de toute la configuration (connexions, favoris, réglages, sauvegardes) dans un fichier chiffré
- 🔐 **Sauvegarde du coffre-fort** en ZIP AES-256 et **restauration** en un geste (« Extraire dans le coffre-fort »)
- 🕶️ **Confidentialité renforcée** : photos, vidéos et musiques du coffre (ou d'un serveur) lues **dans l'appli**, copies déchiffrées effacées dès que vous la quittez, noms de fichiers masqués dans les notifications de l'écran verrouillé
- 📶 Partage Wi-Fi et découverte réseau fonctionnent aussi quand le téléphone sert de **point d'accès**

### Version 1.4 — sécurité renforcée

- 🔐 **Coffre-fort chiffré** (AES-256-GCM) déverrouillé par empreinte, visage ou code
- 🔑 **Verrouillage de l'application** et **mots de passe protégés par biométrie**
- 🧾 **Vérification de l'identité des serveurs** (empreinte SSH, certificat TLS FTPS/WebDAV) avec alerte en cas de changement
- ☁️ **WebDAV** : Nextcloud, kDrive, pCloud, NAS
- 📡 **Découverte du réseau** et liste des partages SMB, **partage Wi-Fi vers PC**
- 🗜️ **7z, RAR, TAR.GZ/BZ2/XZ** + protection contre les archives piégées
- 📊 **Analyse du stockage** en carte, **lecteurs PDF et audio/vidéo** intégrés
- 🦠 Vérification **VirusTotal**, **mode confidentiel**, mises à jour **vérifiées** (SHA-256 + signature)

---

## 🚫 Zéro publicité, zéro pistage — vraiment

La plupart des explorateurs de fichiers gratuits du Play Store se financent par la publicité : bannières, vidéos plein écran, fenêtres surgissantes, et souvent des traqueurs qui analysent votre utilisation.

**Fichiers 6b n'en contient aucun :**

- ❌ **Aucune publicité** : ni bannière, ni vidéo, ni pop-up, ni « version Pro » pour les retirer
- ❌ **Aucun traqueur ni statistique** : aucune bibliothèque d'analyse (Google Analytics, Firebase, Facebook SDK…) n'est intégrée
- ❌ **Aucun compte** à créer, aucune inscription, aucun e-mail demandé
- ❌ **Aucun abonnement**, aucun achat intégré, aucune fonction bloquée
- ✅ **Vos fichiers restent sur votre téléphone** : l'application ne communique qu'avec les serveurs que **vous** configurez (Google Drive, NAS, serveur SFTP…)

---

## 📥 Installation

1. Sur le téléphone, touchez **[Télécharger Fichiers 6b](https://github.com/alexter13/fichiers-6b/releases/latest/download/Fichiers6b.apk)** : le fichier `Fichiers6b.apk` se télécharge.
2. Ouvrez le fichier téléchargé (notification ou dossier **Téléchargements**).
3. Si Android le demande, autorisez votre navigateur à **installer des applications inconnues**, puis revenez en arrière et touchez **Installer**.
4. Si **Google Play Protect** affiche un avertissement (normal pour une application hors Play Store) : touchez **Plus de détails** → **Installer quand même**.
5. Au premier lancement, touchez **Accorder l'accès** puis activez **Accès à tous les fichiers**. Cette autorisation est indispensable à tout explorateur de fichiers sur Android 11 et plus.

#### 🔄 Mises à jour automatiques

Inutile de revenir sur cette page : quand une nouvelle version est publiée, **l'application vous prévient elle-même** (« Mise à jour disponible ») et l'installe en un geste. Vos réglages, connexions et favoris sont conservés.

---

## ✨ Fonctionnalités

### 🏠 Accueil
- Espace utilisé et libre de chaque stockage (interne, carte SD, clé USB)
- Catégories avec compteurs : **Images, Vidéos, Audio, Documents, Archives, APK, Applications, Téléchargements, Corbeille**
- Accès rapide aux dossiers courants et à vos favoris, fichiers récents en vignettes

### 📂 Navigation
- Stockage interne, **carte SD**, **clé USB OTG** et racine du système
- **Onglets** multiples et **double volet** (deux dossiers côte à côte)
- Affichage **liste ou grille**, **miniatures** des photos, vidéos et applications
- Tri par nom (tri naturel : fichier2 avant fichier10), taille, date ou type
- Fichiers cachés, filtre instantané, favoris, **raccourcis de dossiers sur l'écran d'accueil**

### 🛠️ Gestion des fichiers
- **Copier, couper, coller, renommer, supprimer**, sélection multiple
- **Renommage en lot** (numérotation, rechercher / remplacer, aperçu)
- **Corbeille** : les fichiers supprimés sont restaurables
- Gestion des doublons à la copie : remplacer, ignorer ou garder les deux
- Copies longues en arrière-plan avec barre de progression et notification

### 📄 Fichiers et outils
- **Éditeur de texte** intégré (txt, log, json, xml, scripts…) avec recherche
- **Visionneuse d'images** : balayage, zoom au pincement
- **Propriétés** détaillées : taille, droits, emplacement
- **Empreintes MD5, SHA-1, SHA-256, SHA-512** calculées en une lecture, comparées automatiquement à l'empreinte copiée (vérifier un téléchargement)
- **Partager sans métadonnées** (GPS, appareil, auteur...) : photos, documents Office et PDF
- **Analyse d'un APK** : signataire, autorisations sensibles, cohérence avec l'appli installée
- **Recherche** dans tous les sous-dossiers, avec jokers `*` `?` et recherche dans le contenu des fichiers texte
- **Gros fichiers** : les 200 fichiers qui prennent le plus de place
- **Doublons** : détection des fichiers identiques pour libérer de l'espace
- **Applications installées** : sauvegarder l'APK, partager, désinstaller

### 🗜️ Archives
- **ZIP, 7z, RAR (de RAR 1.5 à RAR 7, RAR 5 compris), TAR, TAR.GZ / TGZ, TAR.BZ2, TAR.XZ, GZ, BZ2, XZ** : extraction ici ou dans un sous-dossier
- **Parcourir toutes ces archives comme un dossier** et ouvrir un fichier sans tout extraire ; ZIP, 7z et RAR **protégés par mot de passe**
- Créer un **ZIP** (avec **mot de passe AES-256** en option), un **7z** (meilleure compression) ou un **TAR.GZ**
- **Protection contre les archives piégées** : chemins `../` et liens symboliques bloqués, arrêt automatique des « bombes de décompression » (taux de compression anormal, espace disque insuffisant, nombre d'entrées excessif)

### 🎬 Lecteurs intégrés
- **Lecteur PDF** (défilement continu, zoom)
- **Lecteur audio et vidéo** (liste de lecture avec les autres médias du dossier)

### ☁️ Cloud et réseau
- **Google Drive** : Mon Drive, Partagés avec moi, Drives partagés ; les Google Docs / Sheets / Slides s'ouvrent en Word / Excel / PowerPoint
- **WebDAV** : **Nextcloud, ownCloud, kDrive (Infomaniak), pCloud, Koofr, NAS Synology / QNAP**
- **SMB** : partages Windows et NAS (Synology, QNAP…)
- **SFTP** (SSH) : mot de passe ou clé privée
- **FTPS / FTP**
- **Découverte du réseau** : détection automatique des NAS et serveurs du Wi-Fi (SMB, SFTP, FTP, WebDAV) et **liste des partages** d'un serveur, connexion pré-remplie en un geste
- **Audit de sécurité** des appareils détectés (une vingtaine de vérifications, rapport Markdown à partager ou enregistrer)
- **Outils réseau** : ping, ports, DNS, Wi-Fi, réveil à distance
- **Envoi vers un téléphone par QR code** : le destinataire scanne et reçoit les fichiers par le Wi-Fi (avec Fichiers 6b : dossier « Téléchargements/Fichiers 6b reçus » ; sans l'appli ou sur iPhone : page de téléchargement). Adresse secrète à usage unique (jeton 128 bits), seuls les fichiers choisis sont visibles, arrêt automatique après 15 min d'inactivité
- **Partage Wi-Fi vers PC** : récupérez (et déposez) des fichiers du téléphone depuis le navigateur d'un ordinateur, sans câble ni logiciel
- Copier et déplacer **entre tous les emplacements** : téléphone ↔ Drive ↔ Nextcloud ↔ NAS ↔ serveur

### 💾 Sauvegarde automatique
- Choisissez un dossier (Appareil photo, Captures d'écran, Documents, Téléchargements ou n'importe quel dossier) et une destination (NAS SMB, SFTP, FTPS, WebDAV/Nextcloud, Google Drive)
- Fréquence de 1 à 24 h, **Wi-Fi uniquement** et **en charge uniquement** en option, batterie faible respectée
- Envoi **incrémental** (seuls les nouveaux fichiers ou modifiés), écriture sous nom temporaire puis renommage : jamais de fichier tronqué sur le serveur
- **Aucune suppression sur le serveur** ; bilan affiché après chaque passage
- **Libérer de l'espace** (option désactivée par défaut, confirmation demandée) : retire du téléphone les fichiers sauvegardés depuis plus de 30, 90, 180 ou 365 jours, seulement s'ils sont inchangés depuis l'envoi et présents sur le serveur avec la même taille (vérifié juste avant ; au moindre doute, le fichier est gardé)

### 🧹 Nettoyeur
- Dossiers vides, caches de miniatures (`.thumbnails`), fichiers temporaires et téléchargements interrompus, verrous Office, `Thumbs.db`
- APK dont l'application est déjà installée, anciens gros téléchargements (à vérifier, non cochés par défaut)
- Aperçu détaillé avant de nettoyer ; APK et téléchargements passent par la corbeille

### 📲 Transfert et sauvegarde
- **Export de la configuration** (connexions avec mots de passe, favoris, réglages, sauvegardes automatiques) dans un fichier `.f6b` chiffré **AES-256-GCM** (clé dérivée du mot de passe par PBKDF2, 600 000 itérations)
- **Sauvegarde du coffre-fort** en ZIP chiffré AES-256, restauration directe dans le coffre
- **Changer de téléphone** : tout transférer vers le nouveau téléphone par QR code (configuration et coffre chiffrés, fichiers remis à leur place)
- **Sauvegarde du téléphone** vers Google Drive, NAS ou serveur (incrémentale, automatique ou à la demande) et **restauration** sur n'importe quel téléphone
- **Rangement automatique** par règles (tri par type, déplacement, corbeille des fichiers anciens)

### 📂 Android/data et Android/obb (Shizuku)
- Depuis Android 11, ces dossiers sont interdits à tous les explorateurs ; avec l'application gratuite **Shizuku** (démarrée par le débogage sans fil, sans root), Fichiers 6b peut les parcourir, copier et modifier
- Parcours guidé : installation, démarrage, autorisation

### 📊 Analyse du stockage
- **Carte proportionnelle** (treemap) : chaque dossier est un rectangle à la taille de ce qu'il occupe ; touchez pour descendre dans l'arborescence

### 🎨 Personnalisation
- Thème clair, sombre ou automatique, **6 couleurs d'accent**, couleurs Material You
- **Noir pur AMOLED** pour économiser la batterie, affichage compact

### 🔗 Intégration Android
- Sert de **sélecteur de fichiers** pour les autres applications
- Reçoit les fichiers **partagés** depuis n'importe quelle application
- **Tuiles des réglages rapides** et **raccourcis** de l'icône (Recevoir par QR, Partage Wi-Fi, Coffre-fort, Outils réseau)

---

## ☁️ Google Drive — accès sur invitation

La connexion à Google Drive est réservée aux comptes Gmail autorisés par l'éditeur (application en phase de test auprès de Google). **Demandez l'ajout de votre adresse Gmail à 6bernova.**

À la première connexion, Google affiche « Google n'a pas validé cette application » : touchez **Continuer**. Toutes les autres fonctions marchent sans aucune inscription.

Tant que l'application est en test chez Google, **l'autorisation expire au bout de 7 jours**. Fichiers 6b vous prévient la veille, met les sauvegardes Drive en pause si elle a expiré et propose **« Renouveler »** (accueil ou notification) : un geste suffit, les sauvegardes reprennent aussitôt.

---

## 🔒 Confidentialité et sécurité

- **Aucune donnée collectée**, aucune statistique, aucun traqueur, aucune publicité
- 🔐 **Coffre-fort chiffré** : vos fichiers sensibles chiffrés en **AES-256-GCM** (noms compris), invisibles de la galerie, des autres applications et d'un PC branché en USB ; ouverture par empreinte, visage ou code
- 🔑 **Verrouillage de l'application** par biométrie ou code de l'appareil, avec délai de reverrouillage réglable
- 🛡️ **Mots de passe des connexions** chiffrés (AES-256) par le Keystore matériel d'Android, et en option **déchiffrables uniquement après authentification biométrique**
- 🕶️ **Mode confidentiel** : pas de capture d'écran, aperçu masqué dans les applications récentes
- 🧾 **Identité des serveurs vérifiée** : empreinte de la clé SSH et du certificat TLS (FTPS, WebDAV) présentée à la première connexion ; alerte rouge et connexion bloquée si elle change (protection contre l'interception)
- ⚠️ Avertissement clair pour les protocoles non chiffrés (FTP, WebDAV en http://)
- 🧾 **Journal d'erreurs 100 % local** : aucun envoi automatique, le rapport n'est transmis que si vous le décidez, après l'avoir lu
- 🦠 **Vérification VirusTotal** : seule l'empreinte SHA-256 du fichier est consultée, le fichier n'est jamais envoyé
- 📦 **Mises à jour vérifiées** : empreinte SHA-256 et certificat de signature contrôlés avant chaque installation
- Google Drive : connexion officielle via les services Google ; aucun mot de passe ne transite par l'application

> ⚠️ Le coffre-fort est stocké dans l'espace privé de l'application : **désinstaller l'application ou effacer ses données détruit définitivement le coffre**. Faites régulièrement une *sauvegarde du coffre-fort* (Réglages) et gardez-la hors du téléphone.

---

## ❓ Questions fréquentes

**C'est vraiment gratuit ?** Oui, sans publicité ni achat intégré, et ça le restera.

**Pourquoi « Accès à tous les fichiers » ?** C'est l'autorisation qu'Android exige pour qu'un explorateur puisse gérer tous vos dossiers. Sans elle, l'application ne verrait que ses propres fichiers.

**Pourquoi ce n'est pas sur le Play Store ?** L'application est distribuée directement par son éditeur. Les mises à jour sont intégrées à l'application.

**Puis-je voir le dossier `Android/data` ?** Android le réserve au système depuis la version 11, pour tous les explorateurs. Fichiers 6b y accède quand même grâce à Shizuku (voir ci-dessous), sans rooter le téléphone.

**Comment changer de téléphone ?** Deux façons. Les deux téléphones côte à côte : sur l'ancien, Accueil → *Changer de téléphone* ; sur le nouveau, *Recevoir (QR)* et scannez le code (même Wi-Fi, sans Internet). Ou à distance : *Sauvegarde du téléphone* vers Google Drive ou votre NAS, puis sur le nouveau téléphone ouvrez le dossier de la sauvegarde et touchez « Restaurer ». Dans les deux cas, chaque fichier retrouve son dossier et sa date.

**La sauvegarde du téléphone remplace-t-elle celle de Google ?** Non, elle la complète : Android ne permet à aucune application de copier les données internes des autres applis (conversations, SMS, contacts). La sauvegarde Google du téléphone s'en charge ; Fichiers 6b sauvegarde vos fichiers (photos, documents, médias WhatsApp...), ses propres réglages et le coffre-fort, là où vous le choisissez.

**Où trouver une ancienne version ?** Sur la page [Releases](https://github.com/alexter13/fichiers-6b/releases) : chaque version y garde son APK, ses notes et son empreinte.

**Pourquoi un PDF n'est-il pas partagé « sans métadonnées » ?** Il est protégé par un mot de passe ou chiffré : ses informations ne peuvent pas être retirées sans le mot de passe du propriétaire. Plutôt que de l'envoyer tel quel à votre insu, l'appli refuse et vous laisse choisir le partage normal.

**Comment accéder à Android/data ?** Installez Shizuku, démarrez-le (Options pour les développeurs → Débogage sans fil, l'appli Shizuku guide), puis dans Fichiers 6b : menu → *Android/data (Shizuku)*. À refaire après chaque redémarrage du téléphone (limite d'Android).

**Les sauvegardes ne partent pas sur mon Xiaomi / Samsung ?** Ouvrez *Sauvegarde automatique* : un encadré indique si l'économie de batterie bloque l'appli et ouvre directement le bon réglage.

**La sauvegarde automatique supprime-t-elle quelque chose ?** Jamais : elle ne fait qu'ajouter ou mettre à jour des fichiers sur la destination.

**Le partage Wi-Fi est-il sûr ?** Il n'est accessible que depuis votre réseau local, protégé par un mot de passe aléatoire renouvelé à chaque démarrage, et s'arrête seul après 30 minutes d'inactivité. Le trafic n'étant pas chiffré, ne l'utilisez pas sur un Wi-Fi public.

**Mes RAR ne s'ouvrent pas ?** Depuis la 1.7, tous les formats RAR sont lus (RAR 1.5 à RAR 7). Seule exception : les archives créées avec un dictionnaire géant (option WinRAR 7 de plus d'1 Go) dépassent la mémoire d'un téléphone ; un message l'indique clairement.

**Pourquoi l'appli peut demander la « Position » ?** Uniquement dans Outils réseau > Wi-Fi, si vous voulez voir le nom du réseau connecté : Android le cache sans cette autorisation. Elle n'est jamais demandée ailleurs et aucune position n'est enregistrée. La liste des réseaux voisins utilise, depuis Android 13, l'autorisation « Appareils à proximité » déclarée sans localisation.

**L'audit de sécurité est-il risqué pour mes appareils ?** Non : il ne fait que des lectures (bannières, négociations de protocole, accès invité ou anonyme, communautés SNMP par défaut) et n'essaie aucun mot de passe. N'auditez qu'un réseau qui vous appartient ou pour lequel vous avez une autorisation.

**Pourquoi l'appli demande l'accès à l'appareil photo ?** Uniquement pour scanner le QR code d'un envoi entre téléphones, au moment où vous appuyez sur « Scanner ». Le scanner est intégré (ZXing) : il fonctionne hors ligne et n'utilise pas les services Google.

---

## ✅ Vérifier l'authenticité

- Empreinte SHA-256 de l'APK 2.0.1 : `d563de61b34e444444d3104ba606957ead5c10af151a883b635a3c69be0e0a86` (aussi affichée sur la page de la [version 2.0.1](https://github.com/alexter13/fichiers-6b/releases/tag/v2.0.1))
- Certificat de signature (SHA-256) : `B6:B9:3D:81:05:8F:BD:C4:00:4D:05:87:8E:6F:0D:35:37:89:C4:AC:6B:03:FF:9D:89:2B:C4:0D:95:5E:FB:EB`

<div align="center">

**Fichiers 6b** · © 2026 [6bernova](https://www.6bernova.fun) · Fait en France 🇫🇷 · **Sans publicité, pour de vrai.**

</div>
