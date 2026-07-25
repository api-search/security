---
api_key_in:
- query
api_specs:
- filename: zapier-accounts-api-openapi.yml
  format: yaml
  label: Zapier Accounts API
  slug: zapier-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-accounts-api-openapi.yml
- filename: zapier-actions-api-openapi.yml
  format: yaml
  label: Zapier Actions API
  slug: zapier-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-actions-api-openapi.yml
- filename: zapier-apps-api-openapi.yml
  format: yaml
  label: Zapier Apps API
  slug: zapier-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-apps-api-openapi.yml
- filename: zapier-authentications-api-openapi.yml
  format: yaml
  label: Zapier Authentications API
  slug: zapier-authentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-authentications-api-openapi.yml
- filename: zapier-categories-api-openapi.yml
  format: yaml
  label: Zapier Categories API
  slug: zapier-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-categories-api-openapi.yml
- filename: zapier-experimental-api-openapi.yml
  format: yaml
  label: Zapier Experimental API
  slug: zapier-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-experimental-api-openapi.yml
- filename: zapier-inputs-api-openapi.yml
  format: yaml
  label: Zapier Inputs API
  slug: zapier-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-inputs-api-openapi.yml
- filename: zapier-outputs-api-openapi.yml
  format: yaml
  label: Zapier Outputs API
  slug: zapier-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-outputs-api-openapi.yml
- filename: zapier-zap-templates-api-openapi.yml
  format: yaml
  label: Zapier Zap Templates API
  slug: zapier-zap-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-zap-templates-api-openapi.yml
- filename: zapier-zaps-api-openapi.yml
  format: yaml
  label: Zapier Zaps API
  slug: zapier-zaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-zaps-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zapier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Zapier secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Zapier
provider_slug: zapier
scheme_count: 2
schemes:
- description: See our authentication documentation for how to find your Client ID
  in: query
  name: ClientIDAuthentication
  parameter: client_id
  sources:
  - openapi/zapier-partner-api.yml
  type: apiKey
- description: 'See our OAuth2 authentication documentation here: https://docs.zapier.com/powered-by-zapier/api-reference/authentication'
  flows:
  - authorizationUrl: https://zapier.com/oauth/authorize/
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://zapier.com/oauth/token/
  - authorizationUrl: https://zapier.com/oauth/authorize/
    flow: implicit
    scopes: 8
  name: OAuth
  sources:
  - openapi/zapier-partner-api.yml
  type: oauth2
slug: zapier-authentication
source_filename: zapier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zapier-partner-api.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: ClientIDAuthentication\n  type: apiKey\n  in: query\n  parameter: client_id\n  description: See our authentication documentation for how to find your Client ID\n  sources:\n  - openapi/zapier-partner-api.yml\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://zapier.com/oauth/authorize/\n    tokenUrl: https://zapier.com/oauth/token/\n    scopes: 8\n  - flow: implicit\n    authorizationUrl: https://zapier.com/oauth/authorize/\n    scopes: 8\n  description: 'See our OAuth2 authentication documentation here: https://docs.zapier.com/powered-by-zapier/api-reference/authentication'\n  sources:\n  - openapi/zapier-partner-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/authentication/zapier-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Integrations
- iPaaS
---
