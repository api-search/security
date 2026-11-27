---
anonymous_access: false
api_key_in: []
api_specs:
- filename: figma-files-api-openapi.yml
  format: yaml
  label: Figma Files API
  slug: figma-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-files-api-openapi.yml
- filename: figma-projects-api-openapi.yml
  format: yaml
  label: Figma Projects API
  slug: figma-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-projects-api-openapi.yml
- filename: figma-component-sets-api-openapi.yml
  format: yaml
  label: Figma Component Sets API
  slug: figma-component-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-component-sets-api-openapi.yml
- filename: figma-activity-logs-api-openapi.yml
  format: yaml
  label: Figma Activity Logs API
  slug: figma-activity-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-activity-logs-api-openapi.yml
- filename: figma-payments-api-openapi.yml
  format: yaml
  label: Figma Payments API
  slug: figma-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-payments-api-openapi.yml
- filename: figma-dev-resources-api-openapi.yml
  format: yaml
  label: Figma Dev Resources API
  slug: figma-dev-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-dev-resources-api-openapi.yml
- filename: figma-comments-api-openapi.yml
  format: yaml
  label: Figma Comments API
  slug: figma-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-comments-api-openapi.yml
- filename: figma-components-api-openapi.yml
  format: yaml
  label: Figma Components API
  slug: figma-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-components-api-openapi.yml
- filename: figma-library-analytics-api-openapi.yml
  format: yaml
  label: Figma Library Analytics API
  slug: figma-library-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-library-analytics-api-openapi.yml
- filename: figma-users-api-openapi.yml
  format: yaml
  label: Figma Users API
  slug: figma-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-users-api-openapi.yml
- filename: figma-ai-usage-api-openapi.yml
  format: yaml
  label: Figma AI Usage API
  slug: figma-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-ai-usage-api-openapi.yml
- filename: figma-comment-reactions-api-openapi.yml
  format: yaml
  label: Figma Comment Reactions API
  slug: figma-comment-reactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-comment-reactions-api-openapi.yml
- filename: figma-developer-logs-api-openapi.yml
  format: yaml
  label: Figma Developer Logs API
  slug: figma-developer-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-developer-logs-api-openapi.yml
- filename: figma-folders-api-openapi.yml
  format: yaml
  label: Figma Folders API
  slug: figma-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-folders-api-openapi.yml
- filename: figma-styles-api-openapi.yml
  format: yaml
  label: Figma Styles API
  slug: figma-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-styles-api-openapi.yml
- filename: figma-variables-api-openapi.yml
  format: yaml
  label: Figma Variables API
  slug: figma-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-variables-api-openapi.yml
- filename: figma-webhooks-api-openapi.yml
  format: yaml
  label: Figma Webhooks API
  slug: figma-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-webhooks-api-openapi.yml
- filename: figma-teams-api-openapi.yml
  format: yaml
  label: Figma Teams API
  slug: figma-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-teams-api-openapi.yml
- filename: figma-o-embed-api-openapi.yml
  format: yaml
  label: Figma o Embed API
  slug: figma-o-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-o-embed-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Figma Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Figma secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Figma
provider_slug: figma
scheme_count: 3
schemes:
- docs: https://developers.figma.com/docs/rest-api/oauth-apps/
  flows:
  - authorizationUrl: https://www.figma.com/oauth
    client_auth: 'Authorization: Basic <BASE64_ENCODED_CLIENT_ID_AND_SECRET>'
    code_lifetime: Authentication codes expire 30 seconds after being issued
    flow: authorizationCode
    pkce: optional; S256 only
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OAuth2
  note: Token response includes access token expiration in seconds; refresh flow documented. Figma for Government uses a separate api.figma-gov host.
  required_for:
  - Activity Logs API
  - Discovery API
  - Embed API
  scopes_ref: scopes/figma-scopes.yml
  spec_sources:
  - OAuth2
  - OrgOAuth2 securitySchemes in openapi/*.yml
  type: oauth2
  usage: 'Authorization: Bearer <TOKEN>'
- docs: https://developers.figma.com/docs/rest-api/plan-access-tokens/
  header: X-Figma-Token
  in: header
  name: PlanAccessToken
  note: 'Scoped to an Organization or Enterprise plan, not tied to a user; managed by plan administrators; optional resource allowlist; max expiration of 1 year. Categories: REST API, npm registry, Figma CLI (fixed scope set). REST API tokens cannot call endpoints requiring file_code_connect:write, file_variables:write, file_comments:write, /v1/me or /v1/oembed.'
  type: apiKey
- docs: https://developers.figma.com/docs/rest-api/personal-access-tokens/
  header: X-Figma-Token
  in: header
  name: PersonalAccessToken
  note: Acts as the user who generated it; expiration and scopes set at creation.
  type: apiKey
slug: figma-authentication
source_filename: figma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: searched\nsource: https://developers.figma.com/docs/rest-api/authentication/\ndocs: https://developers.figma.com/docs/rest-api/authentication/\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  oauth2_flows:\n  - authorizationCode\n  recommended: OAuth app (OAuth 2)\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n    pkce: optional; S256 only\n    code_lifetime: Authentication codes expire 30 seconds after being issued\n    client_auth: 'Authorization: Basic <BASE64_ENCODED_CLIENT_ID_AND_SECRET>'\n  usage: 'Authorization: Bearer <TOKEN>'\n  scopes_ref: scopes/figma-scopes.yml\n  required_for:\n  - Activity Logs API\n  - Discovery API\n  - Embed API\n  note: Token response includes access token expiration in seconds; refresh flow documented. Figma for\n    Government uses a separate api.figma-gov host.\n  docs:\
  \ https://developers.figma.com/docs/rest-api/oauth-apps/\n  spec_sources:\n  - OAuth2\n  - OrgOAuth2 securitySchemes in openapi/*.yml\n- name: PlanAccessToken\n  type: apiKey\n  in: header\n  header: X-Figma-Token\n  note: 'Scoped to an Organization or Enterprise plan, not tied to a user; managed by plan administrators;\n    optional resource allowlist; max expiration of 1 year. Categories: REST API, npm registry, Figma CLI\n    (fixed scope set). REST API tokens cannot call endpoints requiring file_code_connect:write, file_variables:write,\n    file_comments:write, /v1/me or /v1/oembed.'\n  docs: https://developers.figma.com/docs/rest-api/plan-access-tokens/\n- name: PersonalAccessToken\n  type: apiKey\n  in: header\n  header: X-Figma-Token\n  note: Acts as the user who generated it; expiration and scopes set at creation.\n  docs: https://developers.figma.com/docs/rest-api/personal-access-tokens/\ndocs_pages:\n- https://developers.figma.com/docs/rest-api/oauth-apps/\n- https://developers.figma.com/docs/rest-api/plan-access-tokens/\n\
  - https://developers.figma.com/docs/rest-api/personal-access-tokens/\n- https://developers.figma.com/docs/rest-api/scopes/\n"
source_yaml_url: https://artifacts.apis.io/figma/authentication/figma-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
- Figma
---
