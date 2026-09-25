---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: probabl-anthropic-compatible-agent-api-openapi.yml
  format: yaml
  label: Probabl Anthropic Compatible Agent API
  slug: probabl-anthropic-compatible-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/openapi/probabl-anthropic-compatible-agent-api-openapi.yml
- filename: probabl-health-api-openapi.yml
  format: yaml
  label: Probabl Health API
  slug: probabl-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/openapi/probabl-health-api-openapi.yml
- filename: probabl-identity-api-openapi.yml
  format: yaml
  label: Probabl Identity API
  slug: probabl-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/openapi/probabl-identity-api-openapi.yml
- filename: probabl-liveness-api-openapi.yml
  format: yaml
  label: Probabl Liveness API
  slug: probabl-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/openapi/probabl-liveness-api-openapi.yml
- filename: probabl-llm-provider-api-openapi.yml
  format: yaml
  label: Probabl LLM Provider API
  slug: probabl-llm-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/openapi/probabl-llm-provider-api-openapi.yml
- filename: probabl-openai-compatible-agent-api-openapi.yml
  format: yaml
  label: Probabl OpenAI Compatible Agent API
  slug: probabl-openai-compatible-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/openapi/probabl-openai-compatible-agent-api-openapi.yml
- filename: probabl-projects-api-openapi.yml
  format: yaml
  label: Probabl Projects API
  slug: probabl-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/openapi/probabl-projects-api-openapi.yml
- filename: probabl-readiness-api-openapi.yml
  format: yaml
  label: Probabl Readiness API
  slug: probabl-readiness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/openapi/probabl-readiness-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Probabl Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Probabl secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Probabl
