---
api_key_in: []
api_specs:
- filename: signal-ai-affinity-api-openapi.yml
  format: yaml
  label: Signal AI Affinity API
  slug: signal-ai-affinity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-affinity-api-openapi.yml
- filename: signal-ai-categories-api-openapi.yml
  format: yaml
  label: Signal AI Categories API
  slug: signal-ai-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-categories-api-openapi.yml
- filename: signal-ai-content-metrics-api-openapi.yml
  format: yaml
  label: Signal AI Content Metrics API
  slug: signal-ai-content-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-content-metrics-api-openapi.yml
- filename: signal-ai-content-search-api-openapi.yml
  format: yaml
  label: Signal AI Content Search API
  slug: signal-ai-content-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-content-search-api-openapi.yml
- filename: signal-ai-entities-api-openapi.yml
  format: yaml
  label: Signal AI Entities API
  slug: signal-ai-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-entities-api-openapi.yml
- filename: signal-ai-events-api-openapi.yml
  format: yaml
  label: Signal AI Events API
  slug: signal-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-events-api-openapi.yml
- filename: signal-ai-openapi-json-api-openapi.yml
  format: yaml
  label: Signal AI Openapi.json API
  slug: signal-ai-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-openapi-json-api-openapi.yml
- filename: signal-ai-publication-sources-api-openapi.yml
  format: yaml
  label: Signal AI Publication sources API
  slug: signal-ai-publication-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-publication-sources-api-openapi.yml
- filename: signal-ai-risk-events-api-openapi.yml
  format: yaml
  label: Signal AI Risk Events API
  slug: signal-ai-risk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-risk-events-api-openapi.yml
- filename: signal-ai-topics-api-openapi.yml
  format: yaml
  label: Signal AI Topics API
  slug: signal-ai-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-topics-api-openapi.yml
- filename: signal-ai-organisation-api-openapi.yml
  format: yaml
  label: Signal AI Organisation API
  slug: signal-ai-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-organisation-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Signal Ai Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Signal AI secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Signal AI
provider_slug: signal-ai
scheme_count: 1
schemes:
- description: "To obtain the Bearer Token using the Client ID / Secret pair provided to you:\n\n```bash\ncurl -X POST \\\n  -d 'grant_type=client_credentials' \\\n  -d 'client_id=YOUR_CLIENT_ID' \\\n  -d 'client_secret=YOUR_CLIENT_SECRET' \\\n  https://api.signal-ai.com/auth/token\n```\n\nThis will return the following JSON response:\n\n```json\n{\n    \"access_token\": \"eyJhbGciOi…\",\n    \"expires_in\": 86400,\n    …\n}\n```\n\nYou must "
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://api.signal-ai.com/auth/token
  name: OAuth2
  sources:
  - openapi/signal-ai-affinity-api-openapi.yml
  - openapi/signal-ai-categories-api-openapi.yml
  - openapi/signal-ai-content-metrics-api-openapi.yml
  - openapi/signal-ai-content-search-api-openapi.yml
  - openapi/signal-ai-entities-api-openapi.yml
  - openapi/signal-ai-events-api-openapi.yml
  - openapi/signal-ai-openapi-json-api-openapi.yml
  - openapi/signal-ai-organisation-api-openapi.yml
  - openapi/signal-ai-publication-sources-api-openapi.yml
  - openapi/signal-ai-risk-events-api-openapi.yml
  - openapi/signal-ai-topics-api-openapi.yml
  type: oauth2
