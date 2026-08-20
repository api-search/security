---
api_key_in: []
api_specs:
- filename: zeplin-authorization-api-openapi.yml
  format: yaml
  label: Zeplin Authorization API
  slug: zeplin-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-authorization-api-openapi.yml
- filename: zeplin-colors-api-openapi.yml
  format: yaml
  label: Zeplin Colors API
  slug: zeplin-colors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-colors-api-openapi.yml
- filename: zeplin-components-api-openapi.yml
  format: yaml
  label: Zeplin Components API
  slug: zeplin-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-components-api-openapi.yml
- filename: zeplin-connected-components-api-openapi.yml
  format: yaml
  label: Zeplin Connected Components API
  slug: zeplin-connected-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-connected-components-api-openapi.yml
- filename: zeplin-design-tokens-api-openapi.yml
  format: yaml
  label: Zeplin Design Tokens API
  slug: zeplin-design-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-design-tokens-api-openapi.yml
- filename: zeplin-flows-api-openapi.yml
  format: yaml
  label: Zeplin Flows API
  slug: zeplin-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-flows-api-openapi.yml
- filename: zeplin-notifications-api-openapi.yml
  format: yaml
  label: Zeplin Notifications API
  slug: zeplin-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-notifications-api-openapi.yml
- filename: zeplin-organizations-api-openapi.yml
  format: yaml
  label: Zeplin Organizations API
  slug: zeplin-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-organizations-api-openapi.yml
- filename: zeplin-projects-api-openapi.yml
  format: yaml
  label: Zeplin Projects API
  slug: zeplin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-projects-api-openapi.yml
- filename: zeplin-screens-api-openapi.yml
  format: yaml
  label: Zeplin Screens API
  slug: zeplin-screens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-screens-api-openapi.yml
- filename: zeplin-spacing-api-openapi.yml
  format: yaml
  label: Zeplin Spacing API
  slug: zeplin-spacing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-spacing-api-openapi.yml
- filename: zeplin-styleguides-api-openapi.yml
  format: yaml
  label: Zeplin Styleguides API
  slug: zeplin-styleguides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-styleguides-api-openapi.yml
- filename: zeplin-textstyles-api-openapi.yml
  format: yaml
  label: Zeplin TextStyles API
  slug: zeplin-textstyles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-textstyles-api-openapi.yml
- filename: zeplin-users-api-openapi.yml
  format: yaml
  label: Zeplin Users API
  slug: zeplin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-users-api-openapi.yml
- filename: zeplin-variable-collections-api-openapi.yml
  format: yaml
  label: Zeplin Variable Collections API
  slug: zeplin-variable-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-variable-collections-api-openapi.yml
- filename: zeplin-webhooks-api-openapi.yml
  format: yaml
  label: Zeplin Webhooks API
  slug: zeplin-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zeplin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zeplin secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zeplin
provider_slug: zeplin
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: /v1/oauth/token
  name: OAuth2
  sources:
  - openapi/zeplin-zeplin-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: PersonalAccessToken
  scheme: bearer
  sources:
  - openapi/zeplin-zeplin-api-openapi.yml
  type: http
slug: zeplin-authentication
source_filename: zeplin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zeplin-zeplin-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/zeplin-zeplin-api-openapi.yml\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/zeplin-zeplin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/authentication/zeplin-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Design
- Design Handoff
- Developer Tools
- Figma
- Sketch
- Adobe XD
- Style Guides
- Components
- Assets
- Webhook
---
