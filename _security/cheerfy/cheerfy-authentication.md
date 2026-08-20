---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Cheerfy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cheerfy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cheerfy
provider_slug: cheerfy
scheme_count: 1
schemes:
- evidence:
    body: '{"detail":"Authentication credentials were not provided."}'
    fetched: '2026-08-10'
    framework: Django REST Framework (inferred from the challenge + error envelope shape)
    http_status: 401
    server: gunicorn
    url: https://webhook.cheerfy.com/
    www_authenticate: Token
  form: 'Authorization: Token <key>'
  host: https://webhook.cheerfy.com
  in: header
  name: TokenAuth
  parameter_name: Authorization
  scheme: Token
  sources:
  - probe
  type: http
slug: cheerfy-authentication
source_filename: cheerfy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live HTTP probe of https://webhook.cheerfy.com/\nnote: >-\n  There is no OpenAPI to derive securitySchemes from, and the Loyalty Card / Coupons API reference\n  pages on docs.cheerfy.com are unreadable to a non-JavaScript client. This profile records what a\n  live probe of the one reachable Cheerfy API host actually returned: an HTTP 401 carrying\n  \"WWW-Authenticate: Token\", the Django REST Framework token-authentication challenge. The scheme\n  name, header form and error envelope below are observed, not inferred from documentation.\nsummary:\n  types: [http]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: TokenAuth\n  type: http\n  scheme: Token\n  in: header\n  parameter_name: Authorization\n  form: 'Authorization: Token <key>'\n  host: https://webhook.cheerfy.com\n  sources: [probe]\n  evidence:\n    url: https://webhook.cheerfy.com/\n    http_status: 401\n\
  \    www_authenticate: Token\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n    server: gunicorn\n    framework: Django REST Framework (inferred from the challenge + error envelope shape)\n    fetched: '2026-08-10'\noauth:\n  published: false\n  discovery:\n    openid_configuration: not served (404/503/307 on every Cheerfy host)\n    oauth_authorization_server: not served (404/503/307 on every Cheerfy host)\n  note: >-\n    auth.cheerfy.com is referenced by the admin console at admin.cheerfy.com/login/ but returns 404\n    on / and on both OAuth/OIDC discovery paths, so no authorization-server metadata is public.\nkey_issuance:\n  self_service: false\n  note: >-\n    No public sign-up for API credentials. Credentials are issued inside the tenant admin console\n    (https://admin.cheerfy.com/login/); the business-services terms state only that \"CHEERFY\n    provides an API to allow the Business to engage third party service providers\".\ngaps:\n- no machine-readable\
  \ specification declaring securitySchemes\n- no public authentication reference page a machine can read\n- no OAuth or OIDC discovery document on any host\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheerfy/refs/heads/main/authentication/cheerfy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Restaurant
- Hospitality
- CRM
- Loyalty
- Customer Engagement
- Marketing Automation
- Online Ordering
- Payments
---
