---
api_key_in:
- header
api_specs:
- filename: anecdotes-analysis-rules-api-openapi.yml
  format: yaml
  label: anecdotes Analysis Rules API
  slug: anecdotes-analysis-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-analysis-rules-api-openapi.yml
- filename: anecdotes-authorization-api-openapi.yml
  format: yaml
  label: anecdotes Authorization API
  slug: anecdotes-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-authorization-api-openapi.yml
- filename: anecdotes-create-controls-api-openapi.yml
  format: yaml
  label: anecdotes Create Controls API
  slug: anecdotes-create-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-create-controls-api-openapi.yml
- filename: anecdotes-create-evidence-api-openapi.yml
  format: yaml
  label: anecdotes Create Evidence API
  slug: anecdotes-create-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-create-evidence-api-openapi.yml
- filename: anecdotes-custom-fields-api-openapi.yml
  format: yaml
  label: anecdotes Custom Fields API
  slug: anecdotes-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-custom-fields-api-openapi.yml
- filename: anecdotes-download-evidence-api-openapi.yml
  format: yaml
  label: anecdotes Download Evidence API
  slug: anecdotes-download-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-download-evidence-api-openapi.yml
- filename: anecdotes-findings-api-openapi.yml
  format: yaml
  label: anecdotes Findings API
  slug: anecdotes-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-findings-api-openapi.yml
- filename: anecdotes-framework-api-openapi.yml
  format: yaml
  label: anecdotes Framework API
  slug: anecdotes-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-framework-api-openapi.yml
- filename: anecdotes-gated-api-openapi.yml
  format: yaml
  label: anecdotes Gated API
  slug: anecdotes-gated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-gated-api-openapi.yml
- filename: anecdotes-policy-manager-api-openapi.yml
  format: yaml
  label: anecdotes Policy Manager API
  slug: anecdotes-policy-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-policy-manager-api-openapi.yml
- filename: anecdotes-public-api-openapi.yml
  format: yaml
  label: anecdotes Public API
  slug: anecdotes-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-public-api-openapi.yml
- filename: anecdotes-read-controls-api-openapi.yml
  format: yaml
  label: anecdotes Read Controls API
  slug: anecdotes-read-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-read-controls-api-openapi.yml
- filename: anecdotes-read-evidence-metadata-api-openapi.yml
  format: yaml
  label: anecdotes Read Evidence Metadata API
  slug: anecdotes-read-evidence-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-read-evidence-metadata-api-openapi.yml
- filename: anecdotes-requirements-api-openapi.yml
  format: yaml
  label: anecdotes Requirements API
  slug: anecdotes-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-requirements-api-openapi.yml
- filename: anecdotes-risk-api-openapi.yml
  format: yaml
  label: anecdotes Risk API
  slug: anecdotes-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-risk-api-openapi.yml
- filename: anecdotes-token-api-openapi.yml
  format: yaml
  label: anecdotes Token API
  slug: anecdotes-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-token-api-openapi.yml
- filename: anecdotes-update-control-metadata-api-openapi.yml
  format: yaml
  label: anecdotes Update Control Metadata API
  slug: anecdotes-update-control-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-update-control-metadata-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Anecdotes Authentication
name_suffix: Authentication
oauth_flows: []
overview: anecdotes secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: anecdotes
provider_slug: anecdotes
scheme_count: 2
schemes:
- description: Static API key created in the Anecdotes platform under Administration -> API tokens, with a name, expiration date and role. Used only for the exchange endpoint.
  in: header
  name: ApiKey
  parameter: x-anecdotes-api-key
  sources:
  - openapi/anecdotes-grc-openapi.yml
  - openapi/anecdotes-fedramp-20x-openapi.yml
  type: apiKey
  used_by:
  - exchangeApiKey
  - exchangeApiKeyFedramp
- bearerFormat: JWT
  description: 'Short-lived JWT obtained from GET /identity/v1/apikey/exchange. Valid for 1 hour; re-exchange on 401. Sent as `Authorization: Bearer <token>` on every operation other than the exchange itself and the FedRAMP public endpoints.'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/anecdotes-grc-openapi.yml
  - openapi/anecdotes-fedramp-20x-openapi.yml
  type: http
