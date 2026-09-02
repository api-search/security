---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Landis Gyr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Landis+Gyr declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Landis+Gyr
provider_slug: landis-gyr
scheme_count: 0
schemes: []
slug: landis-gyr-authentication
source_filename: landis-gyr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: review.yml (developer-portal bundle inspection) + live /.well-known probes\npublic_api_auth:\n  published: false\n  summary: >-\n    Landis+Gyr documents NO authentication scheme for any product API — no API key, no\n    OAuth 2.0, no mTLS, no accreditation path, no token endpoint, no base URI. There is no\n    OpenAPI to derive securitySchemes from. This artifact records the only authentication\n    surface that could be observed, which belongs to the developer PORTAL, not to an API.\n    No `Authentication` pointer is wired into apis.yml, because the provider does not\n    document API authentication.\nportal_auth:\n  surface: https://developers.landisgyr.com/\n  scheme: Firebase Authentication (Google Identity Platform)\n  identity_provider: identitytoolkit.googleapis.com\n  bot_defence: reCAPTCHA Enterprise\n  flows_observed:\n  - /v1/accounts:signUp\n  - /v1/accounts:signInWithPassword\n  - /v1/accounts:signInWithIdp\n\
  \  - /v1/accounts:resetPassword\n  - /v1/accounts:sendOobCode\n  - /v1/token\n  - /v2/accounts:revokeToken\n  evidence: >-\n    developers.landisgyr.com is a Nuxt SPA on Firebase Hosting (project\n    cop-a-p-obj-s-stabkern-01); the above calls are present in its client bundle.\n  gate: >-\n    Authentication alone is not sufficient. Registration is followed by a validation /\n    approval workflow (POST /register/validate/{id}, an /admin/users/invitations surface,\n    a per-page access_list, and an application-status enum including APPROVED). Every\n    content route renders empty for an anonymous visitor.\ndiscovery_probes:\n- url: https://developers.landisgyr.com/.well-known/openid-configuration\n  status: 404\n- url: https://www.landisgyr.com/.well-known/openid-configuration\n  status: 404\n- url: https://developers.landisgyr.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://www.landisgyr.com/.well-known/oauth-authorization-server\n  status: 404\nschemes: []\n\
  summary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landis-gyr/refs/heads/main/authentication/landis-gyr-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Water
- Smart Metering
- AMI
- Grid
- Grid Edge
- Demand Response
- Internet of Things
- Meter Data Management
- Wi-SUN
- Energy Technology
---
