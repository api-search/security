---
api_key_in: []
api_specs:
- filename: verdigris-technologies-control-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Control API
  slug: verdigris-technologies-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-control-api-openapi.yml
- filename: verdigris-technologies-current-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Current API
  slug: verdigris-technologies-current-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-current-api-openapi.yml
- filename: verdigris-technologies-energy-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Energy API
  slug: verdigris-technologies-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-energy-api-openapi.yml
- filename: verdigris-technologies-events-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Events API
  slug: verdigris-technologies-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-events-api-openapi.yml
- filename: verdigris-technologies-forecast-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Forecast API
  slug: verdigris-technologies-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-forecast-api-openapi.yml
- filename: verdigris-technologies-power-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Power API
  slug: verdigris-technologies-power-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-power-api-openapi.yml
- filename: verdigris-technologies-power-factor-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Power Factor API
  slug: verdigris-technologies-power-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-power-factor-api-openapi.yml
- filename: verdigris-technologies-total-harmonic-distortion-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Total Harmonic Distortion API
  slug: verdigris-technologies-total-harmonic-distortion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-total-harmonic-distortion-api-openapi.yml
- filename: verdigris-technologies-voltage-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Voltage API
  slug: verdigris-technologies-voltage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-voltage-api-openapi.yml
- filename: verdigris-technologies-weather-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Weather API
  slug: verdigris-technologies-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-weather-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Verdigris Technologies Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Verdigris Technologies secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Verdigris Technologies
provider_slug: verdigris-technologies
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.verdigris.co/oauth/token
  name: oauth2
  sources:
  - openapi/verdigris-technologies-data-v4-openapi.json
  type: oauth2
slug: verdigris-technologies-authentication
source_filename: verdigris-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/verdigris-technologies-data-v4-openapi.json\ndocs: https://docs.verdigris.co/reference/authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  token_type: Bearer JWT\n  token_lifetime_seconds: 3600\n  audience: https://api.verdigris.co/\n  credential_provisioning: Verdigris Admin Console (admin.verdigris.co) issues a Client ID + Client Secret per API key\n  token_request_rate_limit: 20 token requests per hour (480 per rolling 24h); HTTP 429 when exceeded\n  access_note: API access is restricted to active Verdigris customers\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.verdigris.co/oauth/token\n    scopes: 0\n  sources:\n  - openapi/verdigris-technologies-data-v4-openapi.json\nnotes:\n- Obtain a token by POSTing grant_type=client_credentials with client_id, client_secret,\n  and audience=https://api.verdigris.co/ to https://auth.verdigris.co/oauth/token.\n\
  - Send the returned token on every API call via the Authorization header (Bearer scheme).\n- Tokens live for 1 hour; cache and reuse them to avoid the 20/hour token-issuance limit.\n- Identity provider is Auth0 (auth.verdigris.co publishes an OIDC discovery document).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/authentication/verdigris-technologies-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Energy
- Energy Management
- Building Automation
- Smart Buildings
- IoT
- Sustainability
- Power Monitoring
- Time Series
- Analytics
- Electricity
---
