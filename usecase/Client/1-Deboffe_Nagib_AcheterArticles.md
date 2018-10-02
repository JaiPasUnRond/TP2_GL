# Acheter des articles

## Description
Le caissier enregistre les achats du client.

## Pré-requis
- Un client avec des articles à acheter
- Un caissier identifié
- Une BD produit

## Post-requis
- Un client qui repart avec ses articles payés et son ticket de caisse

## Acteurs concernés
- Client
- Caissier
- BD Produit

## Glossaire
- Panier
- Article
- Montant partiel
- Montant total
- Ticket de caisse
- Code barre
- Scanner
- Mode de paiement

## Intéractions

- Client : Dit bonjour.
- Caisse : Réponds bonjour.
- Système : crée un nouveau panier.

- Pour chaque article :
- Caissier : Présente l'article.
- Système  : Lit le code barre, vérifie l'existence du produit dans la BD Produit,
		   signale si l'article existe bien puis l'ajoute au panier,
		   affiche le montant partiel.
- Caissier : Annonce le montant total au client.
- Système  : présente les choix du mode de paiement.
- Caissier : choisi le mode de paiement.
- Client   : paie.
- Système  : enregistre le paiement, sort le ticket de caisse.
- Caissier : prend le ticket et le donne au client. 
