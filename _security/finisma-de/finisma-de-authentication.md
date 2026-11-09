---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finisma-de-konto-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Konto API
  slug: finisma-de-konto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-konto-api-openapi.yml
- filename: finisma-de-kontoausz-ge-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Kontoauszüge API
  slug: finisma-de-kontoausz-ge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-kontoausz-ge-api-openapi.yml
- filename: finisma-de-partner-checks-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Partner Checks API
  slug: finisma-de-partner-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-partner-checks-api-openapi.yml
- filename: finisma-de-rechnungen-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Rechnungen API
  slug: finisma-de-rechnungen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-rechnungen-api-openapi.yml
- filename: finisma-de-selbstauskunft-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Selbstauskunft API
  slug: finisma-de-selbstauskunft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-selbstauskunft-api-openapi.yml
- filename: finisma-de-zahlungsverkehr-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Zahlungsverkehr API
  slug: finisma-de-zahlungsverkehr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-zahlungsverkehr-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Finisma De Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Paulibytes UG (haftungsbeschränkt) secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Paulibytes UG (haftungsbeschränkt)
provider_slug: finisma-de
scheme_count: 2
schemes:
- description: API-Key (fnsm_…) aus dem finisma-Konto unter /konto oder OAuth-Zugriffstoken (fnso_…).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/finisma-de-openapi.json
  type: http
- description: OAuth 2.1 mit PKCE (S256). Clients können sich per Dynamic Client Registration unter /api/oauth/register selbst anmelden.
  flows:
  - authorizationUrl: https://finisma.de/api/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://finisma.de/api/oauth/token
  name: oauth2
  sources:
  - openapi/finisma-de-openapi.json
  type: oauth2
slug: finisma-de-authentication
source_filename: finisma-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/finisma-de-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API-Key (fnsm_…) aus dem finisma-Konto unter /konto oder OAuth-Zugriffstoken\n    (fnso_…).\n  sources:\n  - openapi/finisma-de-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://finisma.de/api/oauth/authorize\n    tokenUrl: https://finisma.de/api/oauth/token\n    scopes: 2\n  description: OAuth 2.1 mit PKCE (S256). Clients können sich per Dynamic Client Registration\n    unter /api/oauth/register selbst anmelden.\n  sources:\n  - openapi/finisma-de-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/finisma-de/authentication/finisma-de-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- FinTech
- Invoice
- PDF
- ZUGFeRD
- API
---
