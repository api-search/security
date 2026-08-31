---
api_key_in:
- header
api_specs:
- filename: sex-offenders-api-sex-offenders-api-openapi.yml
  format: yaml
  label: Sex Offenders API Sex Offenders API
  slug: sex-offenders-api-sex-offenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sex-offenders-api/refs/heads/main/openapi/sex-offenders-api-sex-offenders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sex Offenders Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sex Offenders API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sex Offenders API
provider_slug: sex-offenders-api
scheme_count: 1
schemes:
- in: header
  issuance: manual
  issuance_note: 'CrimeoMeter''s own wording on the product page: ''x-api-key: (Request your private api-key via the "Contact Us" form)''. There is no self-service key endpoint, no developer console key page, and no documented key rotation, expiry or scoping.'
  issuance_url: https://www.crimeometer.com/#contactus
  name: apiKeyAuth
  parameter: x-api-key
  required: true
  sources:
  - https://www.crimeometer.com/sex-offenders-api
  - https://documenter.getpostman.com/view/12755833/TzK2auPn
  - openapi/sex-offenders-api-sex-offenders-api-openapi.yml
  type: apiKey
slug: sex-offenders-api-authentication
source_filename: sex-offenders-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: >-\n  https://www.crimeometer.com/sex-offenders-api (HEADERS block: Content-Type and x-api-key),\n  the public Postman collection https://documenter.getpostman.com/view/12755833/TzK2auPn\n  (every one of its 21 requests carries an x-api-key header), and\n  openapi/sex-offenders-api-sex-offenders-api-openapi.yml.\ndocs: https://www.crimeometer.com/sex-offenders-api\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth: false\n  oidc: false\n  mtls: false\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    required: true\n    issuance: manual\n    issuance_url: https://www.crimeometer.com/#contactus\n    issuance_note: >-\n      CrimeoMeter's own wording on the product page: 'x-api-key: (Request your private\n      api-key via the \"Contact Us\" form)'. There is no self-service key endpoint, no\n      developer console key page, and no documented key rotation, expiry\
  \ or scoping.\n    sources:\n      - https://www.crimeometer.com/sex-offenders-api\n      - https://documenter.getpostman.com/view/12755833/TzK2auPn\n      - openapi/sex-offenders-api-sex-offenders-api-openapi.yml\ntransport:\n  https_required: true\n  tls_version_observed: TLSv1.3\n  see: security/sex-offenders-api-domain-security.yml\nfailure_modes:\n  - status: 403\n    body: '{\"message\":\"Forbidden\"}'\n    meaning: Missing, invalid or unentitled key. See errors/sex-offenders-api-problem-types.yml.\ngaps:\n  - No key rotation, expiry or revocation policy is published.\n  - No scopes or per-endpoint entitlements are documented; one key appears to grant the whole subscription.\n  - Key issuance is a human sales loop, so an agent cannot self-onboard.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sex-offenders-api/refs/heads/main/authentication/sex-offenders-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sex Offenders
- Public Safety
- Crime Data
- Background Checks
- Criminal Justice
- Government Data
- Geospatial
- Real Estate
- Risk
- People Data
---
