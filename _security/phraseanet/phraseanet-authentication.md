---
api_key_in:
- query
api_specs:
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Records API
  slug: phraseanet-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Databoxes and Collections API
  slug: phraseanet-databoxes-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Metadata API
  slug: phraseanet-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Search API
  slug: phraseanet-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Stories API
  slug: phraseanet-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Baskets API
  slug: phraseanet-baskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Feeds API
  slug: phraseanet-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Account API
  slug: phraseanet-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Phraseanet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Phraseanet secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Phraseanet
provider_slug: phraseanet
scheme_count: 2
schemes:
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  sources:
  - openapi/phraseanet-openapi.yml
  type: oauth2
- description: OAuth2 access token passed as the oauth_token query parameter.
  in: query
  name: oauthTokenParam
  parameter: oauth_token
  sources:
  - openapi/phraseanet-openapi.yml
  type: apiKey
slug: phraseanet-authentication
source_filename: phraseanet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/phraseanet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n    scopes: 0\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n  sources:\n  - openapi/phraseanet-openapi.yml\n- name: oauthTokenParam\n  type: apiKey\n  in: query\n  parameter: oauth_token\n  description: OAuth2 access token passed as the oauth_token query parameter.\n  sources:\n  - openapi/phraseanet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/authentication/phraseanet-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Digital Asset Management
- DAM
- Media
- Metadata
- Open Source
- Search
---
