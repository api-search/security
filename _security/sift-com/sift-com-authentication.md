---
api_key_in: []
api_specs:
- filename: sift-com-decisions-api-openapi.yml
  format: yaml
  label: Sift Decisions API
  slug: sift-com-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-com-decisions-api-openapi.yml
- filename: sift-com-events-api-openapi.yml
  format: yaml
  label: Sift Events API
  slug: sift-com-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-com-events-api-openapi.yml
- filename: sift-com-labels-api-openapi.yml
  format: yaml
  label: Sift Labels API
  slug: sift-com-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-com-labels-api-openapi.yml
- filename: sift-com-scores-api-openapi.yml
  format: yaml
  label: Sift Scores API
  slug: sift-com-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-com-scores-api-openapi.yml
- filename: sift-com-verification-api-openapi.yml
  format: yaml
  label: Sift Verification API
  slug: sift-com-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-com-verification-api-openapi.yml
- filename: sift-com-workflows-api-openapi.yml
  format: yaml
  label: Sift Workflows API
  slug: sift-com-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-com-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sift Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sift
provider_slug: sift-com
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/sift-decisions-api-openapi.yml
  - openapi/sift-events-api-openapi.yml
  - openapi/sift-labels-api-openapi.yml
  - openapi/sift-score-api-openapi.yml
  - openapi/sift-verification-api-openapi.yml
  - openapi/sift-workflows-api-openapi.yml
  type: http
slug: sift-com-authentication
source_filename: sift-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sift-decisions-api-openapi.yml, openapi/sift-events-api-openapi.yml, openapi/sift-labels-api-openapi.yml,\n  openapi/sift-score-api-openapi.yml, openapi/sift-verification-api-openapi.yml, openapi/sift-workflows-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sift-decisions-api-openapi.yml\n  - openapi/sift-events-api-openapi.yml\n  - openapi/sift-labels-api-openapi.yml\n  - openapi/sift-score-api-openapi.yml\n  - openapi/sift-verification-api-openapi.yml\n  - openapi/sift-workflows-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/authentication/sift-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Fraud Prevention
- Trust and Safety
- Risk Scoring
- Identity Verification
- Chargebacks
- Account Takeover
- Content Abuse
---
