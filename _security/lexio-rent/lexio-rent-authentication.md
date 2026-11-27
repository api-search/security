---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lexio-rent-catalogue-api-openapi.yml
  format: yaml
  label: Lexio Catalogue API
  slug: lexio-rent-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-catalogue-api-openapi.yml
- filename: lexio-rent-clients-api-openapi.yml
  format: yaml
  label: Lexio Clients API
  slug: lexio-rent-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-clients-api-openapi.yml
- filename: lexio-rent-d-part-et-retour-api-openapi.yml
  format: yaml
  label: Lexio Départ et retour API
  slug: lexio-rent-d-part-et-retour-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-d-part-et-retour-api-openapi.yml
- filename: lexio-rent-entretien-api-openapi.yml
  format: yaml
  label: Lexio Entretien API
  slug: lexio-rent-entretien-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-entretien-api-openapi.yml
- filename: lexio-rent-flotte-api-openapi.yml
  format: yaml
  label: Lexio Flotte API
  slug: lexio-rent-flotte-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-flotte-api-openapi.yml
- filename: lexio-rent-locations-api-openapi.yml
  format: yaml
  label: Lexio Locations API
  slug: lexio-rent-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-locations-api-openapi.yml
- filename: lexio-rent-modifications-api-openapi.yml
  format: yaml
  label: Lexio Modifications API
  slug: lexio-rent-modifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-modifications-api-openapi.yml
- filename: lexio-rent-offre-api-openapi.yml
  format: yaml
  label: Lexio Offre API
  slug: lexio-rent-offre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-offre-api-openapi.yml
- filename: lexio-rent-organisation-api-openapi.yml
  format: yaml
  label: Lexio Organisation API
  slug: lexio-rent-organisation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-organisation-api-openapi.yml
- filename: lexio-rent-paiements-api-openapi.yml
  format: yaml
  label: Lexio Paiements API
  slug: lexio-rent-paiements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-paiements-api-openapi.yml
- filename: lexio-rent-tarification-api-openapi.yml
  format: yaml
  label: Lexio Tarification API
  slug: lexio-rent-tarification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-tarification-api-openapi.yml
- filename: lexio-rent-v-nements-api-openapi.yml
  format: yaml
  label: Lexio Événements API
  slug: lexio-rent-v-nements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexio-rent/openapi/lexio-rent-v-nements-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lexio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lexio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lexio
provider_slug: lexio-rent
scheme_count: 1
schemes:
- bearerFormat: lck_…
  description: 'Clé API `lck_…` créée dans Lexio (Paramètres → Développeur), envoyée en `Authorization: Bearer`. Voir [Authentification](https://docs.lexio.rent/authentification).'
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/lexio-rent-openapi.json
  type: http
slug: lexio-rent-authentication
source_filename: lexio-rent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/lexio-rent-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: lck_…\n  description: 'Clé API `lck_…` créée dans Lexio (Paramètres → Développeur), envoyée en `Authorization:\n    Bearer`. Voir [Authentification](https://docs.lexio.rent/authentification).'\n  sources:\n  - openapi/lexio-rent-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lexio-rent/authentication/lexio-rent-authentication.yml
summary_line: http · 1 scheme
tags:
- Car Rental
- Software-as-a-Service
- Fleet Management
- French
- B2B
---
