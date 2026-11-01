---
anonymous_access: false
api_key_in: []
api_specs:
- filename: intencheck-com-analyze-api-openapi.yml
  format: yaml
  label: intencheck-com Analyze API
  slug: intencheck-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-analyze-api-openapi.yml
- filename: intencheck-com-api-keys-api-openapi.yml
  format: yaml
  label: intencheck-com API Keys API
  slug: intencheck-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-api-keys-api-openapi.yml
- filename: intencheck-com-checkout-api-openapi.yml
  format: yaml
  label: intencheck-com Checkout API
  slug: intencheck-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-checkout-api-openapi.yml
- filename: intencheck-com-demo-api-openapi.yml
  format: yaml
  label: intencheck-com Demo API
  slug: intencheck-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-demo-api-openapi.yml
- filename: intencheck-com-docs-api-openapi.yml
  format: yaml
  label: intencheck-com Docs API
  slug: intencheck-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-docs-api-openapi.yml
- filename: intencheck-com-mcp-api-openapi.yml
  format: yaml
  label: intencheck-com MCP API
  slug: intencheck-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-mcp-api-openapi.yml
- filename: intencheck-com-reply-api-openapi.yml
  format: yaml
  label: intencheck-com Reply API
  slug: intencheck-com-reply-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-reply-api-openapi.yml
- filename: intencheck-com-report-error-api-openapi.yml
  format: yaml
  label: intencheck-com Report Error API
  slug: intencheck-com-report-error-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-report-error-api-openapi.yml
- filename: intencheck-com-transactions-api-openapi.yml
  format: yaml
  label: intencheck-com Transactions API
  slug: intencheck-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-transactions-api-openapi.yml
- filename: intencheck-com-webhooks-api-openapi.yml
  format: yaml
  label: intencheck-com Webhooks API
  slug: intencheck-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Intencheck Com Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: intencheck-com secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: intencheck-com
provider_slug: intencheck-com
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: /api/v1/auth/login
  name: OAuth2PasswordBearer
  sources:
  - openapi/intencheck-com-openapi.json
  type: oauth2
slug: intencheck-com-authentication
source_filename: intencheck-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/intencheck-com-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /api/v1/auth/login\n    scopes: 0\n  sources:\n  - openapi/intencheck-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/intencheck-com/authentication/intencheck-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI
- NLP
- TextAnalysis
- Sentiment
- Emotion
---
