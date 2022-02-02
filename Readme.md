# Playbook de test AWX

**Il faudra changer les valeurs entre crochets !**

## Construction de l'image

```bash
ansible-builder build --tag=<votre-registry>/my-custom-ee:1.0.0
```

## L'inventaire

Editer le fichier host dans le dossier inventory et ajouter vos machines.

## Le playbook

Ce playbook installer le package kubernetes sur le node ou se trouve le cluster
et récupère la liste des pods en running.