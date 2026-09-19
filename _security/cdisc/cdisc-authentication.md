---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cdisc-adam-api-openapi.yml
  format: yaml
  label: cdisc ADaM API
  slug: cdisc-adam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-adam-api-openapi.yml
- filename: cdisc-biomedical-concepts-api-openapi.yml
  format: yaml
  label: cdisc Biomedical Concepts API
  slug: cdisc-biomedical-concepts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-biomedical-concepts-api-openapi.yml
- filename: cdisc-cdash-api-openapi.yml
  format: yaml
  label: cdisc CDASH API
  slug: cdisc-cdash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-cdash-api-openapi.yml
- filename: cdisc-products-api-openapi.yml
  format: yaml
  label: cdisc Products API
  slug: cdisc-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-products-api-openapi.yml
- filename: cdisc-sdtm-api-openapi.yml
  format: yaml
  label: cdisc SDTM API
  slug: cdisc-sdtm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-sdtm-api-openapi.yml
- filename: cdisc-terminology-api-openapi.yml
  format: yaml
  label: cdisc Terminology API
  slug: cdisc-terminology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-terminology-api-openapi.yml
- filename: cdisc-ars-api-openapi.yml
  format: yaml
  label: CDISC Analysis Results Standard (ARS) API
  slug: cdisc-analysis-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-ars-api-openapi.yml
- filename: cdisc-dataset-json-api-openapi.json
  format: json
  label: CDISC Dataset-JSON API (standard specification)
  slug: cdisc-dataset-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-dataset-json-api-openapi.json
- filename: cdisc-usdm-api-openapi.yml
  format: yaml
  label: CDISC USDM (DDF) Study Definitions API
  slug: cdisc-usdm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-usdm-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cdisc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cdisc secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cdisc
provider_slug: cdisc
scheme_count: 1
schemes:
- description: Single-factor API key ("subscription key" in Azure API Management terms) sent on every request as the `api-key` header. Declared identically in every published CDISC contract.
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/_original/cdisc-library-openapi.yml
  - openapi/cdisc-ars-api-openapi.yml
  - openapi/cdisc-sdtm-api-openapi.yml
  type: apiKey
slug: cdisc-authentication
source_filename: cdisc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  live 401 from https://library.cdisc.org/api/mdr/products (probed 2026-09-17);\n  https://www.cdisc.org/cdisc-library/getting-started ; https://api.developer.library.cdisc.org/ ;\n  openapi/_original/cdisc-library-openapi.yml ; openapi/cdisc-ars-api-openapi.yml\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  oidc: false\n  mtls: false\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter: api-key\n    description: >-\n      Single-factor API key (\"subscription key\" in Azure API Management terms) sent on every request as the\n      `api-key` header. Declared identically in every published CDISC contract.\n    sources:\n      - openapi/_original/cdisc-library-openapi.yml\n      - openapi/cdisc-ars-api-openapi.yml\n      - openapi/cdisc-sdtm-api-openapi.yml\nlive_evidence:\n  url: https://library.cdisc.org/api/mdr/products\n  status: 401\n  probed: '2026-09-17'\n\
  \  www_authenticate: 'AzureApiManagementKey realm=\"https://api.library.cdisc.org/api\", name=\"api-key\", type=\"header\"'\n  body: '{ \"statusCode\": 401, \"message\": \"Access denied due to missing subscription key. Make sure to include subscription key when making requests to an API.\" }'\nonboarding:\n  steps:\n    - Request a CDISC Library account at https://www.cdisc.org/cdisc-library/api-account-request (the page is\n      access-controlled and returned 403 to an anonymous crawler on 2026-09-17; it renders a CDISC sign-in/sign-up form).\n    - Complete Microsoft Azure AD B2C email verification for the CDISC Library account (documented step-by-step\n      on https://www.cdisc.org/cdisc-library/getting-started).\n    - Sign in to the Azure API Management developer portal at https://api.developer.library.cdisc.org/ and\n      subscribe to the product; the portal issues primary and secondary keys.\n  eligibility: CDISC member organisations and open-source developers (per the license\
  \ block of the CDISC contracts).\n  self_serve: false\n  note: >-\n    Key issuance is gated behind an approved account, not an instant signup. The developer portal itself\n    redirects anonymous visitors to /signin.\nrotation:\n  supported: true\n  note: >-\n    Azure API Management issues primary and secondary subscription keys per product and supports regeneration\n    from the developer portal — a platform capability, not a documented CDISC policy.\nscopes:\n  present: false\n  note: No OAuth scopes exist; entitlement is per-product subscription, granted by membership level.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/authentication/cdisc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Clinical Trials
- Standards
- Life Sciences
- Pharma
- Healthcare
- Metadata
- Controlled Terminology
- Data Exchange
- Non-Profit
---
