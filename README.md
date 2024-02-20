Pour exécuter le site web en local, suivre ces étapes: 
1 Récupérer le code de l'appli : Download le zip depuis le repository Git
https://github.com/Avo400/GarageTest 

2.Copier-coller ce dossier dans un nouveau répertoire : C:\Temp\MEP_PourGarageDeAvo\GarageTest-main

3.Démarrer les 2 services MySQL (Wampapache64 et Wampmysqld64) via services Windows

4. Dans une fenêtre commande line (qu'on abrègera en "cmd"), 
taper la commande: cd C:\Temp\MEP_PourGarageDeAvo\GarageTest-main

5. Ensuite, taper : C:\Temp\MEP_PourGarageDeAvo\GarageTest-main>mysql -u root -p
mysql> source RestoreBDD_TableParTable.sql;
Cela va restaurer la bdd depuis le fichier "RestoreBDD_TableParTable.sql".

6.Ouvrir un nouveau cmd et taper : cd C:\Temp\MEP_PourGarageDeAvo\GarageTest-main. Puis taper: code .

7. Les étapes 8 à 12 doivent être réalisées dans un nouveau terminal qu'on crée dans l'IDE VSCode au chemin d'accès suivant: C:\Temp\MEP_PourGarageDeAvo\GarageTest-main

8. Taper la commande suivante afin d'installer composer : C:\Temp\MEP_PourGarageDeAvo\GarageTest-main> composer install

9. Installer les librairies JS: C:\Temp\MEP_PourGarageDeAvo\GarageTest-main> npm install --force

10.Compiler les librairies js:  : C:\Temp\MEP_PourGarageDeAvo\GarageTest-main> npm run build

11. Démarrer le server interne Symfony : C:\Temp\MEP_PourGarageDeAvo\GarageTest-main> symfony server:start

12. Récupérer l'URL fournie par le résultat de l'étape 9 qui a pour préfixe "http://localhost" et la coller dans un navigateur web.





