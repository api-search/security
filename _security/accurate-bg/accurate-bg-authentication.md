---
api_key_in: []
api_specs:
- filename: accurate-bg-openapi.yml
  format: yaml
  label: Accurate Candidates API
  slug: accurate-bg-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-openapi.yml
- filename: accurate-bg-openapi.yml
  format: yaml
  label: Accurate Orders API
  slug: accurate-bg-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-openapi.yml
- filename: accurate-bg-openapi.yml
  format: yaml
  label: Accurate Packages API
  slug: accurate-bg-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-openapi.yml
- filename: accurate-bg-openapi.yml
  format: yaml
  label: Accurate Reports API
  slug: accurate-bg-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-openapi.yml
- filename: accurate-bg-openapi.yml
  format: yaml
  label: Accurate Documents API
  slug: accurate-bg-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-openapi.yml
- filename: accurate-bg-openapi.yml
  format: yaml
  label: Accurate Adjudication API
  slug: accurate-bg-adjudication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-openapi.yml
- filename: accurate-bg-openapi.yml
  format: yaml
  label: Accurate Verifications API
  slug: accurate-bg-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-openapi.yml
- filename: accurate-bg-openapi.yml
  format: yaml
  label: Accurate Notifications API
  slug: accurate-bg-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Accurate Bg Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Accurate Background secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Accurate Background
provider_slug: accurate-bg
scheme_count: 1
schemes:
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/accurate-bg-openapi.yml
  type: oauth2
slug: accurate-bg-authentication
source_filename: accurate-bg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accurate-bg-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n    scopes: 0\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\n  sources:\n  - openapi/accurate-bg-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/authentication/accurate-bg-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Background Checks
- Employment Screening
- Identity Verification
- Compliance
- HR Tech
- Screening
---
