---
api_key_in: []
auth_types:
- connection-string
description: ''
kind: authentication
layout: security
method: searched
name: Postgresml Authentication
name_suffix: Authentication
oauth_flows: []
overview: PostgresML secures its APIs with connection-string across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PostgresML
provider_slug: postgresml
scheme_count: 1
schemes:
- docs: https://postgresml.org/docs
  format: postgresql://user:password@host:port/database
  name: postgres-connection-string
  notes: No API keys, bearer tokens or OAuth. Access control and TLS are handled at the Postgres/PgCat layer; PostgresML Cloud provisions per-database credentials.
  secret: KORVUS_DATABASE_URL / DATABASE_URL
  transport: postgres-wire-protocol
  type: connection-string
slug: postgresml-authentication
source_filename: postgresml-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/postgresml/korvus + https://postgresml.org/docs\nnotes: >-\n  PostgresML exposes no REST/HTTP API and therefore no OpenAPI securitySchemes.\n  Authentication is Postgres-native: clients authenticate with a PostgreSQL\n  connection string (DATABASE_URL) that carries the username, password and host\n  of a self-hosted Postgres (with the pgml + pgvector extensions) or a managed\n  PostgresML Cloud database. The Korvus SDK reads this from the\n  KORVUS_DATABASE_URL environment variable.\nsummary:\n  types: [connection-string]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: postgres-connection-string\n  type: connection-string\n  transport: postgres-wire-protocol\n  secret: KORVUS_DATABASE_URL / DATABASE_URL\n  format: \"postgresql://user:password@host:port/database\"\n  docs: https://postgresml.org/docs\n  notes: >-\n    No API keys, bearer tokens or OAuth. Access control and TLS are handled at\n   \
  \ the Postgres/PgCat layer; PostgresML Cloud provisions per-database\n    credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postgresml/refs/heads/main/authentication/postgresml-authentication.yml
summary_line: connection-string · 1 scheme
tags:
- Company
- Ai Ml
- Machine Learning
- Vector Search
- Embeddings
- PostgreSQL
- RAG
- LLM
- Database
---
