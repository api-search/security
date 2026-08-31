---
api_key_in: []
auth_types: []
description: No OpenAPI or authentication reference page is published for the Akita / Postman observability API — Akita's documentation host no longer resolves and the observability API host serves no spec. The authentication model below is DERIVED from the first-party open-source agent's own REST client, which is the only public description of how the API is called. It is faithful to that source and is not a substitute for provider documentation.
kind: authentication
layout: security
method: derived
name: Akita Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akita Software declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Akita Software
provider_slug: akita-software
scheme_count: 0
schemes: []
slug: akita-software-authentication
source_filename: akita-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Akita Software\nproviderId: akita-software\ngenerated: '2026-08-30'\nmethod: derived\nsource: >-\n  rest/auth_handlers.go, rest/base_client.go and rest/domain.go in\n  https://github.com/postmanlabs/postman-insights-agent (Apache-2.0), read\n  2026-08-30\ndescription: >-\n  No OpenAPI or authentication reference page is published for the Akita /\n  Postman observability API — Akita's documentation host no longer resolves and\n  the observability API host serves no spec. The authentication model below is\n  DERIVED from the first-party open-source agent's own REST client, which is the\n  only public description of how the API is called. It is faithful to that\n  source and is not a substitute for provider documentation.\napi_host:\n  us: https://api.observability.postman.com\n  eu: https://api.observability.eu.postman.com\n  selection: >-\n    --domain overrides everything; otherwise --region /\
  \ POSTMAN_REGION (US\n    default) plus POSTMAN_ENV select the host.\n  source: rest/domain.go\nsecuritySchemes:\n  - name: postman_api_key\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: >-\n      Primary scheme. The Postman API key is sent as an `x-api-key` request\n      header on every call. Supplied via the POSTMAN_API_KEY or\n      POSTMAN_INSIGHTS_API_KEY environment variable.\n    environment_variables:\n      - POSTMAN_API_KEY\n      - POSTMAN_INSIGHTS_API_KEY\n    status: current\n  - name: postman_environment\n    type: apiKey\n    in: header\n    parameter: x-postman-env\n    description: >-\n      Companion header selecting the Postman backend environment. Set only when\n      POSTMAN_ENV is non-empty. Not a credential on its own.\n    environment_variables:\n      - POSTMAN_ENV\n    status: current\n  - name: akita_basic\n    type: http\n    scheme: basic\n    description: >-\n      Legacy fallback used only when no Postman key is present: the\
  \ Akita API\n      key ID and secret are sent as HTTP Basic credentials. The source marks\n      this path as retained for integration tests.\n    environment_variables:\n      - AKITA_API_KEY_ID\n      - AKITA_API_KEY_SECRET\n    status: legacy\n  - name: daemonset_verification_token\n    type: apiKey\n    in: header\n    description: >-\n      A Postman Insights verification token used by the Kubernetes daemonset\n      process to authenticate telemetry requests, distinct from the user API\n      key. Header name not exposed in the reviewed source.\n    status: current\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  published: false\n  note: >-\n    Key-authenticated surface with no OAuth flows and no scope reference, so no\n    scopes/ artifact is emitted. Authorization is enforced server-side by team\n    entitlement — the API returns 403 with \"API Catalog is not enabled for this\n    team\" when the feature is not licensed.\ntransport:\n  https_only: true\n \
  \ note: >-\n    The client hardcodes scheme \"https\"; plain HTTP is reachable only behind the\n    test_only_disable_https flag. Request bodies are sent as application/json.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akita-software/refs/heads/main/authentication/akita-software-authentication.yml
summary_line: 0 schemes
tags:
- Acquired
- API Discovery
- API Mapping
- API Observability
- Traffic Analysis
---
