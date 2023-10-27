
# Balance_connectée
Encore une balance connectée pour peser nos ruches.
Cette version contrairement à ce que j'ai pu trouvé sur le net est voulu entiérement paramétrable par l'utilisateur sans aucune intervension de reprogrammation du microcontroleur.
Elle peut_être utilisée avec n'importe quel type de pont de mesures puisque le calibrage se fait à partir du site web embarqué.

Pour le moment elle n'est prévue que pour envoyer la masse de la ruche à l'utilisateur par un SMS. Le nombre de SMS par jour et l'heure d'envoi sont paramétrable par l'interface WEB.

Le site web embarqué n'est accessible que proche de la balance et à condition de l'avoir mis en service. En fonctionnement normal le site web est arrété pour des questions de sécurité et d'économie d'énergie.

## Images du serveur web embarqué

<p align="center">
  <img src="https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/0_accueil.png" alt="Accueil" style="drop-shadow (5px 5px 5px #666666); width: 80%;" />
</p>


## Constitution de la balance
<p align="center">
Cette balance est construite autour d'un ESP32 WROOM de chez 
</p>
<p align="center">
<img width="250" class="center" alt="esp32" src="https://github.com/herve-tourrel/balance_connecte1/assets/144062443/eb6e473b-8eb0-4ec0-bf2f-6bb68e623fc9">
</p>
<p align="center">
basée sur une carte A7608 de chez Lilygo
</p>
<p align="center">
 <img width="200" class="center" alt="A7608"  src="https://www.lilygo.cc/cdn/shop/files/LILYGO-DEVELOPMENT-BOARDS_3.jpg?v=1683355413">
</p>
<p align="center">
Cette carte intégre tout ce qu'il nous faut sauf le convertisseur Analogique Numérique Amplificateur HX711
</p>
<p align="center">
<img width="200" class="center" alt="A7608"  src="https://github.com/herve-tourrel/balance_connecte1/assets/144062443/3a6e936a-f305-487c-b31a-9b413b0b3f3f">
</p>

Au dos de cette carte il ya un support pour la batterie LI-ion 18650 et sur le devant :
* un emplacement pour la carte SIM
* le module A7608 compatible 4G
* un connecteur pour panneau solaire pour recharger la batterie

**Pour la commande du composant principal voici le lien direct sur le site du fabricant:**

<p align="center">
https://www.lilygo.cc/products/t-a7608e-h?bg_ref=ym9qhdJWHc
</p>

**Pour les connecteurs :**

 https://fr.aliexpress.com/item/1005003084329744.html
 
 Il faut prendre la "couleur" : back nut  qui correspond au montage dans un trou de 13mm.
 Il faut ensuite prendre :
 * un 2P pour le panneau solaire extérieur
 * un 3P pour la configuration et l'anti-soulévement ( Attention il faut 2 connecteurs male pour une balance ( un seul suplémentaires pour la configuration de plusieurs balances)
 * un 5P pour la connection aux pont de mesure de masse

**Pour le boitier :**

 https://fr.aliexpress.com/item/1005001304761174.html
 
Boîtier étanche transparent en plastique IP67
 * Taille : with ears
 * Couleur : 200-120-75 (Taille)

**Le prototype :**


**Le schéma du module de pesage :**
<p align="center">
<img width="200" class="center" alt="Schema"  src="https://github.com/herve-tourrel/balance_connecte1/blob/main/Images/Schema_balance.drawio.png">
</p>

