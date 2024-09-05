# Carte de Visite NFC (VCARD) - Instructions

### 1. Achat de la carte NFC
Achetez des cartes NFC via ce lien : [Lien Amazon](https://amzn.to/3TlecVY).

### 2. Créer une fiche contact sur iPhone ou Mac
#### iPhone :
- Ouvrez l’app *Contacts* et créez votre fiche.
- Descendez tout en bas de la fiche et sélectionnez "Partager cette fiche".
- Choisissez les champs à inclure dans la carte de visite, puis cliquez sur "OK".
- Enregistrez la fiche dans *Fichiers* en cliquant sur "Enregistrer dans Fichiers".

#### Mac :
- Ouvrez l’app *Contacts* et créez votre fiche.
- Allez dans le menu *Fichier*, puis sélectionnez *Exporter* > *Exporter vCard*.

Cela va créer un fichier **prenom_nom.vcf**.

### 3. Hébergement du fichier vCard
- Accédez à votre gestionnaire de fichiers (via *cPanel* ou *FTP*).
- Créez un dossier nommé **vcard** dans le répertoire racine de votre hébergement, idéalement dans le dossier *public_html*.
- Importez le fichier **.vcf** dans ce dossier. Assurez-vous de renommer le fichier sans accents ni espaces.

L’adresse du fichier ressemblera à :
```
mon_domaine.fr/vcard/prenom_nom.vcf
```

C'est ce lien que vous devrez copier pour l'étape suivante.

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
Testez ensuite la carte NFC pour vérifier que la vCard s’affiche correctement.
