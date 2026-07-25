---
api_key_in: []
api_specs:
- filename: guidewire-integration-gateway-asyncapi.yml
  format: yaml
  label: Guidewire Integration Gateway API
  slug: guidewire-integration-gateway-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/asyncapi/guidewire-integration-gateway-asyncapi.yml
- filename: guidewire-accounts-api-openapi.yml
  format: yaml
  label: Guidewire Accounts API
  slug: guidewire-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-accounts-api-openapi.yml
- filename: guidewire-claims-api-openapi.yml
  format: yaml
  label: Guidewire Claims API
  slug: guidewire-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-claims-api-openapi.yml
- filename: guidewire-exposures-api-openapi.yml
  format: yaml
  label: Guidewire Exposures API
  slug: guidewire-exposures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-exposures-api-openapi.yml
- filename: guidewire-fnol-api-openapi.yml
  format: yaml
  label: Guidewire FNOL API
  slug: guidewire-fnol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-fnol-api-openapi.yml
- filename: guidewire-payments-api-openapi.yml
  format: yaml
  label: Guidewire Payments API
  slug: guidewire-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-payments-api-openapi.yml
- filename: guidewire-policies-api-openapi.yml
  format: yaml
  label: Guidewire Policies API
  slug: guidewire-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-policies-api-openapi.yml
- filename: guidewire-quotes-api-openapi.yml
  format: yaml
  label: Guidewire Quotes API
  slug: guidewire-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-quotes-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Guidewire Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Guidewire secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Guidewire
provider_slug: guidewire
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.guidewire.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://login.guidewire.com/oauth/token
  name: OAuth2
  sources:
  - openapi/guidewire-claimcenter-openapi.yml
  - openapi/guidewire-policycenter-openapi.yml
  type: oauth2
slug: guidewire-authentication
source_filename: guidewire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guidewire-claimcenter-openapi.yml, openapi/guidewire-policycenter-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.guidewire.com/oauth/authorize\n    tokenUrl: https://login.guidewire.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/guidewire-claimcenter-openapi.yml\n  - openapi/guidewire-policycenter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/authentication/guidewire-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Insurance
- Policy
- Claims
- Billing
- P&C
---