slug: signal-ai-authentication
source_filename: signal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://api.signal-ai.com/docs\nsource: https://api.signal-ai.com/openapi.json (live, fetched 2026-08-13, HTTP 200) + openapi/signal-ai-affinity-api-openapi.yml, openapi/signal-ai-categories-api-openapi.yml,\n  openapi/signal-ai-content-metrics-api-openapi.yml, openapi/signal-ai-content-search-api-openapi.yml,\n  openapi/signal-ai-entities-api-openapi.yml, openapi/signal-ai-events-api-openapi.yml, openapi/signal-ai-openapi-json-api-openapi.yml,\n  openapi/signal-ai-organisation-api-openapi.yml, openapi/signal-ai-publication-sources-api-openapi.yml,\n  openapi/signal-ai-risk-events-api-openapi.yml, openapi/signal-ai-topics-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.signal-ai.com/auth/token\n    scopes: 6\n  description: \"To obtain the Bearer Token using the Client ID / Secret\
  \ pair provided to you:\\n\\\n    \\n```bash\\ncurl -X POST \\\\\\n  -d 'grant_type=client_credentials' \\\\\\n  -d 'client_id=YOUR_CLIENT_ID'\\\n    \\ \\\\\\n  -d 'client_secret=YOUR_CLIENT_SECRET' \\\\\\n  https://api.signal-ai.com/auth/token\\n\\\n    ```\\n\\nThis will return the following JSON response:\\n\\n```json\\n{\\n    \\\"access_token\\\"\\\n    : \\\"eyJhbGciOi…\\\",\\n    \\\"expires_in\\\": 86400,\\n    …\\n}\\n```\\n\\nYou must \"\n  sources:\n  - openapi/signal-ai-affinity-api-openapi.yml\n  - openapi/signal-ai-categories-api-openapi.yml\n  - openapi/signal-ai-content-metrics-api-openapi.yml\n  - openapi/signal-ai-content-search-api-openapi.yml\n  - openapi/signal-ai-entities-api-openapi.yml\n  - openapi/signal-ai-events-api-openapi.yml\n  - openapi/signal-ai-openapi-json-api-openapi.yml\n  - openapi/signal-ai-organisation-api-openapi.yml\n  - openapi/signal-ai-publication-sources-api-openapi.yml\n  - openapi/signal-ai-risk-events-api-openapi.yml\n  - openapi/signal-ai-topics-api-openapi.yml\n\
  \nenrichment:\n  generated: '2026-08-13'\n  method: searched\n  docs: https://api.signal-ai.com/docs\n  summary: >-\n    One authentication style across the whole REST surface: OAuth2\n    client-credentials. There is no API key, no basic auth, no mTLS and no\n    user-facing authorization-code flow on the REST API. Credentials are a Client\n    ID / Client Secret pair issued by Signal AI to contracted customers, not\n    self-issued through a developer portal.\n  token:\n    endpoint: https://api.signal-ai.com/auth/token\n    grant_type: client_credentials\n    request: 'POST form-encoded: grant_type=client_credentials, client_id, client_secret'\n    response_fields: [access_token, expires_in]\n    ttl_seconds: 86400\n    usage: 'Authorization: Bearer <access_token>'\n    failure_status: 401\n  identity_provider:\n    product: Keycloak\n    issuer: https://login.signal-ai.com/auth/realms/signal\n    discovery: well-known/signal-ai-openid-configuration.json\n    grant_types_supported:\
  \ [authorization_code, implicit, refresh_token, password, client_credentials,\n      'urn:ietf:params:oauth:grant-type:device_code', 'urn:openid:params:grant-type:ciba']\n  agent_surface:\n    endpoint: https://mcp.signal-ai.com/mcp\n    style: oauth2-bearer\n    challenge: RFC 6750 WWW-Authenticate with RFC 9728 resource_metadata pointer\n    scopes: [openid, 'mcp:tools', offline_access]\n    pkce: S256\n    note: >-\n      The MCP surface authenticates against the same Keycloak realm but through a\n      browser authorization-code + PKCE flow (observed on the 302 from\n      https://mcp.signal-ai.com/docs), not the REST client-credentials grant.\n  probes:\n  - url: https://api.signal-ai.com/topics\n    status: 401\n    note: 'Unauthenticated GET; response carries signal-version: 1 and no auth challenge\n      header.'\n  - url: https://mcp.signal-ai.com/mcp\n    status: 401\n    note: Unauthenticated tools/list; returns a correct Bearer challenge with resource_metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/authentication/signal-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Media Intelligence
- Reputation Management
- Risk Intelligence
- News
- Content Search
- Knowledge Graph
- ESG
- Artificial Intelligence
- Analytics
---
