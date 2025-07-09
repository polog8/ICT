# Interactive Content Tool (ICT) v2.0

### Un outil sur mesure pour créer des schémas interactifs

**ICT** est une application web autonome, fonctionnant entièrement côté client, développée pour simplifier le processus de création de cartes d'images interactives et responsives. Elle a été conçue pour surmonter les défis des outils en ligne standards en offrant un flux de travail flexible et efficace, spécifiquement pour l'intégration de diagrammes complexes dans des plateformes de partage de connaissances comme Google Sites.

Cet outil se compose de deux modules principaux : un **Convertisseur de lien Google Drive** et un **Mapper d'Images**.

---

## Fonctionnalités Clés

-   **Support multi-formes :** Dessinez des **rectangles**, **cercles** et **polygones** pour épouser les contours de vos images.
-   **Édition avancée des formes :** Redimensionnez les cercles par leur rayon et ajustez les polygones en déplaçant leurs sommets individuellement.
-   **Gestion des calques :** Contrôlez précisément l'ordre de superposition de vos zones interactives.
-   **Intégration Google Drive :** Convertit les liens de partage Google Drive en URL d'images directes et intégrables.
-   **Canevas Interactif :** Chargez n'importe quelle image via une URL (Google Drive) et dessinez, déplacez et modifiez des zones avec une grande précision.
-   **Snap-to-Grid :** Une fonctionnalité optionnelle d'alignement sur une grille pour positionner parfaitement plusieurs zones.
-   **Éditeur de propriétés :** Assignez facilement un titre (pour les infobulles), un lien hypertexte, une destination (`_blank`, `_top`...) et une couleur d'affichage à chaque zone.
-   **Génération de code automatique :** Obtenez instantanément le code HTML `<map>` et JavaScript complet, propre et responsive, prêt à être intégré dans n'importe quelle page web.
-   **Stockage local et sécurisé :** Toutes vos configurations sont sauvegardées directement dans le `localStorage` de votre navigateur. **<font color="red">Aucune donnée n'est jamais envoyée sur un serveur externe.</font>** L'application fonctionne entièrement en local dans votre navigateur.


---

## Guide d'utilisation

### Module 1: Convertisseur de lien Google Drive

1.  **Obtenir le lien de partage** : Dans votre Google Drive, faites un clic droit sur votre image et obtenez le lien de partage. Assurez-vous que les permissions sont réglées sur "Tous les utilisateurs disposant du lien".
2.  **Coller & Convertir** : Collez le lien (ex: `https://drive.google.com/file/d/FILE_ID/view?usp=sharing`) dans le champ du convertisseur.
3.  **Cliquer sur `Convertir`** : L'outil génère un **lien direct vers l'image** et le place automatiquement dans le champ "URL de l'image à mapper" ci-dessous.

### Module 2: Mapper d'Images Interactif

#### Étape 1: Charger une Image

1.  Utilisez le convertisseur ci-dessus ou collez directement une URL d'image valide dans le champ "URL de l'image à mapper".
2.  Cliquez sur `Charger l'image`. L'image apparaît sur le canevas, prête à être modifiée.

#### Étape 2: Créer et Éditer les Zones

-   **Choisir un outil** : D'abord, sélectionnez votre outil de dessin : **Rectangle**, **Cercle**, ou **Polygone**.
-   **Créer une zone** :
    -   **Rectangle** : Cliquez et faites glisser pour dessiner le rectangle.
    -   **Cercle** : Cliquez pour définir le centre, puis faites glisser pour définir le rayon.
    -   **Polygone** : Cliquez pour placer chaque sommet. Appuyez sur **`Entrée`** pour finaliser la forme.
-   **Sélectionner une zone** : Cliquez simplement à l'intérieur d'une forme existante. Elle sera mise en surbrillance et l'éditeur de propriétés apparaîtra.
-   **Modifier une zone** :
    -   **Déplacer** : Cliquez au centre d'une forme sélectionnée et faites-la glisser.
    -   **Modifier la forme** :
        -   **Rectangle** : Faites glisser l'une des 8 poignées sur les bords et les coins.
        -   **Cercle** : Faites glisser la poignée située sur sa circonférence pour ajuster le rayon.
        -   **Polygone** : Faites glisser n'importe quel sommet (poignée) pour le repositionner.
