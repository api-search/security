---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hover-agreements-api-openapi.yml
  format: yaml
  label: HOVER Agreements API
  slug: hover-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-agreements-api-openapi.yml
- filename: hover-blueprints-api-openapi.yml
  format: yaml
  label: HOVER Blueprints API
  slug: hover-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-blueprints-api-openapi.yml
- filename: hover-blueprints-copy-api-openapi.yml
  format: yaml
  label: HOVER Blueprints (COPY) API
  slug: hover-blueprints-copy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-blueprints-copy-api-openapi.yml
- filename: hover-capture-requests-api-openapi.yml
  format: yaml
  label: HOVER Capture Requests API
  slug: hover-capture-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-capture-requests-api-openapi.yml
- filename: hover-deliverables-api-openapi.yml
  format: yaml
  label: HOVER Deliverables API
  slug: hover-deliverables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-deliverables-api-openapi.yml
- filename: hover-estimates-api-openapi.yml
  format: yaml
  label: HOVER Estimates API
  slug: hover-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-estimates-api-openapi.yml
- filename: hover-https-api-openapi.yml
  format: yaml
  label: 'HOVER Https: API'
  slug: hover-https-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-https-api-openapi.yml
- filename: hover-inspection-workflows-api-openapi.yml
  format: yaml
  label: HOVER Inspection Workflows API
  slug: hover-inspection-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-inspection-workflows-api-openapi.yml
- filename: hover-inspections-api-openapi.yml
  format: yaml
  label: HOVER Inspections API
  slug: hover-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-inspections-api-openapi.yml
- filename: hover-instant-design-api-openapi.yml
  format: yaml
  label: HOVER Instant Design API
  slug: hover-instant-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-instant-design-api-openapi.yml
- filename: hover-job-shares-api-openapi.yml
  format: yaml
  label: HOVER Job Shares API
  slug: hover-job-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-job-shares-api-openapi.yml
- filename: hover-jobs-api-openapi.yml
  format: yaml
  label: HOVER Jobs API
  slug: hover-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-jobs-api-openapi.yml
- filename: hover-models-api-openapi.yml
  format: yaml
  label: HOVER Models API
  slug: hover-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-models-api-openapi.yml
- filename: hover-notes-api-openapi.yml
  format: yaml
  label: HOVER Notes API
  slug: hover-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-notes-api-openapi.yml
- filename: hover-notes-json-api-openapi.yml
  format: yaml
  label: HOVER Notes.json API
  slug: hover-notes-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-notes-json-api-openapi.yml
- filename: hover-oauth-api-openapi.yml
  format: yaml
  label: HOVER OAuth API
  slug: hover-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-oauth-api-openapi.yml
- filename: hover-orgs-api-openapi.yml
  format: yaml
  label: HOVER Orgs API
  slug: hover-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-orgs-api-openapi.yml
- filename: hover-payments-api-openapi.yml
  format: yaml
  label: HOVER Payments API
  slug: hover-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-payments-api-openapi.yml
- filename: hover-users-api-openapi.yml
  format: yaml
  label: HOVER Users API
  slug: hover-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-users-api-openapi.yml
- filename: hover-wallets-api-openapi.yml
  format: yaml
  label: HOVER Wallets API
  slug: hover-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-wallets-api-openapi.yml
- filename: hover-waste-factor-api-openapi.yml
  format: yaml
  label: HOVER Waste Factor API
  slug: hover-waste-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-waste-factor-api-openapi.yml
- filename: hover-webhooks-api-openapi.yml
  format: yaml
  label: HOVER Webhooks API
  slug: hover-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/openapi/hover-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hover Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: HOVER secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: HOVER
provider_slug: hover
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://hover.to/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://hover.to/oauth/token
    tokenUrl: https://hover.to/oauth/token
  levels:
  - user
  - org
  name: OAuth2
  org_level_note: Some endpoints, when used with org-level OAuth 2.0, require a params[current_user_email] or params[current_user_id] value or a 422 may be returned.
  token:
    access_token_note: An access token is valid for 2 hours and must be refreshed.
    access_token_ttl: 2h
    refresh_token_note: A refresh token is valid indefinitely but invalidates when it is exchanged for a new access token / refresh token combination.
  type: oauth2
slug: hover-authentication
source_filename: hover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.hover.to/docs/oauth-20-authentication\ndocs: https://developers.hover.to/docs/oauth-20-authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, refreshToken]\n  api_key_in: []\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://hover.to/oauth/authorize\n        tokenUrl: https://hover.to/oauth/token\n        refreshUrl: https://hover.to/oauth/token\n    token:\n      access_token_ttl: 2h\n      access_token_note: An access token is valid for 2 hours and must be refreshed.\n      refresh_token_note: >-\n        A refresh token is valid indefinitely but invalidates when it is\n        exchanged for a new access token / refresh token combination.\n    levels:\n      - user\n      - org\n    org_level_note: >-\n      Some endpoints, when used with org-level OAuth 2.0, require a\n      params[current_user_email] or\
  \ params[current_user_id] value or a 422 may\n      be returned.\nscopes_documented: false\nscopes_note: >-\n  Hover's public OAuth documentation does not enumerate granular scopes; access\n  is governed at the user/organization level.\nmcp_auth: https://developers.hover.to/docs/authentication-for-mcp-use\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/authentication/hover-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise
- Construction
- Roofing
- Insurance
- 3D Modeling
- Property Data
- Measurements
- Home Services
- Geospatial
---
