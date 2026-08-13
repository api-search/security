---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Marin Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marin Software secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Marin Software
provider_slug: marin-software
scheme_count: 1
schemes:
- credential_issuance: contact your Marin representative
  description: All Marin API endpoints require HTTP Basic authorization using a Marin username and password — the same credentials used to sign in to the MarinOne application, granting access to the same client accounts. Credentials are issued by a Marin representative; there is no self-service key issuance, no OAuth, and no API-key surface documented.
  name: basicAuth
  scheme: basic
  sources:
  - https://support.marinsoftware.com/en_US/bulk-actions/marin-api
  type: http
slug: marin-software-authentication
source_filename: marin-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://support.marinsoftware.com/en_US/bulk-actions/marin-api\ndocs: https://support.marinsoftware.com/en_US/bulk-actions/marin-api\nnote: >-\n  Marin Software publishes no OpenAPI, so this profile is read from the provider's own\n  live help-center API article rather than derived from a machine-readable spec. The\n  dedicated developer portal that the docs point at\n  (http://developers.marinsoftware.com/api/docs/) no longer resolves to a docs site —\n  every *.marinsoftware.com subdomain is a wildcard catch-all that 301/200s to the\n  marketing homepage — so the help center is the only remaining public auth reference.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    All Marin API endpoints require HTTP Basic authorization using a Marin username and\n    password — the same credentials used to sign in to the MarinOne application,\
  \ granting\n    access to the same client accounts. Credentials are issued by a Marin representative;\n    there is no self-service key issuance, no OAuth, and no API-key surface documented.\n  credential_issuance: contact your Marin representative\n  sources:\n  - https://support.marinsoftware.com/en_US/bulk-actions/marin-api\ntenancy:\n  note: >-\n    Marin does not scope requests through the token. Account scoping is carried in required\n    query-string parameters on every call, with the values read out of the MarinOne UI.\n  parameters:\n  - name: clientId\n    in: query\n    required: true\n    description: Marin client ID — Client ID column in M1 > Accounts > Publishers grid.\n  - name: customerId\n    in: query\n    required: true\n    description: Marin customer ID — Customer ID column in M1 > Accounts > Publishers grid.\n  - name: userId\n    in: query\n    required: true\n    description: Marin user ID — the docs instruct the caller to read it from the browser\n      developer-tools\
  \ HTTP request headers.\n  - name: userCustomerId\n    in: query\n    required: true\n    description: Marin user customer ID — Customer ID column in M1 > Accounts > Publishers grid.\ntransport:\n  https_only: true\n  note: Only HTTPS requests are supported; plain HTTP will fail.\ngaps:\n- No OAuth 2.0 or OpenID Connect surface is documented.\n- No scopes or permissions model is published, so scopes/ is intentionally absent.\n- No API keys, no token rotation policy, and no MFA guidance for API credentials.\n- Credentials are the interactive user's own username and password, so an API credential\n  cannot be revoked independently of the human account.\nx-evidence:\n- url: https://support.marinsoftware.com/en_US/bulk-actions/marin-api\n  status: 200\n  fetched: '2026-08-12'\n- url: https://developers.marinsoftware.com/api/docs/\n  status: 200\n  note: redirects to https://www.marinsoftware.com/ — the developer docs portal is gone\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marin-software/refs/heads/main/authentication/marin-software-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Martech
- Advertising
- Marketing
- Performance Marketing
- Digital Advertising
- Paid Search
- Paid Social
- Retail Media
- Campaign Management
- Bid Management
- Bulk Upload
---
