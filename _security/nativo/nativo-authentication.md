---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Nativo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nativo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Nativo
provider_slug: nativo
scheme_count: 2
schemes:
- applies_to: Nativo API V3 (https://api.nativo.com/v3)
  binding: per-user
  example_from_docs: 'curl -X GET "https://api.nativo.com" -H "Authorization: Bearer yourToken"'
  format: 'Authorization: Bearer <token>'
  header: Authorization
  id: personal_access_token
  in: header
  issuance: Generated from the User Edit page of the Nativo platform, under the API Access section ("Generate Token"), re-authenticated with the user's own account password.
  recommended_practice: Nativo recommends creating a dedicated API user rather than issuing a token against a person's login, for monitoring and control.
  rotation: Shown once at generation and never retrievable again. A misplaced token is replaced by generating a new one and disabling the old one. No expiry is documented.
  scheme: bearer
  type: http
- applies_to: Nativo Ad Serving API BETA (https://jadserve.postrelease.com/adsver/api)
  id: ad_serving_access
  in: n/a
  note: The published request examples carry only query parameters (visitor_id, user_ip, user_agent, page_url) and no credential. The docs state "Please contact your CSM to obtain access to the Ad Serving API" and that the target site URL must already exist in the Nativo system, so authorization appears to be by allow-listed site rather than by a request credential. Not verified — the endpoint was not called.
  type: none
slug: nativo-authentication
source_filename: nativo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://api-docs.nativo.com/docs/auth\ndocs: https://api-docs.nativo.com/docs/auth\nname: Nativo\nsummary: >-\n  The Nativo API V3 authenticates with a per-user Personal Access Token presented as an HTTP Bearer\n  credential. There is no OAuth 2.0, no OpenID Connect, no mTLS and no scope model — permissions are\n  carried by the platform role assigned to the user the token belongs to. The BETA Ad Serving API is\n  a separate surface with no documented request credential; access is provisioned out of band by a\n  Nativo CSM.\nschemes:\n- id: personal_access_token\n  type: http\n  scheme: bearer\n  applies_to: Nativo API V3 (https://api.nativo.com/v3)\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <token>'\n  example_from_docs: 'curl -X GET \"https://api.nativo.com\" -H \"Authorization: Bearer yourToken\"'\n  issuance: >-\n    Generated from the User Edit page of the Nativo platform, under the API Access\
  \ section\n    (\"Generate Token\"), re-authenticated with the user's own account password.\n  binding: per-user\n  rotation: >-\n    Shown once at generation and never retrievable again. A misplaced token is replaced by\n    generating a new one and disabling the old one. No expiry is documented.\n  recommended_practice: >-\n    Nativo recommends creating a dedicated API user rather than issuing a token against a person's\n    login, for monitoring and control.\n- id: ad_serving_access\n  type: none\n  applies_to: Nativo Ad Serving API BETA (https://jadserve.postrelease.com/adsver/api)\n  in: n/a\n  note: >-\n    The published request examples carry only query parameters (visitor_id, user_ip, user_agent,\n    page_url) and no credential. The docs state \"Please contact your CSM to obtain access to the\n    Ad Serving API\" and that the target site URL must already exist in the Nativo system, so\n    authorization appears to be by allow-listed site rather than by a request credential.\
  \ Not\n    verified — the endpoint was not called.\nauthorization_model:\n  style: role-based, platform-side\n  roles_published:\n  - Organizational Admin\n  - Campaign Manager\n  - Campaign Editor\n  - Publication Manager\n  - Reports Only\n  roles_source: https://ads.life360.com/legal/technical-organizational-measures\n  scopes: none\n  note: >-\n    Permission failures surface as HTTP 403 with a descriptive message; the site-targeting search\n    endpoint explicitly documents a 403 when a user queries an entity type their account cannot\n    access.\nnot_supported:\n- oauth2\n- openIdConnect\n- mutualTLS\n- apiKey query parameter\n- request signing / HMAC\nprobes:\n- url: https://api.nativo.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://api.nativo.com/.well-known/openid-configuration\n  status: 404\n- url: https://api.nativo.com/.well-known/oauth-protected-resource\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nativo/refs/heads/main/authentication/nativo-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- AdTech
- Native Advertising
- Programmatic Advertising
- Supply Side Platform
- Ad Serving
- Marketing
- Publishing
- Reporting
- Mobile SDK
---
