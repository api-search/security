---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clipform-io-analytics-api-openapi.yml
  format: yaml
  label: Clipform Analytics API
  slug: clipform-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-analytics-api-openapi.yml
- filename: clipform-io-authentication-api-openapi.yml
  format: yaml
  label: Clipform Authentication API
  slug: clipform-io-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-authentication-api-openapi.yml
- filename: clipform-io-dynamic-links-api-openapi.yml
  format: yaml
  label: Clipform Dynamic Links API
  slug: clipform-io-dynamic-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-dynamic-links-api-openapi.yml
- filename: clipform-io-forms-api-openapi.yml
  format: yaml
  label: Clipform Forms API
  slug: clipform-io-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-forms-api-openapi.yml
- filename: clipform-io-integrations-api-openapi.yml
  format: yaml
  label: Clipform Integrations API
  slug: clipform-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-integrations-api-openapi.yml
- filename: clipform-io-node-media-api-openapi.yml
  format: yaml
  label: Clipform Node Media API
  slug: clipform-io-node-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-node-media-api-openapi.yml
- filename: clipform-io-nodes-api-openapi.yml
  format: yaml
  label: Clipform Nodes API
  slug: clipform-io-nodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-nodes-api-openapi.yml
- filename: clipform-io-tags-api-openapi.yml
  format: yaml
  label: Clipform Tags API
  slug: clipform-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-tags-api-openapi.yml
- filename: clipform-io-tracked-links-api-openapi.yml
  format: yaml
  label: Clipform Tracked Links API
  slug: clipform-io-tracked-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-tracked-links-api-openapi.yml
- filename: clipform-io-webhooks-api-openapi.yml
  format: yaml
  label: Clipform Webhooks API
  slug: clipform-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clipform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Clipform secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Clipform
provider_slug: clipform-io
scheme_count: 2
schemes:
- description: API key (cf_*) passed as Bearer token
  issuance: Self-serve in the dashboard under Developers > API keys; shown only once; revocable. Available on every plan including free.
  key_format: A cf_ prefix followed by 64 hex characters (256 bits of entropy)
  key_prefix: cf_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clipform-io-openapi.yml
  type: http
- description: Authorization-code OAuth for installed apps acting on a user's workspace. Access tokens (cf_at_*) are passed as Bearer tokens and authorize the Integrations operations. They are opaque, single-audience, server-side records. Client credentials are issued per app - contact support@clipform.io.
  flows:
  - authorizationUrl: https://api.clipform.io/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.clipform.io/oauth/token
  name: oauth2
  note: The docs OAuth page listed in llms.txt (https://clipform.io/docs/api/oauth) returned 404 on 2026-11-04; OAuth details come from the OpenAPI only.
  sources:
  - openapi/clipform-io-openapi.yml
  token_prefix: cf_at_
  type: oauth2
slug: clipform-io-authentication
source_filename: clipform-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.clipform.io/docs/api/api-keys/\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key (cf_*) passed as Bearer token\n  sources:\n  - openapi/clipform-io-openapi.yml\n  key_prefix: cf_\n  key_format: A cf_ prefix followed by 64 hex characters (256 bits of entropy)\n  issuance: Self-serve in the dashboard under Developers > API keys; shown only once; revocable. Available\n    on every plan including free.\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.clipform.io/oauth/authorize\n    tokenUrl: https://api.clipform.io/oauth/token\n    scopes: 3\n  description: Authorization-code OAuth for installed apps acting on a user's workspace. Access tokens\n    (cf_at_*) are passed as Bearer tokens and authorize the Integrations operations. They are opaque,\n\
  \    single-audience, server-side records. Client credentials are issued per app - contact support@clipform.io.\n  sources:\n  - openapi/clipform-io-openapi.yml\n  token_prefix: cf_at_\n  note: The docs OAuth page listed in llms.txt (https://clipform.io/docs/api/oauth) returned 404 on 2026-11-04;\n    OAuth details come from the OpenAPI only.\ndocs: https://www.clipform.io/docs/api/api-keys/\nmcp_auth: The MCP server at https://mcp.clipform.io supports OAuth sign-in and anonymous sessions; the\n  local stdio server (@clipform/mcp-server) requires CLIPFORM_API_KEY (https://www.clipform.io/docs/api/mcp/).\n"
source_yaml_url: https://artifacts.apis.io/clipform-io/authentication/clipform-io-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Forms
- Form Builder
- Video
- Surveys
- Webhook
- MCP
- Lead Capture
---
