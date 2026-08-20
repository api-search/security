---
api_key_in: []
auth_types: []
description: 'Giveffect does not publish how its API is authenticated. There is no developer portal, no auth page, no OAuth or OIDC discovery document, and no OpenAPI with securitySchemes to derive from. Probing the production API host anonymously does not reveal the scheme either: unknown paths return 404 rather than a 401 with a WWW-Authenticate challenge, so the service does not advertise its challenge to an unauthenticated caller. NO Authentication pointer is emitted from this file — it records that the auth model is undocumented, which is the opposite of authentication_documented.'
kind: authentication
layout: security
method: searched
name: Giveffect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Giveffect declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Giveffect
provider_slug: giveffect
scheme_count: 0
schemes: []
slug: giveffect-authentication
source_filename: giveffect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: giveffect.com + api.giveffect.com probes\nname: Giveffect API authentication\ndescription: >-\n  Giveffect does not publish how its API is authenticated. There is no developer\n  portal, no auth page, no OAuth or OIDC discovery document, and no OpenAPI with\n  securitySchemes to derive from. Probing the production API host anonymously\n  does not reveal the scheme either: unknown paths return 404 rather than a 401\n  with a WWW-Authenticate challenge, so the service does not advertise its\n  challenge to an unauthenticated caller. NO Authentication pointer is emitted\n  from this file — it records that the auth model is undocumented, which is the\n  opposite of authentication_documented.\ndocumented: false\nschemes: []\nscheme_count: 0\ndiscovery:\n- url: https://api.giveffect.com/.well-known/openid-configuration\n  status: 404\n- url: https://api.giveffect.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://api.giveffect.com/.well-known/oauth-protected-resource\n\
  \  status: 404\n- url: https://www.giveffect.com/.well-known/openid-configuration\n  status: 404\n- url: https://www.giveffect.com/.well-known/oauth-authorization-server\n  status: 404\nchallenge_observed:\n  www_authenticate: false\n  status_on_unknown_path: 404\n  note: >-\n    GET https://api.giveffect.com/v1/donors returns\n    {\"error\":{\"code\":404,\"message\":\"Not Found - Invalid resource\"}} with no\n    WWW-Authenticate header. A 401 could not be provoked anonymously.\nprovisioning:\n  model: enterprise-provisioned\n  tier: Ultimate+\n  evidence: >-\n    \"Open API and custom integration\" is listed only on the Ultimate+ pricing\n    card; the Ultimate card reads \"All system features (excludes open API)\".\n    Access is therefore granted by Giveffect sales/success, not self-serve.\n  source: https://www.giveffect.com/pricing\n  self_serve_key_issuance: false\nplatform_auth:\n  note: >-\n    Platform (not API) authentication is a username/password login at\n    https://app.giveffect.com,\
  \ and two-factor authentication was shipped to the\n    product as a 2025 update. This says nothing about how API callers\n    authenticate.\n  source: https://www.giveffect.com/nonprofit-resource-center/giveffect-2025-new-features/\nscopes:\n  applicable: false\n  note: >-\n    No OAuth surface exists, so scopes/ is skipped rather than written empty.\nx-evidence:\n- url: https://api.giveffect.com/v1/donors\n  http_status: 404\n  fetched: '2026-08-13'\n- url: https://www.giveffect.com/pricing\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://www.giveffect.com/api\n  http_status: 302\n  redirect_to: https://www.giveffect.com/signin\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giveffect/refs/heads/main/authentication/giveffect-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Non-Profit
- Fundraising
- CRM
- Donations
- Volunteer Management
- Marketing Automation
- Software-as-a-Service
---
