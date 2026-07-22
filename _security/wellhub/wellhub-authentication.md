---
api_key_in: []
api_specs:
- filename: wellhub-integrations-openapi-original.json
  format: json
  label: Wellhub Integrations API
  slug: wellhub-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellhub/refs/heads/main/openapi/wellhub-integrations-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wellhub Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Wellhub secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Wellhub
provider_slug: wellhub
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token obtained from POST /oauth/token using the client_credentials grant type. Although the OpenAPI declares an http-bearer scheme, the documented mechanism is the OAuth 2.0 client-credentials flow.
  name: OAuth2
  scheme: bearer
  sources:
  - openapi/wellhub-integrations-openapi-original.json
  type: http
slug: wellhub-authentication
source_filename: wellhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wellhub-integrations-openapi-original.json\ndocs: https://developer-hub.wellhub.com/docs/integrations/api/getting-started/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  presented_as: Authorization Bearer JWT\ngrant:\n  flow: client_credentials\n  token_endpoint: https://api.clients.wellhub.com/oauth/token\n  token_request_content_type: application/x-www-form-urlencoded\n  request_fields: [client_id, client_secret, grant_type]\n  token_format: JWT (Bearer)\n  credential_management: Wellhub for Companies portal (clients.wellhub.com) -> Settings -> API OAuth credentials; permissions chosen per product area at creation; secret shown once; expiration configurable.\nschemes:\n- name: OAuth2\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Bearer token obtained from POST /oauth/token using the client_credentials grant type.\n    Although the OpenAPI declares an http-bearer\
  \ scheme, the documented mechanism is the\n    OAuth 2.0 client-credentials flow.\n  sources:\n  - openapi/wellhub-integrations-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellhub/refs/heads/main/authentication/wellhub-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Health
- Wellbeing
- Corporate Benefits
- Fitness
- HR
- Eligibility
- Employee Benefits
---
