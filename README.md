<style>
  .image-avec-ombre {
    box-shadow: 5px 5px 5px 0 rgba(0, 0, 0, 0.2);
  }

.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}

</style>

# Balance_connectée
Encore une balance connectée pour peser nos ruches.
Cette version contrairement à ce que j'ai pu trouvé sur le net est voulu entiérement paramétrable par l'utilisateur sans aucune intervension de reprogrammation du microcontroleur.
Elle peut_être utilisée avec n'importe quel type de pont de mesures puisque le calibrage se fait à partir du site web embarqué.

Pour le moment elle n'est prévue que pour envoyer la masse de la ruche à l'utilisateur par un SMS. Le nombre de SMS par jour et l'heure d'envoi sont paramétrable par l'interface WEB.

Le site web embarqué n'est accessible que proche de la balance et à condition de l'avoir mis en service. En fonctionnement normal le site web est arrété pour des questions de sécurité et d'économie d'énergie.

## Images du serveur web embarqué


![Accueil](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/0_accueil.png)
![Tare](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/1_tare.png)
![Tare](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/1_tare_reponse.png)
![Calibration](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/2_calibration.png)
![Calibration](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/2_calibration_rempli.png)
![Calibration](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/2_calibration_rempli.png)
![Nom ruche](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/3_nom_ruche.png)
![Nom ruche](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/3_nom_ruche_rempli.png)
![Nom ruche](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/3_nom_ruche_reponse.png)
![Config SMS](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/4_config_sms.png)
![Config SMS](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/4_config_sms_rempli.png)
![Config SMS](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/4_config_sms_reponse.png)
![Test SMS](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/5_test_sms.png)
![Test SMS](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/5_test_sms_reponse.png)
![Charge batterie](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/6_charge_batterie.png)
![Mesure Masse](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/7_mesure_masse.png)
![Validation configuration](https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/8_valid_config.png)

## Constitution de la balance

Cette balance est construite autour d'un ESP32 WROOM de chez 

<img width="250" class="center" alt="esp32" src="https://github.com/herve-tourrel/balance_connecte1/assets/144062443/eb6e473b-8eb0-4ec0-bf2f-6bb68e623fc9">

basée sur une carte A7608 de chez Lilygo

 <img width="200" class="center" alt="A7608"  src="https://www.lilygo.cc/cdn/shop/files/LILYGO-DEVELOPMENT-BOARDS_3.jpg?v=1683355413">

Cette carte intégre tout ce qu'il nous faut sauf le convertisseur Analogique Numérique Amplificateur HX711

<img width="200" class="center" alt="A7608"  src="https://github.com/herve-tourrel/balance_connecte1/assets/144062443/3a6e936a-f305-487c-b31a-9b413b0b3f3f">

Au dos de cette carte il ya un support pour la batterie LI-ion 18650, sur le devant :
* un emplacement pour la carte SIM
* le module A7608 comptaible 4G
* un connecteur pour panneau solaire pour recharger la batterie


Pour la commande du composant principal voici le lien direct sur le site du fabricant.
 https://www.lilygo.cc/products/t-a7608e-h?bg_ref=ym9qhdJWHc
