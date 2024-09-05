# Carte de Visite NFC (VCARD) - Instructions

### 1. Achat de la carte NFC
Achetez des cartes NFC sur Amazon via ce lien : [Lien Amazon](https://amzn.to/3TlecVY).

### 2. Créer une fiche contact sur iPhone ou Mac
#### iPhone :
- Ouvrez l’app *Contacts* et créez votre fiche.
- Une fois la fiche créée, allez tout en bas de la fiche et sélectionnez "Partager cette fiche".
- Sélectionnez les champs à inclure dans votre carte de visite, puis cliquez sur "OK".
- Enregistrez la fiche dans *Fichiers* en cliquant sur "Enregistrer dans Fichiers".

#### Mac :
- Ouvrez l’app *Contacts* et créez votre fiche.
- Allez dans le menu *Fichier*, puis sélectionnez *Exporter* > *Exporter vCard*.

Cela va créer un fichier **prenom_nom.vcf**.

### 3. Hébergement du fichier vCard
- Accédez au gestionnaire de fichiers de votre hébergeur (via *cPanel* ou *FTP*).
- Créez un dossier nommé **vcard** dans le répertoire racine de votre hébergement, idéalement dans le dossier *public_html*.
- Importez le fichier **.vcf** dans ce dossier. Renommez-le sans accents ni espaces.

Exemple : 
```
mon_domaine.fr/vcard/prenom_nom.vcf
```

### 4. Encoder la carte NFC
- Ouvrez l’app *NFC Tools* sur votre iPhone : [Lien iOS NFC Tools](https://apps.apple.com/fr/app/nfc-tools/id1252962749).
- Sélectionnez "Écrire", puis "Ajouter un enregistrement".
- Choisissez "URL/URI", puis collez le lien du fichier vCard hébergé, par exemple :
```
mon_domaine.fr/vcard/prenom_nom.vcf
```
- Cliquez sur "OK", puis sur "Écrire".
- Approchez la carte NFC vierge de votre iPhone pour l’encoder.

### 5. Tester la carte
Une fois la carte NFC encodée, testez-la pour vous assurer que la vCard se charge correctement.
