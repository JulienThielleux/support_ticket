# support_ticket

Ce projet met en œuvre un système de RAG en utilisant Google Cloud Platform et des bases de données vectorielles. L'objectif principal est d'expérimenter les workflows RAG sur GCP.

Un dataset contenant des descriptions d'incidents informatiques sert de base.
Toutes les entrées du dataset sont converties en représentations vectorielles à l'aide d'un modèle d'embedding.
Les embeddings sont stockés dans une base de données vectorielle hébergée sur GCP.

Des requêtes sont envoyées à la base de données vectorielle pour trouver les 5 occurrences les plus proches en termes de similarité dans l'espace vectoriel.
Ce genre d'outil pourrait permettre à une équipe de maintenance d'optimiser la recherche d'incidents similaires.