provider_slug: probabl
scheme_count: 2
schemes:
- description: Workspace-scoped API key. skore sends it as the X-API-Key header when SKORE_HUB_API_KEY is set (non-interactive / agent use). Keys are minted by an interactively logged-in user.
  env_var: SKORE_HUB_API_KEY
  in: header
  key_fields:
    expires_at: optional date-time
    name: optional
    permissions: required, array of Permission
    workspace_id: required
  lifecycle_operations:
  - openapi/probabl-identity-api-openapi.yml#create_api_key_identity_users__user_id__api_keys_post
  - openapi/probabl-identity-api-openapi.yml#list_api_keys_identity_users__user_id__api_keys_get
  - openapi/probabl-identity-api-openapi.yml#patch_api_key_identity_users__user_id__api_keys__api_key_id__patch
  - openapi/probabl-identity-api-openapi.yml#delete_api_key_identity_users__user_id__api_keys__api_key_id__delete
  name: SkoreHubAPIKey
  parameter: X-API-Key
  permissions:
  - create:project
  - read:project
  - update:project
  - delete:project
  - create:invitation
  - read:invitation
  - delete:invitation
  permissions_source: OpenAPI components.schemas.Permission (API-key permissions, not OAuth scopes)
  type: apiKey
  used_by:
  - REST API
  - Skore Hub MCP server (https://api.skore.probabl.ai/mcp) via requestHeaders X-API-Key
- bearer_header: 'Authorization: Bearer <access_token>'
  description: 'Interactive login. The hub brokers an external identity provider (OIDC): /identity/oauth/login returns the IdP authorization_url (authorization code flow); /identity/oauth/device/login + /identity/oauth/device/token implement a device flow used by the skore Python client and skore-cli. Refresh via /identity/oauth/token/refresh; logout revokes tokens at the OAuth2 provider when a revocation endpoint is advertised.'
  flows:
  - flow: authorizationCode
    operations:
    - openapi/probabl-identity-api-openapi.yml#oauth_login_identity_oauth_login_get
    - openapi/probabl-identity-api-openapi.yml#oauth_callback_identity_oauth_callback_get
  - flow: deviceCode
    operations:
    - openapi/probabl-identity-api-openapi.yml#oauth_device_identity_oauth_device_login_get
    - openapi/probabl-identity-api-openapi.yml#oauth_device_token_identity_oauth_device_token_get
  name: SkoreHubOAuth
  note: Token responses carry a `scope` string but no scope catalogue is published.
  scopes_documented: false
  type: oauth2
slug: probabl-authentication
source_filename: probabl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource:\n- https://api.skore.probabl.ai/openapi.json\n- https://github.com/probabl-ai/skore/blob/main/skore/src/skore/_plugins/hub/authentication/apikey.py\n- https://github.com/probabl-ai/skore-cli/blob/main/src/skore_cli/_hub_auth.py\n- https://github.com/probabl-ai/skore-cli/blob/main/README.md\nnote: The live Skore Hub OpenAPI (3.1.0) declares NO components.securitySchemes, so derive-authentication.py yields\n  nothing. The schemes below come from Probabl's own first-party client code (skore, skore-cli) and the identity\n  operations in the spec. An unauthenticated GET /identity/users/me and GET /v1/models both returned 401 {\"detail\":\"Unauthorized\"}\n  on 2026-09-16.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - deviceCode\n  declared_in_openapi: false\nschemes:\n- name: SkoreHubAPIKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  env_var: SKORE_HUB_API_KEY\n\
  \  description: Workspace-scoped API key. skore sends it as the X-API-Key header when SKORE_HUB_API_KEY is set (non-interactive\n    / agent use). Keys are minted by an interactively logged-in user.\n  lifecycle_operations:\n  - openapi/probabl-identity-api-openapi.yml#create_api_key_identity_users__user_id__api_keys_post\n  - openapi/probabl-identity-api-openapi.yml#list_api_keys_identity_users__user_id__api_keys_get\n  - openapi/probabl-identity-api-openapi.yml#patch_api_key_identity_users__user_id__api_keys__api_key_id__patch\n  - openapi/probabl-identity-api-openapi.yml#delete_api_key_identity_users__user_id__api_keys__api_key_id__delete\n  key_fields:\n    workspace_id: required\n    permissions: required, array of Permission\n    expires_at: optional date-time\n    name: optional\n  permissions:\n  - create:project\n  - read:project\n  - update:project\n  - delete:project\n  - create:invitation\n  - read:invitation\n  - delete:invitation\n  permissions_source: OpenAPI components.schemas.Permission\
  \ (API-key permissions, not OAuth scopes)\n  used_by:\n  - REST API\n  - Skore Hub MCP server (https://api.skore.probabl.ai/mcp) via requestHeaders X-API-Key\n- name: SkoreHubOAuth\n  type: oauth2\n  bearer_header: 'Authorization: Bearer <access_token>'\n  description: 'Interactive login. The hub brokers an external identity provider (OIDC): /identity/oauth/login returns\n    the IdP authorization_url (authorization code flow); /identity/oauth/device/login + /identity/oauth/device/token\n    implement a device flow used by the skore Python client and skore-cli. Refresh via /identity/oauth/token/refresh;\n    logout revokes tokens at the OAuth2 provider when a revocation endpoint is advertised.'\n  flows:\n  - flow: authorizationCode\n    operations:\n    - openapi/probabl-identity-api-openapi.yml#oauth_login_identity_oauth_login_get\n    - openapi/probabl-identity-api-openapi.yml#oauth_callback_identity_oauth_callback_get\n  - flow: deviceCode\n    operations:\n    - openapi/probabl-identity-api-openapi.yml#oauth_device_identity_oauth_device_login_get\n\
  \    - openapi/probabl-identity-api-openapi.yml#oauth_device_token_identity_oauth_device_token_get\n  scopes_documented: false\n  note: Token responses carry a `scope` string but no scope catalogue is published.\nworkspace_header:\n  name: x-skore-workspace\n  in: header\n  operations:\n  - /v1/chat/completions\n  - /v1/responses\n  - /v1/messages\nroles:\n  values:\n  - owner\n  - contributor\n  - reader\n  source: OpenAPI components.schemas.WorkspaceRole\ndocs: https://github.com/probabl-ai/skore-cli#agent\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/probabl/refs/heads/main/authentication/probabl-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Open Source
- Machine Learning
- Data Science
- scikit-learn
- MLOps
- Model Evaluation
- Experiment Tracking
- Agent Skills
- Artificial Intelligence
- Python
- France
---
