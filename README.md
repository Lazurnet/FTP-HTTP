# Mini serveur Web : exploration du protocole HTTP

L'objectif de ce projet est de comprendre le fonctionnement de la communication entre un client (navigateur) et un serveur Web à travers le protocole HTTP.  
Le serveur est capable de répondre à plusieurs requêtes et de retourner différentes pages HTML.


## 1. Architecture client / serveur

Lorsqu'un utilisateur ouvre une page Web, son navigateur envoie une requête HTTP à un serveur.

Le serveur traite la demande puis renvoie une réponse contenant généralement du HTML.


flowchart LR

A["Navigateur Web<br/>Client"] -->|GET /| B[Serveur Web]

B -->|200 OK<br/>HTML| A

A -->|GET /about| B

B -->|200 OK<br/>Page About| A
