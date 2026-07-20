---
api_key_in:
- header
auth_types:
- http
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Agentuity Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Agentuity secures its APIs with http, apiKey, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Agentuity
provider_slug: agentuity
scheme_count: 4
schemes:
- description: 'Most REST API requests require a Bearer token. Pass an API key or SDK key in the Authorization header as `Authorization: Bearer [example key]`. The SDK key is found in the Agentuity Console under project settings and is read from the AGENTUITY_SDK_KEY environment variable by the SDK service clients.'
  env: AGENTUITY_SDK_KEY
  format: Bearer <api_key|sdk_key>
  header: Authorization
  name: bearerToken
  scheme: bearer
  type: http
- description: Project- and organization-scoped API keys (prefix ak_) created and managed via the API Keys API and the CLI. Presented as bearer tokens.
  docs: https://agentuity.dev/reference/api/api-keys
  id_prefix: ak_
  in: header
  name: apiKeys
  type: apiKey
- description: OAuth 2.0 / OIDC applications with client credentials, user consent, and authorization scopes, managed via the OAuth Applications API. Enables "Sign in with Agentuity".
  docs: https://agentuity.dev/reference/api/oauth
  name: oauthApplications
  type: oauth2
- description: Agentuity OIDC provider — add Agentuity account sign-in and scoped access to your app with OAuth 2.0 and OIDC ("Sign in with Agentuity").
  docs: https://agentuity.dev/services/oidc-provider
  name: agentuityOIDC
  type: openIdConnect
slug: agentuity-authentication
source_filename: agentuity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://agentuity.dev/reference/api/ai-gateway.md\ndocs: https://agentuity.dev/services/authentication\nsummary:\n  types: [http, apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  primary: bearer-token\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Most REST API requests require a Bearer token. Pass an API key or SDK key in the\n    Authorization header as `Authorization: Bearer [example key]`. The SDK key is found in\n    the Agentuity Console under project settings and is read from the AGENTUITY_SDK_KEY\n    environment variable by the SDK service clients.\n  header: Authorization\n  format: \"Bearer <api_key|sdk_key>\"\n  env: AGENTUITY_SDK_KEY\n- name: apiKeys\n  type: apiKey\n  in: header\n  description: >-\n    Project- and organization-scoped API keys (prefix ak_) created and managed via the\n    API Keys API and the\
  \ CLI. Presented as bearer tokens.\n  id_prefix: ak_\n  docs: https://agentuity.dev/reference/api/api-keys\n- name: oauthApplications\n  type: oauth2\n  description: >-\n    OAuth 2.0 / OIDC applications with client credentials, user consent, and authorization\n    scopes, managed via the OAuth Applications API. Enables \"Sign in with Agentuity\".\n  docs: https://agentuity.dev/reference/api/oauth\n- name: agentuityOIDC\n  type: openIdConnect\n  description: >-\n    Agentuity OIDC provider — add Agentuity account sign-in and scoped access to your app\n    with OAuth 2.0 and OIDC (\"Sign in with Agentuity\").\n  docs: https://agentuity.dev/services/oidc-provider\npublic_endpoints:\n- description: A small number of endpoints are public and require no auth (e.g. AI Gateway GET /models).\nnotes: >-\n  Auth model captured from the published REST API reference (no OpenAPI/Swagger spec is\n  published, so this profile is search-derived from the docs rather than machine-derived).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentuity/refs/heads/main/authentication/agentuity-authentication.yml
summary_line: http/apiKey/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Agents
- Artificial Intelligence
- Cloud
- Serverless
- Platform
- Developer Tools
- LLM
- Infrastructure
- Deployment
- AI Gateway
---
