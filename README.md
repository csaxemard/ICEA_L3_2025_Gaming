# Coincés sur l'Île

## Concept
Projet Gaming, L3 SDN 2025-2026  
Sophie et Josh sont coincés sur une île mystérieuse.  
Pour s'en échapper ils doivent résoudre les épreuves de l'île en prenant garde au monstre qui les chasse.

<br>

## Contribution

### Tech stack
- Unreal Engine v5.5.4

### Etapes pour démarrer

- Cloner la repo, ajouter les dossiers d'assets au dossier Content
- Lien de téléchargement des dossiers d'assets à ajouter à Content (ils ne devraient pas changer trop souvent) : [Lien google drive](https://drive.google.com/drive/folders/1_4r0SfPOuimYr4dif7mUADnOuMw9D5Rz?usp=sharing)


### Architecture de dossiers
```js
Content/
    _Main/    // Espace de travail principal
        Characters/      // Tout ce qui concerne les personnages
            Bob/
            PlayerInputs/
            BP_Player
        CommonSystems/   // Systèmes divers partagés entre tous les niveaux
            Weapons/
        Core/            // Blueprints qui gèrent la logique et le code des niveaux
            GameInstance
            GM_MainLevel1
            GM_MiniGame1
        Maps/            // Contient tous les levels
            MainLevel/   // Eléments spécifiques aux zones / niveaux (systèmes, environnements, UI, ...)
            MiniGame1/
                Totems/   // Le système de Totems du MiniGame1
                    BP_Platform
                    SM_Platform1
                    SM_Platform2
                    T_Platform2
                    M_Platform
                    BP_Totem
                    BP_TotemSpawner
                    WBP_TotemNumber
            MainLevel.umap
            MiniGame1.umap
        UI/               // Interface
    StarterContent/, etc...  // assets externes
```


<br>

##
Date de départ : 17 novembre 2025
