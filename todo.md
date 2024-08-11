## Brainstorming

- [ ] Specification
      --- Partie étude de YOLO
- [x] Quelle version ? V8
- [x] Comment utiliser avec des bounding boxes ?
- [ ] Résoudre le probleme de mise a l'echelle des résolutions

--- Partie etude du dataset

- [ ] Présenter le dataset
      --- Préparation du dataset de football
- [x] Télécharger la lib de hugginfaces/datasets (voir comment)
- [x] Code qui télécharge le dataset sur HF
- [x] Code qui affiche une image de manière random une image avec les boundings boxes
- [x] Code qui prépare le dataset pour le finetuning
  - [x] Autres bonnes pratiques de préparation du dataset (transformations...)
  - [x] Split du dataset en training et validation

--- YOLO setup

- [x] Code qui télécharge yolo
- [x] Code qui charge yolo
- [ ] Parametrage de yolo
- [ ] Code qui freeze yolo la ou il faut

--- Training

- [ ] Préparation de l'entrainement avec Pytorch
- [ ] Code d'entrainement

--- Validation

- [ ] Affichage du resultat
- [ ] Code qui valide
- [ ] Code qui test le modèle finetuné sur une video de football