-   **Gérer l'ordre (Calques)** : Utilisez les flèches ▲ et ▼ dans la table "Liste des zones" pour changer l'ordre de superposition des formes.
-   **Éditer les propriétés** :
    -   **Titre (infobulle)** : Le texte qui apparaîtra au survol. _<font color="green">Astuce: Pour un saut de ligne dans une infobulle, tapez l'élément HTML `<br>` directement dans le champ "Titre".</font>_
    -   **URL du lien** : La destination du clic.
    -   **Cible** : Comment le lien s'ouvre (ex: `_blank` pour un nouvel onglet).
    -   **Couleur** : La couleur de la zone dans l'éditeur (pour l'organisation).



#### Étape 3: Gérer les Configurations (Sauvegarde & Chargement)

-   **Sauvegarder** :
    1.  Cliquez sur `Sauvegarder`.
    2.  Donnez un nom descriptif à votre configuration (ex: `h225_cockpit_schema`).
    3.  Votre configuration est enregistrée et apparaît dans la liste "Configurations sauvegardées".
-   **Charger** :
    1.  Cliquez sur le nom de la configuration souhaitée dans la liste.
    2.  Alternativement, cliquez sur `Charger` et entrez le nom manuellement.
-   **Supprimer** : Cliquez sur le menu à trois points (⋮) à côté d'une configuration et sélectionnez "Supprimer".

#### Étape 4: Utiliser le Code Final

1.  Une fois votre travail terminé, le code complet est généré dans la zone de texte **"Code HTML généré"**.
2.  Cliquez sur `Copier le code`.
3.  Collez ce bloc de code dans un module **"Intégrer" -> "Intégrer le code"** sur votre Google Site, ou dans n'importe quelle page HTML.

---

## Bonnes Pratiques

-   **Soyez Concis** : Gardez le texte de vos infobulles court et pertinent.
-   **Restez Organisé** : Utilisez la fonction **Couleur** pour regrouper visuellement les zones interactives pendant votre travail.
-   **Soyez Précis** : Activez l'option **Snap-to-Grid** pour aligner parfaitement vos zones.
-   **Nommez Clairement** : Utilisez des noms de sauvegarde descriptifs (ex: `H225_ACS_Schema_v1.1`) pour retrouver facilement votre travail.

## Sécurité & Confidentialité des Données

-   **Opération Côté Client** : ICT est une application entièrement client. Tout le traitement se fait dans votre navigateur.
-   **Aucun Stockage en Ligne** : **Aucune donnée d'image ou de configuration n'est jamais envoyée ou stockée sur un serveur externe.** La fonctionnalité "Sauvegarder" utilise le `localStorage` de votre navigateur, un espace de stockage sécurisé et privé sur votre ordinateur.
-   **Conséquence** : Votre travail est confidentiel. Cependant, cela signifie que les configurations ne sont pas synchronisées entre différents ordinateurs ou navigateurs.

## Limitations Connues

-   **Accessibilité de l'image** : L'outil nécessite une URL directe vers un fichier image (.png, .jpg, etc.). Il ne fonctionnera pas avec des pages nécessitant une connexion.
-   **Stockage Local** : Les configurations sauvegardées sont liées au navigateur et à l'ordinateur que vous utilisez.

---

 *Cet outil a été développé par Paul GAUTIER lors d'un stage chez Airbus Helicopters (2025).*


---


# Interactive Content Tool (ICT) v2.0

### A Custom Tool for Creating Interactive Schematics

**ICT** is a standalone, client-side web application developed to streamline the process of creating interactive, responsive image maps. It was designed to solve the challenges of using standard online tools by offering a flexible and efficient workflow, specifically for integrating complex diagrams into knowledge-sharing platforms like Google Sites.

This tool is composed of two main modules: a **Google Drive Link Converter** and an **Image Mapper**.

---

## Key Features

-   **Multi-Shape Support**: Draw complex **rectangles**, **circles**, and **polygons** to match the contours of your images.
-   **Advanced Shape Editing**: Resize circles by their radius and adjust polygons by dragging their individual vertices.
-   **Layer Management**: Precisely control the stacking order of your interactive zones.
-   **Google Drive Integration**: Converts Google Drive sharing links into direct, embeddable image URLs.
-   **Interactive Canvas**: Load any image via URL, then draw, move, and modify zones with high precision.
-   **Snap-to-Grid**: An optional grid-snapping feature to perfectly align multiple zones.
-   **Property Editor**: Easily assign a title (for tooltips), a hyperlink, a target (`_blank`, `_top`...), and a display color to each zone.
-   **Automatic Code Generation**: Instantly get the complete, clean, and responsive HTML `<map>` and JavaScript code, ready for any web page.
-   **Secure, Local Storage**: All your mapping configurations are saved directly in your browser's `localStorage`. **<font color="red">No data is ever sent to an external server.</font>** The application runs entirely locally in your browser.
---

