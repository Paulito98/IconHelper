# IconHelper

Ce plugin est un outil conçu pour les **développeur**, il permet dans des tablines de panel d'avoir les icons des objets/Véhicules grace à l'id que vous entrez.

## Exemple : 
Déjà , mettez le .dll en **dépendance** , ensuite le using : 
```
using Icon98Helper;
```

```
UIPanel panel = new UIPanel("Test", UIPanel.PanelType.TabPrice);
```

```
panel.AddTabLine("Nom de la tabline", "Le prix (ne mettez rien pour aucun chiffre sur la tabline", IconHelper.GetIconIDByID(1), ui => { }); // exemple pour affiché l'icon id 1.
```

```
panel.AddTabLine("Nom de la tabline", "Le prix (ne mettez rien pour aucun chiffre sur la tabline", IconHelper.GetVehicleIconID(0), ui => { }); // exemple pour affiché le véhicule id 1.
```

## Attention ! 
Le panel doit être un **tabprice** pour pouvoir affiché les icons !
