 ##en cours de construction .
 
Pour programmer la balance on pourra utiliser l'outil logiciel de chez Expressif.

Téléchargez le logiciel [Flash Download Tool](https://www.espressif.com/en/support/download/other-tools).

## Programmation :

<script 
  type="module" 
  src="https://unpkg.com/esp-web-tools@9/dist/web/install-button.js?module" 
></script>

 
Pour programmer directement à partir de la page Web[ Lien vers la page de programmation](https://herve-tourrel.github.io/balance_connecte1/flash.html).



 <esp-web-install-button 
  manifest="https://firmware.esphome.io/esphome-web/manifest.json" 
></esp-web-install-button>

## Utilisation d'ESP Web Tools

Bienvenue dans ESP Web Tools ! Vous pouvez accéder à l'outil directement en suivant [ce lien vers la démo en ligne](lien-vers-la-demo). Assurez-vous de consulter les instructions ci-dessous pour savoir comment utiliser l'outil de manière efficace.
Attention je n'ai pas trouvé comment flasher les pages web avec cet outil.


## Utilisation d'ESP Tool

### Instructions

1. Copiez la totalité du dossier test dans un répertoire de votre poste de travail.
2. Ouvrez la page web[ ESP Tool ](https://espressif.github.io/esptool-js/)
3. Connectez votre carte à votre poste de travail
4. Puis appuyez sur connect :                                              ![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/d51613bc-6ea6-45ad-b92c-85ecc871752c)
5. Choisissez le bon port de communication, pour moi ici le 17 :           ![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/2efa2ec0-651b-4e2a-bce9-749b10b1c930)
6. Puis appuyez sur connexion :                                            ![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/da431ba4-56e7-4a82-bbc2-91d04bb4fe29)
7. Vous devez voir dans la console (partie en noir) quelque chose comme ça :![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/9a63b94d-cc95-43c1-ab97-0800107b0a9c)
8. En plus du premier fichier proposeé il faut ajouter 4 autres fichier en cliquant sur le bouton Add File ![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/8d28af4d-b37b-4658-9a69-45b6d61bc9db)
9. Vous devez obtenir ceci, attention à bien remplir la case Flash Adress pour chacuns des fichiers.![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/e08734c8-428b-4b97-ac72-8a9f75df1508)
10. Ensuite vous pouvez appuyer sur le bouton Program à coté de Add File. Vous devriez voir dans la console quelque chose comme ça :![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/4f4d8de0-e4cd-4a33-9b3e-d53b9c0514c7)
11. Une fois la programmation terminée, vous devez vous deconnecter du mode programmation avec le bouton Disconnect : ![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/0ddb7f85-044a-4c4f-adf6-f97fca030f09)
12. Puis maintenant, vous connectez à la console avec le bouton Start : ![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/31ca785a-6e7a-47d5-bdcb-975f687a2b7e)
13. De nouveau choissisez le bon port de communication de votre carte (ici le 17) puis Connexion : ![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/8e771fdc-4c56-4225-bc70-85d7d77e1ebd)
14. Il faut ensuite faire un Reset :![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/ce2a4bfa-072d-4b44-889b-2481a67d11a1)
15. Dans la console maintenant vous devriez voir quelque chose comme ça :![image](https://github.com/herve-tourrel/balance_connecte1/assets/144062443/9aad231a-dc97-4558-8501-fb19595dfca6)