## Usage Guide

### Module 1: Google Drive Link Converter

1.  **Get Share Link**: In your Google Drive, right-click your image and get the shareable link. Ensure permissions are set to "Anyone with the link".
2.  **Paste & Convert**: Paste the link (e.g., `https://drive.google.com/file/d/FILE_ID/view?usp=sharing`) into the converter's input field.
3.  **Click `Convert`**: The tool generates a **direct image URL** and automatically places it in the "Image URL to map" field below.

### Module 2: Interactive Image Mapper

#### Step 1: Loading an Image

1.  Use the converter above or directly paste a valid image URL into the "Image URL to map" field.
2.  Click `Load Image`. The image will appear on the canvas, ready to be mapped.

#### Step 2: Creating and Editing Zones

-   **Choose a Tool**: First, select your drawing tool: **Rectangle**, **Circle**, or **Polygon**.
-   **Create a Zone**:
    -   **Rectangle**: Click and drag to draw the rectangle.
    -   **Circle**: Click to set the center, then drag out to set the radius.
    -   **Polygon**: Click to place each vertex. Press **`Enter`** to finalize the shape.
-   **Select a Zone**: Simply click inside an existing shape. It will be highlighted, and the property editor will appear.
-   **Modify a Zone**:
    -   **Move**: Click and drag a selected shape from its body.
    -   **Edit Shape**:
        -   **Rectangle**: Drag any of the 8 handles on its edges and corners.
        -   **Circle**: Drag the handle on its circumference to adjust the radius.
        -   **Polygon**: Drag any of its vertices (handles) to reposition them.
-   **Manage Order (Layers)**: Use the ▲ and ▼ arrows in the "Zone List" table to change the stacking order of shapes.
-   **Edit Properties**:
    -   **Title (tooltip)**: The text that will appear on hover. *<font color="green">Tip: For a line break, type `<br>` in the "Title" property.</font>*
    -   **Link URL**: The click destination.
    -   **Target**: How the link opens (e.g., `_blank` for a new tab).
    -   **Color**: The zone's color in the editor (for organization).

#### Step 3: Managing Configurations (Save & Load)

-   **To Save**:
    1.  Click `Save`.
    2.  Enter a descriptive name for your configuration (e.g., `h225_cockpit_schema`).
    3.  Your configuration is saved and will appear in the "Saved Configurations" list.
-   **To Load**:
    1.  Click the name of the desired configuration in the list.
    2.  Alternatively, click `Load` and type the name manually.
-   **To Delete**: Click the three-dot menu (⋮) next to a configuration and select "Delete".

#### Step 4: Using the Final Code

1.  Once your work is complete, the final code is automatically generated in the **"Generated HTML Code"** text area.
2.  Click `Copy Code`.
3.  Paste this code block into an **"Embed" -> "Embed code"** module on your Google Site, or into any HTML page.

---

## Best Practices

-   **Be Concise**: Keep your tooltip text short and to the point.
-   **Stay Organized**: Use the **Color** feature to visually group related zones while you work.
-   **Be Precise**: Enable the **Snap-to-Grid** feature to perfectly align your zones.
-   **Name Clearly**: Use descriptive names when saving configurations (e.g., `H225_ACS_Schema_v1.1`) so you can easily find them later.

## Security & Data Privacy

-   **Client-Side Operation**: ICT is a fully client-side application. All processing occurs entirely within your web browser.
-   **No Online Storage**: **No image data or mapping configurations are ever uploaded to or stored on an external server.** The "Save" functionality uses your browser's `localStorage`, which is a secure storage space private to your computer and browser.
-   **Implication**: Your work is confidential. However, this also means that saved configurations are not automatically synced between different computers or browsers.

## Known Limitations

-   **Image Accessibility**: The tool requires a direct URL to an image file (.png, .jpg, etc.). It will not work with pages that require a login.
-   **Local Storage**: Saved configurations are tied to the specific browser and machine you are using.

---

*This tool was developed by Paul GAUTIER during an internship at Airbus Helicopters (2025).*