slug: anecdotes-authentication
source_filename: anecdotes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://help.anecdotes.ai/api/overview\nderived_from: openapi/anecdotes-grc-openapi.yml, openapi/anecdotes-fedramp-20x-openapi.yml\ndocs:\n- https://help.anecdotes.ai/api/token\n- https://help.anecdotes.ai/technical-setup/api/using-the-anecdotes-api\n- https://help.anecdotes.ai/technical-setup/api/create-an-api-token\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: two-step - static API key exchanged for a short-lived JWT\n  token_lifetime_seconds: 3600\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-anecdotes-api-key\n  description: >-\n    Static API key created in the Anecdotes platform under Administration -> API tokens, with a name,\n    expiration date and role. Used only for the exchange endpoint.\n  used_by: [exchangeApiKey, exchangeApiKeyFedramp]\n  sources:\n  - openapi/anecdotes-grc-openapi.yml\n  - openapi/anecdotes-fedramp-20x-openapi.yml\n\
  - name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Short-lived JWT obtained from GET /identity/v1/apikey/exchange. Valid for 1 hour; re-exchange on 401.\n    Sent as `Authorization: Bearer <token>` on every operation other than the exchange itself and the\n    FedRAMP public endpoints.\n  sources:\n  - openapi/anecdotes-grc-openapi.yml\n  - openapi/anecdotes-fedramp-20x-openapi.yml\nflow:\n- step: 1\n  action: Create an API token in the platform (Administration -> API tokens), assigning name, expiration date and role.\n- step: 2\n  action: 'GET https://api.anecdotes.ai/identity/v1/apikey/exchange with header x-anecdotes-api-key: <token>'\n  returns: JWT as text/plain\n- step: 3\n  action: 'Send Authorization: Bearer <JWT> on all subsequent requests.'\n- step: 4\n  action: On 401, repeat step 2 - JWTs expire after 60 minutes.\nadditional_requirements:\n- header: User-Agent\n  required: true\n  format: 'YOUR-APP-NAME/1.0 (+contact@domain.com)'\n \
  \ note: >-\n    A descriptive User-Agent identifying the calling application is mandatory. The documented cause of a\n    403 despite a valid JWT is a missing or unacceptable User-Agent.\n- header: trustcenterurl\n  required: true\n  applies_to: FedRAMP 20x endpoints\n  example: trust.anecdotes.ai\nauthorization:\n  model: role-based, assigned per API token\n  roles:\n  - name: Admin\n    description: Can pull or push any data and perform any available action on the system. Required for the MCP Proxy.\n  - name: Integrator\n    description: Can create new evidence and push data into self-managed evidence.\n  - name: Auditor\n    description: Can read general information about, and export, the frameworks the auditor has access to.\n  scopes: none - Anecdotes has no OAuth scope surface; authorization is by token role.\nanonymous_access:\n  present: true\n  endpoints:\n  - POST /fedramp20x/v1/access\n  - GET /fedramp20x/v1/public/info\n  note: >-\n    The FedRAMP 20x public tier requires\
  \ no credentials at all; verified live on 2026-07-31 with HTTP 200.\nmcp:\n  scheme: api-key\n  header: X-anecdotes-api-key\n  note: The MCP Proxy takes the raw API key directly rather than an exchanged JWT, and requires the Admin role.\n  artifact: mcp/anecdotes-mcp.yml\nfederated_identity:\n  sso:\n    protocol: SAML 2.0\n    providers: [Okta, Microsoft Entra ID, OneLogin, JumpCloud, PingIdentity]\n    docs: https://help.anecdotes.ai/technical-setup/sso\n  provisioning:\n    protocol: SCIM\n    providers: [Okta, Microsoft Entra ID]\n    role_mapping: true\n    docs: https://help.anecdotes.ai/technical-setup/scim\n  note: >-\n    SSO and SCIM govern human access to the platform, not API token authentication. Anecdotes is a\n    service provider, not an identity provider, so it serves no OIDC discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/authentication/anecdotes-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Compliance
- Governance
- Risk
- Security
- GRC
- Audit
- Evidence
- Continuous Compliance
- FedRAMP
- Artificial Intelligence
- Agents
---
