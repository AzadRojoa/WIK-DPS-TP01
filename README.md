Azad Rojoa

- Consignes:

  Mettre en place son environnement de développement et les bases du projet avec le moins de dépendances possibles.

  Développer une API qui retourne au format JSON les headers de la requête quand il y une requête HTTP GET sur /ping.

  Le serveur doit écouter sur un port configurable via la variable d'environnement : PING_LISTEN_PORT.

  Réponse vide avec code 404 si quoi que ça soit d'autre que GET /ping ou code 500 si erreur inconnue.

  Réalisation d'un README avec documentation sur le lancement du projet.

- Lancement du programme:

  Cargo run

  Changement de port: export PING_LISTEN_PORT= (numero du port)

- Tester le programme :

  Terminal : curl http://127.0.0.1:8080/ping

  Navigateur: http://127.0.0.1:8080/ping

- Fonctionnement:

  Une route "Ping" qui montre tous les headers en format JSON.

  Toutes les autres routes renvoit une erreur 404.

- Technos:

  Rust
  Actix
  Serde
