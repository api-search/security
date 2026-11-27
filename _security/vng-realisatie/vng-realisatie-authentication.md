---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vng-realisatie-autorisaties-openapi.yml
  format: yaml
  label: VNG Realisatie Autorisaties API
  slug: vng-realisatie-autorisaties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-autorisaties-openapi.yml
- filename: vng-realisatie-besluiten-openapi.yml
  format: yaml
  label: VNG Realisatie Besluiten API
  slug: vng-realisatie-besluiten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-besluiten-openapi.yml
- filename: vng-realisatie-catalogi-openapi.yml
  format: yaml
  label: VNG Realisatie Catalogi API
  slug: vng-realisatie-catalogi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-catalogi-openapi.yml
- filename: vng-realisatie-documenten-openapi.yml
  format: yaml
  label: VNG Realisatie Documenten API
  slug: vng-realisatie-documenten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-documenten-openapi.yml
- filename: vng-realisatie-klantinteracties-openapi.yml
  format: yaml
  label: VNG Realisatie Klantinteracties
  slug: vng-realisatie-klantinteracties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-klantinteracties-openapi.yml
- filename: vng-realisatie-notificaties-openapi.yml
  format: yaml
  label: VNG Realisatie Notification API
  slug: vng-realisatie-notificaties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-notificaties-openapi.yml
- filename: vng-realisatie-referentielijsten-openapi.yml
  format: yaml
  label: VNG Realisatie Referentielijsten & Selectielijst API
  slug: vng-realisatie-referentielijsten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-referentielijsten-openapi.yml
- filename: vng-realisatie-woz-bevragen-openapi.yml
  format: yaml
  label: VNG Realisatie BG IMWOZ WOZ
  slug: vng-realisatie-woz-bevragen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-woz-bevragen-openapi.yml
- filename: vng-realisatie-zaken-openapi.yml
  format: yaml
  label: VNG Realisatie Zaken API
  slug: vng-realisatie-zaken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-zaken-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: VNG Realisatie Authentication
name_suffix: Authentication
oauth_flows: []
overview: VNG Realisatie secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VNG Realisatie
provider_slug: vng-realisatie
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: JWT-Claims
  scheme: bearer
  sources:
  - openapi/vng-realisatie-autorisaties-openapi.yml
  - openapi/vng-realisatie-besluiten-openapi.yml
  - openapi/vng-realisatie-catalogi-openapi.yml
  - openapi/vng-realisatie-documenten-openapi.yml
  - openapi/vng-realisatie-notificaties-openapi.yml
  - openapi/vng-realisatie-zaken-openapi.yml
  type: http
slug: vng-realisatie-authentication
source_filename: vng-realisatie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource:\n- https://vng-realisatie.github.io/gemma-zaken/themas/achtergronddocumentatie/authenticatie-autorisatie\n- https://vng-realisatie.github.io/gemma-zaken/ontwikkelaars/handleidingen-en-tutorials/api-guides\n- openapi/vng-realisatie-autorisaties-openapi.yml, openapi/vng-realisatie-besluiten-openapi.yml, openapi/vng-realisatie-catalogi-openapi.yml,\n  openapi/vng-realisatie-documenten-openapi.yml, openapi/vng-realisatie-notificaties-openapi.yml, openapi/vng-realisatie-zaken-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT-Claims\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/vng-realisatie-autorisaties-openapi.yml\n  - openapi/vng-realisatie-besluiten-openapi.yml\n  - openapi/vng-realisatie-catalogi-openapi.yml\n  - openapi/vng-realisatie-documenten-openapi.yml\n  - openapi/vng-realisatie-notificaties-openapi.yml\n  - openapi/vng-realisatie-zaken-openapi.yml\ndocs: https://vng-realisatie.github.io/gemma-zaken/themas/achtergronddocumentatie/authenticatie-autorisatie\n\
  flow: 'Applications register out-of-band with a provider and receive a client_id and secret; they sign a JWT (shared secret,\n  HMAC) carrying client_id, sent as \"Authorization: Bearer <JWT>\". The provider validates the JWT and queries the Autorisaties\n  API (AC) for that client_id''s authorisations; failures return HTTP 403. User authentication is out of scope and left to\n  the municipality.'\ntoken_tool: https://github.com/VNG-Realisatie/token-issuer\nnotes:\n- 'Docs: \"JWT kunnen niet gerevoked worden - daarom is het wenselijk om een korte expiry toe te kennen (bijvoorbeeld 24h).\"'\n- Klantinteracties, WOZ-bevragen and Referentielijsten specs declare no securitySchemes.\n"
source_yaml_url: https://artifacts.apis.io/vng-realisatie/authentication/vng-realisatie-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Government
- Municipalities
- Netherlands
- API Standards
- Common Ground
- Open Standard
- Public Sector
---
