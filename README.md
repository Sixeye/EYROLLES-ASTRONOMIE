# EYROLLES-ASTRONOMIE

LIBRAIRIE EYROLLES <br/>
Une application simple pour utiliser les paiements Stripe et gérer un panier avec SYMFONY 5.
La base de donnnées est sqlite pour aller vite à l'essentiel. <br/>
<br/>
Avant de commencer:<br/>

Placez vous dans le dossier EYROLLES-ASTRONOMIE<br/>
<br/>
créez un fichier .env <br/>
dans le .env mettez ceci: <br/>
<br/>
DATABASE_URL=sqlite:///%kernel.project_dir%/data.db<br/>
dièse Stripe <br/>
STRIPE_PUBLIC_KEY=<br/>
STRIPE_PRIVATE_KEY=<br/>
<br/>
aussi créez un fichier .env.local dans la racine du projet et insérez-y ceci:<br/>
<br/>
dièse Stripe <br/>
STRIPE_PUBLIC_KEY=votre_public_key_ici_colle_a_egal <br/>
STRIPE_PRIVATE_KEY=votre_private_key_ici_colle_a_egal <br/>
<br/>
En ligne de commande dans le terminal tapez:<br/>
composer install<br/>
symfony server:start<br/>
<br/>
<br/>
<br/>
Pour le faux paiement, comme nous l'avons vu, il vous faudra vos clefs de test de Stripe à renseigner.
Ensuite quand le paiement est lancé utilisez la fausse cartes de crédit 4242 4242 4242 4242   02/25 (date dans le futur)
123 (csv) et un lieu en France, un mail avec un "@", un nom et nous sommes bons.
<br/>
__________________________________<br/>
<br/>
Si vous voulez l'adapter à votre (autre) application, essayez de respecter la version de stripe indiquée dans le
composer.json (on ne sait jamais si d'une version à l'autre ça ne marche plus). 
