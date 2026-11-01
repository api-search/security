---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Jaikin Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: jaikin-eu declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: jaikin-eu
provider_slug: jaikin-eu
scheme_count: 2
schemes:
- description: Clé d'API utilisée pour authentifier les requêtes. Mentionnée comme méthode d'authentification sur la page API du glossaire.
  in: header
  name: API-Key
  type: apiKey
- description: Jeton OAuth mentionné comme alternative à la clé d'API. Aucun détail supplémentaire fourni sur le flux ou les scopes.
  flow: implicit
  type: oauth2
slug: jaikin-eu-authentication
source_filename: jaikin-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://www.jaikin.eu/glossaire/api\nschemes:\n  - type: apiKey\n    name: API-Key\n    in: header\n    description: \"Clé d'API utilisée pour authentifier les requêtes. Mentionnée comme méthode d'authentification sur la page API du glossaire.\"\n  - type: oauth2\n    flow: implicit\n    description: \"Jeton OAuth mentionné comme alternative à la clé d'API. Aucun détail supplémentaire fourni sur le flux ou les scopes.\"\n"
source_yaml_url: https://artifacts.apis.io/jaikin-eu/authentication/jaikin-eu-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Odoo
- Custom-Software
- Consulting
- France
---
