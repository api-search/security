---
anonymous_access: false
api_key_in: []
api_specs:
- filename: curiosity-admin-agent-api-openapi.yml
  format: yaml
  label: Curiosity Admin Agent API
  slug: curiosity-admin-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-admin-agent-api-openapi.yml
- filename: curiosity-build-api-openapi.yml
  format: yaml
  label: Curiosity Build API
  slug: curiosity-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-build-api-openapi.yml
- filename: curiosity-cce-api-openapi.yml
  format: yaml
  label: Curiosity Cce API
  slug: curiosity-cce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-cce-api-openapi.yml
- filename: curiosity-chatai-api-openapi.yml
  format: yaml
  label: Curiosity Chatai API
  slug: curiosity-chatai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-chatai-api-openapi.yml
- filename: curiosity-code-api-openapi.yml
  format: yaml
  label: Curiosity Code API
  slug: curiosity-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-code-api-openapi.yml
- filename: curiosity-config-api-openapi.yml
  format: yaml
  label: Curiosity Config API
  slug: curiosity-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-config-api-openapi.yml
- filename: curiosity-curiosity-api-api-openapi.yml
  format: yaml
  label: Curiosity Curiosity API
  slug: curiosity-curiosity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-curiosity-api-api-openapi.yml
- filename: curiosity-embeddings-api-openapi.yml
  format: yaml
  label: Curiosity Embeddings API
  slug: curiosity-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-embeddings-api-openapi.yml
- filename: curiosity-endpoints-api-openapi.yml
  format: yaml
  label: Curiosity Endpoints API
  slug: curiosity-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-endpoints-api-openapi.yml
- filename: curiosity-graph-api-openapi.yml
  format: yaml
  label: Curiosity Graph API
  slug: curiosity-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-graph-api-openapi.yml
- filename: curiosity-groups-api-openapi.yml
  format: yaml
  label: Curiosity Groups API
  slug: curiosity-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-groups-api-openapi.yml
- filename: curiosity-install-api-openapi.yml
  format: yaml
  label: Curiosity Install API
  slug: curiosity-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-install-api-openapi.yml
- filename: curiosity-login-api-openapi.yml
  format: yaml
  label: Curiosity Login API
  slug: curiosity-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-login-api-openapi.yml
- filename: curiosity-messages-api-openapi.yml
  format: yaml
  label: Curiosity Messages API
  slug: curiosity-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-messages-api-openapi.yml
- filename: curiosity-migrations-api-openapi.yml
  format: yaml
  label: Curiosity Migrations API
  slug: curiosity-migrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-migrations-api-openapi.yml
- filename: curiosity-models-api-openapi.yml
  format: yaml
  label: Curiosity Models API
  slug: curiosity-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-models-api-openapi.yml
- filename: curiosity-node-api-openapi.yml
  format: yaml
  label: Curiosity Node API
  slug: curiosity-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-node-api-openapi.yml
- filename: curiosity-saml-api-openapi.yml
  format: yaml
  label: Curiosity SAML API
  slug: curiosity-saml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-saml-api-openapi.yml
- filename: curiosity-search-api-openapi.yml
  format: yaml
  label: Curiosity Search API
  slug: curiosity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-search-api-openapi.yml
- filename: curiosity-chat-completions-api-openapi.yml
  format: yaml
  label: Curiosity Chat Completions API
  slug: curiosity-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/curiosity-chat-completions-api-openapi.yml
auth_types: []
description: Curiosity uses bearer tokens passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Curiosity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curiosity declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Curiosity
provider_slug: curiosity
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer <endpoint-token>'
  header: Authorization
  how_to_obtain: Created via Admin → API Tokens (API token, Endpoint token) or via login flow for Session JWT.
  location: header
  name: API token / Endpoint token / Session JWT
  type: http-bearer
slug: curiosity-authentication
source_filename: curiosity-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.curiosity.ai/workspace-learning/07-apis-endpoints/02-authentication
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.curiosity.ai/workspace-learning/07-apis-endpoints/02-authentication\nsources:\n- https://docs.curiosity.ai/workspace-learning/07-apis-endpoints/02-authentication\n- https://docs.curiosity.ai/workspace/getting-started/build-your-first-enterprise-ai-app\ndescription: Curiosity uses bearer tokens passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API token / Endpoint token / Session JWT\n  evidence: 'Authorization: Bearer <endpoint-token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Created via Admin → API Tokens (API token, Endpoint token) or via login flow for Session JWT.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented on the referenced pages.\ndocs: https://docs.curiosity.ai/workspace-learning/07-apis-endpoints/02-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/authentication/curiosity-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Knowledge-Graph
- Enterprise
- Data-Integration
- On-Premises
- Company
---
