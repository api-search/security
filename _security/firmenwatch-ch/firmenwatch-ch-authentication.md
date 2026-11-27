---
anonymous_access: false
api_key_in: []
api_specs:
- filename: firmenwatch-ch-aktionen-api-openapi.yml
  format: yaml
  label: Firmenwatch Aktionen API
  slug: firmenwatch-ch-aktionen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-aktionen-api-openapi.yml
- filename: firmenwatch-ch-betrieb-api-openapi.yml
  format: yaml
  label: Firmenwatch Betrieb API
  slug: firmenwatch-ch-betrieb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-betrieb-api-openapi.yml
- filename: firmenwatch-ch-ereignisse-api-openapi.yml
  format: yaml
  label: Firmenwatch Ereignisse API
  slug: firmenwatch-ch-ereignisse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-ereignisse-api-openapi.yml
- filename: firmenwatch-ch-firmen-api-openapi.yml
  format: yaml
  label: Firmenwatch Firmen API
  slug: firmenwatch-ch-firmen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-firmen-api-openapi.yml
- filename: firmenwatch-ch-identitaet-api-openapi.yml
  format: yaml
  label: Firmenwatch Identitaet API
  slug: firmenwatch-ch-identitaet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-identitaet-api-openapi.yml
- filename: firmenwatch-ch-portfolios-api-openapi.yml
  format: yaml
  label: Firmenwatch Portfolios API
  slug: firmenwatch-ch-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-portfolios-api-openapi.yml
- filename: firmenwatch-ch-uid-api-openapi.yml
  format: yaml
  label: Firmenwatch UID API
  slug: firmenwatch-ch-uid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-uid-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Firmenwatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Firmenwatch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Firmenwatch
provider_slug: firmenwatch-ch
scheme_count: 1
schemes:
- bearerFormat: fw_live_…
  description: 'API-Schluessel als Bearer-Token im Authorization-Kopf. Produktivschluessel beginnen mit fw_live_. Das ist bewusst kein OAuth-Flow: Die unveraenderlichen Rechte werden beim Erstellen des Schluessels vergeben.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/firmenwatch-ch-openapi.json
  type: http
slug: firmenwatch-ch-authentication
source_filename: firmenwatch-ch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/firmenwatch-ch-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: fw_live_…\n  description: 'API-Schluessel als Bearer-Token im Authorization-Kopf. Produktivschluessel beginnen\n    mit fw_live_. Das ist bewusst kein OAuth-Flow: Die unveraenderlichen Rechte werden beim\n    Erstellen des Schluessels vergeben.'\n  sources:\n  - openapi/firmenwatch-ch-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/firmenwatch-ch/authentication/firmenwatch-ch-authentication.yml
summary_line: http · 1 scheme
tags:
- Swiss
- Monitoring
- Commercial-Register
- Alerts
- Business Intelligence
---
