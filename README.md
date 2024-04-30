
# InfoCollector

Aquest script, creat per CyberLab amb Bash, recopila informació detallada sobre un sistema Linux i genera un informe amb les dades extretes.


## Característiques

- Extreu la versió del kernel i la distribució
- Extreu informació de les interfícies de xarxa
- Extreu informació dels discs durs
- Extreu informació del processador
- Extreu informació de la memòria ram
- Extreu informació de la targeta gràfica


## Execució

Execució de l'script:

```bash
  chmod +x InfoCollector.sh
  sudo bash InfoCollector.sh
```
Donem el permís d'execució a l'script. L'**script necessita permisos d'administrador per accedir als detalls d'ús del disc dur**. 
## Screenshots

![App Screenshot](https://i.ibb.co/JznNDDK/Info-Collector2.png)

![App Screenshot](https://i.ibb.co/tDs0Tn0/2024-04-30-18-17.png)


## FAQ

#### Per què demana s'ha d'executar amb sudo?

Per veure la informació sobre els discs durs utilitzem la comanda *fdisk -l*. Aquesta comanda no es pot utilitzar sense permisos d'administrador. 

```
fdisk -l
fdisk: cannot open /dev/nvme0n1: Permission denied
```

#### Com puc utilitzar aquesta eina de manera còmoda?

Et pots connectar a la màquina amb SSH i utilitzar **wget** per descarregar l'script. 

```
wget https://raw.githubusercontent.com/CyberLab-CECETI/InfoCollector/main/InfoCollector.sh
```

#### Com puc extreure l'informe?

Si has executat l'script amb SSH, pots fer un cat del fitxer *informe.txt* i copiar la sortida. Si no, es pot copiar el fitxer amb la comanda scp. 


## Feedback

Si teniu alguna consulta o suggerència podeu enviar un correu a **ceceticyberlab@proton.me**

