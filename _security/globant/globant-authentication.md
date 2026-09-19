---
anonymous_access: false
api_key_in: []
api_specs:
- filename: globant-catalog-api-openapi.yml
  format: yaml
  label: Globant Catalog API
  slug: globant-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globant/refs/heads/main/openapi/globant-catalog-api-openapi.yml
- filename: globant-health-api-openapi.yml
  format: yaml
  label: Globant Health API
  slug: globant-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globant/refs/heads/main/openapi/globant-health-api-openapi.yml
auth_types: []
description: 'Globant runs three authentication models across three separate surfaces, and one of them is unusually well documented for agents: glob.ai publishes an auth.md that states in plain language what exists, what is gated, and — explicitly, so agents stop probing — what does NOT exist.'
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Globant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Globant declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Globant
provider_slug: globant
scheme_count: 0
schemes: []
slug: globant-authentication
source_filename: globant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://glob.ai/auth.md, https://docs.globant.ai/en/wiki?20,Glob.AI+OS+API+Reference, https://docs.globant.ai/en/wiki?3895,PyGEAI+API+Authentication\nprovider: Globant\nproviderId: globant\ndescription: >-\n  Globant runs three authentication models across three separate surfaces, and one of them is unusually\n  well documented for agents: glob.ai publishes an auth.md that states in plain language what exists,\n  what is gated, and — explicitly, so agents stop probing — what does NOT exist.\nsurfaces:\n  - surface: Glob.AI public API\n    host: glob.ai\n    spec: ../openapi/globant-glob-ai-public-api-openapi.json\n    docs: https://glob.ai/auth.md\n    schemes:\n      - type: none\n        applies_to:\n          - GET /api/catalog\n          - GET /api/v1/health\n          - /.well-known/api-catalog\n          - /openapi.json\n          - /docs/api.md\n          - /.well-known/agent-skills/index.json\n          - /llms.txt\n\
  \          - /llms-full.txt\n        note: The OpenAPI declares no securitySchemes and no security requirement; the surface is genuinely anonymous.\n      - type: session\n        applies_to: ['everything else on the glob.ai origin']\n        mechanism: Browser session via Globant Access Management (GAM) single sign-on\n        self_service: false\n    declared_absences:\n      - 'No password grant'\n      - 'No client-credentials flow'\n      - 'No API-key self-service'\n      - 'No self-service or anonymous agent registration — programmatic access is provisioned by authenticated users from inside the platform'\n      - 'No OAuth/OIDC discovery metadata: this origin is not an OAuth issuer (/.well-known/openid-configuration, /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource are not served)'\n      - 'No agent-autonomous payments; checkout requires human card entry'\n    access_path: 'https://glob.ai — reviewed request, human-in-the-loop provisioning'\n \
  \ - surface: Glob.AI Hubs Orchestrator (MCP)\n    host: api.beta.glob.ai\n    docs: https://glob.ai/.well-known/agent-skills/orchestrator-mcp-setup/SKILL.md\n    schemes:\n      - type: apiKey\n        name: MCP_TOKEN\n        in: env\n        mechanism: Token passed to the local stdio MCP server as an environment variable\n        issuance: 'Minted by a signed-in human in the Glob.AI console (https://aipods.glob.ai) from a project runner setup'\n        self_service: false\n    observed:\n      - {url: 'https://api.beta.glob.ai/api/v1/projects', status: 401, body: '{\"detail\":\"Authentication required\"}'}\n      - {url: 'https://api.beta.glob.ai/api/v1/health', status: 200, body: '{\"status\":\"ok\",\"version\":\"0.1.0\"}'}\n  - surface: Globant Enterprise AI (Glob.AI OS)\n    host: api.saia.ai\n    docs: https://docs.globant.ai/en/wiki?20,Glob.AI+OS+API+Reference\n    schemes:\n      - type: http\n        scheme: bearer\n        variable: GEAI_APITOKEN\n        scope: project\n   \
  \     mechanism: 'HTTP Bearer token; a per-project API token'\n      - type: http\n        scheme: bearer\n        variable: GEAI_ORGANIZATION_APITOKEN\n        scope: organization\n        mechanism: 'HTTP Bearer token; required for organization-level endpoints (admin/organizations, usageLimits/organizations/*)'\n      - type: oauth2\n        variable: OAuth_accesstoken\n        mechanism: 'Temporary OAuth access tokens offered for enhanced security'\n        note: >-\n          The docs reference OAuth access tokens but publish no authorization/token endpoint, no scope\n          reference and no discovery document. No scopes/ artifact was written for this reason — see\n          notes.\n    token_management:\n      docs: https://docs.globant.ai/en/wiki?564,API+Tokens\n      operations:\n        - 'POST /projects/tokens'\n        - 'GET /organization/project/{id}/tokens'\n        - 'GET /projects/tokens/{ApiTokenId}'\n        - 'PUT /projects/tokens/{ApiTokenId}'\n        - 'DELETE /projects/tokens/{ApiTokenId}'\n\
  \        - 'GET /accessControl/apitoken/validate'\n    related_errors:\n      - {code: 5, message: Api Key Not Found}\n      - {code: 6, message: ApiToken not found or blocked}\n      - {code: 7, message: ApiToken out of scope}\n      - {code: 101, message: Refresh token error}\n      - {code: 102, message: Token revoked, login again}\n      - {code: 103, message: Token expired, login again}\n      - {code: 112, message: Access token not found, login again}\n      - {code: 114, message: Access token not valid, login again}\n      - {code: 122, message: Session token error, login again}\n  - surface: Legacy Globant gateway\n    host: api.globant.com\n    docs: null\n    schemes:\n      - type: unknown\n        mechanism: 'Unknown. Every path, including / and /.well-known/*, returns HTTP 401 {\"status\":\"Error\",\"description\":\" Authentication Error\"}.'\n    note: >-\n      No public documentation for this host was found anywhere. It is a live, wholly gated gateway with\n      no discoverable\
  \ contract.\nnotes:\n  - >-\n    No scopes/globant-scopes.yml was written. glob.ai/auth.md states the origin is not an OAuth issuer,\n    the GEAI docs name OAuth access tokens without publishing a scope reference, and no OpenAPI with\n    oauth2 securitySchemes exists to derive a baseline from. An invented scope list would be fabrication.\n  - >-\n    RBAC inside Globant Enterprise AI is documented separately at\n    https://docs.globant.ai/en/wiki?242,Managing+Roles+and+Permissions+in+Glob.AI+OS and is a\n    platform-internal permission model, not an API scope surface.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globant/refs/heads/main/authentication/globant-authentication.yml
summary_line: 0 schemes
tags:
- Software
- Digital Transformation
- Artificial Intelligence
- Agents
- MCP
- Consulting
- Enterprise
---
