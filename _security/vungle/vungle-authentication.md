---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Vungle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vungle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vungle
provider_slug: vungle
scheme_count: 1
schemes:
- applies_to:
  - Reporting API (https://data.liftoff.io/api/v1)
  - Campaign Management API (https://cm-api.liftoff.io/v1)
  - Audiences Integration API (https://analytics.liftoff.io/audiences/v1)
  - GDPR Opt-Out API (https://analytics.liftoff.io/opt_out/v3)
  description: 'HTTP Basic auth. The username is the Liftoff API Key and the password is the Liftoff API Secret, sent as an Authorization header of the form `Authorization: Basic base64(ApiKey:ApiSecret)`. curl example: `curl --user ''API_KEY:API_SECRET'' --url https://data.liftoff.io/api/v1/apps`'
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.liftoff.io/advertiser/reporting_api
  - https://docs.liftoff.io/advertiser/campaign_management_api
  - https://docs.liftoff.io/advertiser/direct/liftoff-api-audiences
  - https://docs.liftoff.io/advertiser/direct/liftoff-gdpr-opt-out-api
  type: http
slug: vungle-authentication
source_filename: vungle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.liftoff.io/advertiser/reporting_api\ndocs: https://docs.liftoff.io/\nnote: >-\n  Vungle is operated by Liftoff (the Liftoff + Vungle mobile growth and monetization\n  platform). The programmatic API surface is documented at docs.liftoff.io. Every\n  Vungle/Liftoff advertiser API uses HTTP Basic authentication with a Liftoff-issued\n  API key + API secret (obtained from your Account Manager). There is no OAuth 2.0,\n  OpenID Connect, or scope model.\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  credential: API Key + API Secret (issued by Liftoff Account Manager)\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic auth. The username is the Liftoff API Key and the password is the\n      Liftoff API Secret, sent as an Authorization header of the form\n      `Authorization: Basic base64(ApiKey:ApiSecret)`.\n      curl\
  \ example: `curl --user 'API_KEY:API_SECRET' --url https://data.liftoff.io/api/v1/apps`\n    applies_to:\n      - Reporting API (https://data.liftoff.io/api/v1)\n      - Campaign Management API (https://cm-api.liftoff.io/v1)\n      - Audiences Integration API (https://analytics.liftoff.io/audiences/v1)\n      - GDPR Opt-Out API (https://analytics.liftoff.io/opt_out/v3)\n    sources:\n      - https://docs.liftoff.io/advertiser/reporting_api\n      - https://docs.liftoff.io/advertiser/campaign_management_api\n      - https://docs.liftoff.io/advertiser/direct/liftoff-api-audiences\n      - https://docs.liftoff.io/advertiser/direct/liftoff-gdpr-opt-out-api\ncredential_provisioning: >-\n  API Key and API Secret are provisioned out-of-band: advertisers contact their\n  Liftoff Account Manager, who emails the key/secret pair. The Audiences Integration\n  API additionally issues partner-level credentials via a separate channel.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vungle/refs/heads/main/authentication/vungle-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Advertising
- Mobile
- Monetization
- User Acquisition
- Ad Tech
- Analytics
- Reporting
---
