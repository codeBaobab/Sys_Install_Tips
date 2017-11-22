# Commandes de base
## Nettoyage
### Paquets obsolètes (inaccessibles)
```bash
sudo aptitude autoclean
```
### Paquets anciens encore accessibles (ex: kernels)
```bash
sudo apt-get autoremove
```
### Installation avortée
1. Reconfigurer tous les paquets :
```bash
sudo dpkg --configure -a
```
2. Si 1. insuffisant, alors purger :

+   + seulement le ou les paquets problébatiques :
```bash
sudo dpkg -P <paquet1> <paquet2>
```
+   + ou **tous** les paquets incomplètement installés :
```bash
sudo dpkg -P -a
```

