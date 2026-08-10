---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Red Canary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Red Canary secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Red Canary
provider_slug: red-canary
scheme_count: 1
schemes:
- description: Per-user API authentication token. Generated from the Red Canary portal under the user profile -> Security Settings -> "Generate API Authentication Token". The token inherits the roles/permissions of the user who created it, so API authorization is role-based rather than scope-based.
  in: header
  name: X-Api-Key
  parameter_name: X-Api-Key
  sources:
  - https://docs.redcanary.com/docs/red-canary-rest-api
  - https://github.com/redcanaryco/openapi/blob/master/python/redcanary/rest.py
  type: apiKey
slug: red-canary-authentication
source_filename: red-canary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/ has no spec — derived from the provider's own published documentation\ndocs: https://docs.redcanary.com/docs/red-canary-rest-api\nnotes: >-\n  No OpenAPI document is publicly reachable, so this profile is read from Red Canary's\n  public REST API documentation and from its own first-party Python client\n  (https://github.com/redcanaryco/openapi), not from a securitySchemes block.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter_name: X-Api-Key\n  description: >-\n    Per-user API authentication token. Generated from the Red Canary portal under the\n    user profile -> Security Settings -> \"Generate API Authentication Token\". The token\n    inherits the roles/permissions of the user who created it, so API authorization is\n    role-based rather than scope-based.\n  sources:\n  - https://docs.redcanary.com/docs/red-canary-rest-api\n\
  \  - https://github.com/redcanaryco/openapi/blob/master/python/redcanary/rest.py\ntoken_management:\n  scope: per-user\n  rotation: >-\n    Generating a new token revokes any existing token for that user. Red Canary advises\n    periodic rotation.\n  docs: https://docs.redcanary.com/docs/rest-api-faq\n  revocation: implicit on regeneration\ntenancy:\n  model: subdomain\n  host_template: https://<subdomain>.my.redcanary.co/openapi/v3/\n  note: >-\n    Every API call is bound to the customer's own portal subdomain; there is no shared\n    global API host. https://go.my.redcanary.co/ is the subdomain selector / login gate.\nportal_authentication:\n  note: >-\n    Human access to the portal (where the Swagger reference lives) is separate from API\n    token auth and supports SAML SSO and MFA.\n  sso:\n  - provider: Microsoft Entra ID\n    docs: https://docs.redcanary.com/docs/set-up-single-sign-on-to-microsoft-entra-id\n  - provider: Okta\n    docs: https://docs.redcanary.com/docs/set-up-single-sign-on-to-okta\n\
  \  - provider: OneLogin\n    docs: https://docs.redcanary.com/docs/set-up-single-sign-on-to-onelogin\n  - provider: Ping Identity\n    docs: https://docs.redcanary.com/docs/set-up-single-sign-on-to-ping-identity\n  mfa_docs: https://docs.redcanary.com/docs/configure-multi-factor-authentication-mfa\noauth:\n  present: false\n  note: >-\n    The REST API declares no OAuth 2.0 or OpenID Connect surface. No\n    /.well-known/oauth-authorization-server or /.well-known/openid-configuration is\n    served on any Red Canary host (all 404; see well-known/red-canary-well-known.yml).\n    scopes/ is therefore intentionally absent.\nx-evidence:\n  fetched: '2026-08-05'\n  urls:\n  - url: https://docs.redcanary.com/docs/red-canary-rest-api.md\n    http_status: 200\n  - url: https://docs.redcanary.com/docs/rest-api-faq.md\n    http_status: 200\n  - url: https://raw.githubusercontent.com/redcanaryco/openapi/master/python/redcanary/rest.py\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-canary/refs/heads/main/authentication/red-canary-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Threat Detection
- Threat Intelligence
- Endpoint Security
- Incident Response
- Security Operations
- Automation
---
