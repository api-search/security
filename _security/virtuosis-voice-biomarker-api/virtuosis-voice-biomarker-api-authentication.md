---
api_key_in: []
api_specs:
- filename: virtuosis-voice-biomarker-api-accounts-api-openapi.yml
  format: yaml
  label: Virtuosis Voice Biomarker API Accounts API
  slug: virtuosis-voice-biomarker-api-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/openapi/virtuosis-voice-biomarker-api-accounts-api-openapi.yml
- filename: virtuosis-voice-biomarker-api-default-api-openapi.yml
  format: yaml
  label: Virtuosis Voice Biomarker API Voice Biomarker Api Default API
  slug: virtuosis-voice-biomarker-api-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/openapi/virtuosis-voice-biomarker-api-default-api-openapi.yml
- filename: virtuosis-voice-biomarker-api-recordings-api-openapi.yml
  format: yaml
  label: Virtuosis Voice Biomarker API Recordings API
  slug: virtuosis-voice-biomarker-api-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/openapi/virtuosis-voice-biomarker-api-recordings-api-openapi.yml
- filename: virtuosis-voice-biomarker-api-usage-api-openapi.yml
  format: yaml
  label: Virtuosis Voice Biomarker API Usage API
  slug: virtuosis-voice-biomarker-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/openapi/virtuosis-voice-biomarker-api-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Virtuosis Voice Biomarker Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Virtuosis Voice Biomarker API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Virtuosis Voice Biomarker API
provider_slug: virtuosis-voice-biomarker-api
scheme_count: 1
schemes:
- applied_to: all operations
  format: 'Authorization: Bearer <API_KEY>'
  header: Authorization
  in: header
  name: bearerAuth
  note: The v1.3 OpenAPI declares bearerAuth under components.securitySchemes but does not attach a root-level security[] block; instead every operation declares an explicit required Authorization header parameter. The docs are unambiguous that a bearer token is required on all requests.
  scheme: bearer
  sources:
  - openapi/virtuosis-voice-biomarker-api-openapi.yml
  - https://docs.virtuosis.ai/api-reference
  type: http
slug: virtuosis-voice-biomarker-api-authentication
source_filename: virtuosis-voice-biomarker-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-18'\nmethod: searched\nsource: https://docs.virtuosis.ai/api-reference\ndocs:\n  - https://docs.virtuosis.ai/api-reference\n  - https://docs.virtuosis.ai/voice-biomarker-api\nderived_from: openapi/virtuosis-voice-biomarker-api-openapi.yml\nsummary:\n  types:\n    - http\n  model: bearer-token\n  oauth2: false\n  scopes: false\n  note: >-\n    Single-scheme API. A long-lived organisation API key is presented as an HTTP Bearer token on every\n    request. There are no OAuth flows, no scopes, no refresh, and no separate test credential - so\n    scopes/ is intentionally absent for this provider.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <API_KEY>'\n    applied_to: all operations\n    sources:\n      - openapi/virtuosis-voice-biomarker-api-openapi.yml\n      - https://docs.virtuosis.ai/api-reference\n    note: >-\n      The v1.3 OpenAPI declares bearerAuth\
  \ under components.securitySchemes but does not attach a\n      root-level security[] block; instead every operation declares an explicit required Authorization\n      header parameter. The docs are unambiguous that a bearer token is required on all requests.\ncredentials:\n  issuance: >-\n    API keys are provisioned in the Virtuosis app at https://app.virtuosis.ai/. The public site routes\n    API access through a trial request form (https://www.virtuosis.ai/trial-request) rather than\n    instant self-service key generation.\n  scope_of_key: organisation\n  note: >-\n    Accounts created through POST /accounts are scoped to the organisation that owns the API key and\n    are always assigned the \"speaker\" organisation role - the key, not the request, determines tenancy.\n  key_prefix: null\n  key_prefix_note: The provider does not publish a key prefix convention.\n  rotation_policy: not published\n  expiry: not published\nauthorization:\n  model: >-\n    Entitlement-based rather than\
  \ scope-based. Which analysis families a key may request is controlled\n    server-side by Virtuosis, not by anything the caller sends.\n  tiers:\n    - name: self-service\n      covers:\n        - wellbeing\n        - communication_coach\n      note: >-\n        Wellbeing insights (stress, anxiety, mood) and communication insights are available through\n        self-service access.\n      source: https://www.virtuosis.ai/voice-biomarker-api\n    - name: manually validated\n      covers:\n        - parkinsons\n        - alzheimers\n      note: >-\n        Medical insights are released only after manual validation by Virtuosis, stated as within 48\n        hours, in accordance with the intended purpose of its CE-marked software as a medical device.\n      source: https://www.virtuosis.ai/voice-biomarker-api\n  denial_signals:\n    - status: 403\n      condition: Requested analysis is not enabled for the organisation\n    - status: 403\n      condition: Access is suspended\n    - status:\
  \ 403\n      condition: API billing is not provisioned for the organisation\n    - status: 401\n      condition: Missing or invalid bearer token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/authentication/virtuosis-voice-biomarker-api-authentication.yml
summary_line: http · 1 scheme
tags:
- digital health
- voice biomarkers
- speech analysis
- acoustic analysis
- medical device
- mental health
- wellbeing
- neurodegenerative screening
- telehealth
- remote monitoring
- communication coaching
- clinical research
---
