---
anonymous_access: false
api_key_in: []
api_specs:
- filename: temoinpublic-fr-dater-api-openapi.yml
  format: yaml
  label: Témoin public Dater API
  slug: temoinpublic-fr-dater-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temoinpublic-fr/openapi/temoinpublic-fr-dater-api-openapi.yml
- filename: temoinpublic-fr-lire-api-openapi.yml
  format: yaml
  label: Témoin public Lire API
  slug: temoinpublic-fr-lire-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temoinpublic-fr/openapi/temoinpublic-fr-lire-api-openapi.yml
- filename: temoinpublic-fr-registre-api-openapi.yml
  format: yaml
  label: Témoin public Registre API
  slug: temoinpublic-fr-registre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temoinpublic-fr/openapi/temoinpublic-fr-registre-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Témoin public Authentication
name_suffix: Authentication
oauth_flows: []
overview: Témoin public secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Témoin public
provider_slug: temoinpublic-fr
scheme_count: 1
schemes:
- description: Le jeton rendu à l’inscription du flux
  name: jetonDuFlux
  scheme: bearer
  sources:
  - openapi/temoinpublic-fr-openapi.json
  type: http
slug: temoinpublic-fr-authentication
source_filename: temoinpublic-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/temoinpublic-fr-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: jetonDuFlux\n  type: http\n  scheme: bearer\n  description: Le jeton rendu à l’inscription du flux\n  sources:\n  - openapi/temoinpublic-fr-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/temoinpublic-fr/authentication/temoinpublic-fr-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
