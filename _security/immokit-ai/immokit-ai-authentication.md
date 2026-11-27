---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: immokit-ai-bodenrichtwert-api-openapi.yml
  format: yaml
  label: immokit-ai Bodenrichtwert API
  slug: immokit-ai-bodenrichtwert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-bodenrichtwert-api-openapi.yml
- filename: immokit-ai-bodenwert-api-openapi.yml
  format: yaml
  label: immokit-ai Bodenwert API
  slug: immokit-ai-bodenwert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-bodenwert-api-openapi.yml
- filename: immokit-ai-me-api-openapi.yml
  format: yaml
  label: immokit-ai Me API
  slug: immokit-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-me-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: immokit-ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: immokit-ai secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: immokit-ai
provider_slug: immokit-ai
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://bodenrichtwert.ai/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://bodenrichtwert.ai/oauth/token
  name: OAuth2
  sources:
  - openapi/immokit-ai-openapi.json
  type: oauth2
- description: 'Static API key issued in the dashboard (Entwickler → API-Keys). Pass as

    `Authorization: Bearer <key>`. Alternative to the OAuth2 flow above —

    recommended for direct server-to-server integrations that skip the

    interactive OAuth consent screen.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/immokit-ai-openapi.json
  type: http
- description: 'The same API key as `BearerAuth`, passed as `?token=<key>` instead of in a header.


    Intended **only** for clients that cannot set request headers — Google Sheets

    `=IMPORTXML`/`=IMPORTDATA` and comparable spreadsheet importers. Every other client

    should use the `Authorization` header, which takes precedence when both are present.


    A credential in a URL is structurally weaker than one in a header: i'
  in: query
  name: QueryToken
  parameter: token
  sources:
  - openapi/immokit-ai-openapi.json
  type: apiKey
slug: immokit-ai-authentication
source_filename: immokit-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/immokit-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://bodenrichtwert.ai/oauth/authorize\n    tokenUrl: https://bodenrichtwert.ai/oauth/token\n    scopes: 0\n  sources:\n  - openapi/immokit-ai-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Static API key issued in the dashboard (Entwickler → API-Keys). Pass as\n    `Authorization: Bearer <key>`. Alternative to the OAuth2 flow above —\n    recommended for direct server-to-server integrations that skip the\n    interactive OAuth consent screen.\n  sources:\n  - openapi/immokit-ai-openapi.json\n- name: QueryToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: |-\n    The same API key as `BearerAuth`, passed as `?token=<key>`\
  \ instead of in a header.\n\n    Intended **only** for clients that cannot set request headers — Google Sheets\n    `=IMPORTXML`/`=IMPORTDATA` and comparable spreadsheet importers. Every other client\n    should use the `Authorization` header, which takes precedence when both are present.\n\n    A credential in a URL is structurally weaker than one in a header: i\n  sources:\n  - openapi/immokit-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/immokit-ai/authentication/immokit-ai-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
---
