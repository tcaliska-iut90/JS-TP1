# IHM - JavaScript - TP1

* Exercice 1 : IMC
* Développer une page web qui calcule l'indice de masse corporelle : 𝐼𝑀𝐶 = 𝑚𝑎𝑠𝑠𝑒 𝑒𝑛 𝑘𝑔 / (𝑡𝑎𝑖𝑙𝑙𝑒 𝑒𝑛 𝑚)²
* La page web doit contenir 2 champs de texte pour insérer la masse et la taille d'un individu, un bouton pour déclencher le calcul de l'indice et l'afficher dans la page web.
* Pour gérer l'évènement « appuyer sur le bouton » définissez la fonction JavaScript à exécuter lors d'un événement « onclick ».
* La fonction JavaScript doit récupérer le contenu des champs de texte avec la méthode "document.getElementById("identifiant_du_champs").value" puis calculer l'IMC et l'afficher sur la page web.
* Ajouter au script une instruction conditionnelle qui selon la valeur de IMC affiche l'information correspondante :
* IMC État de l'individu :
* | moins de 18,5 maigre                          |
* | entre 18,5 et 25 normal chez un adulte        |
* | entre 25 et 30 surpoids (surcharge pondérale) |
* | entre 30 et 35 obésité                        |
* | entre 35 et 40 obésité sévère                 |
* 
* Ajouter un raccourci (Ctrl+C) au bouton « Calculer » en utilisant le code suivant :
* var isCtrl = false;
* document.onkeyup=function(e){
* if(e.key === 'Control')
* isCtrl=false;
* }
* document.onkeydown=function(e){
* if(e.key === 'Control') isCtrl=true;
* if(e.key === 'c' && isCtrl == true) {
* calculer();
* }}
*
* Ajouter un script qui permet d'afficher le message « appuyer sur le bouton pour calculer
l'IMC » à coté du bouton lorsque la souris est au-dessus du bouton et disparaît lorsque la
souris est ailleurs. (style.display = 'none';)
Le même effet peut être créer en ajoutant tout simplement un titre au bouton.
<input type="button" title="appuyer sur le boutton pour calculer" … >
• Ajouter à la fonction de calcul de l'IMC des fonctions qui testent si les données insérées
dans les 2 champs de texte sont valides : les champs ne sont pas vides, ils contiennent des
chiffres (isNaN(n)) et ils sont positifs. 
Vos messages d'erreurs doivent être affichés dans une petite fenêtre (alert(message)). Ils
doivent être clairs et indiquer explicitement c'est quoi l'erreur d'insertion et dans quel
champ de texte elle s'est produite.
