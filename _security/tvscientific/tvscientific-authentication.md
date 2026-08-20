---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Tvscientific Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tvscientific declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tvscientific
provider_slug: tvscientific
scheme_count: 2
schemes:
- confirmed: false
  evidence:
    body: '{"detail":"Authentication credentials were not provided."}'
    status: 403
    url: https://api.tvscientific.app/v1/campaigns/
  id: unidentified
  note: Django REST Framework returns 403 with this message when no authentication class successfully authenticated the request AND none of them advertises a challenge. Because no WWW-Authenticate header is sent, the accepted credential type cannot be named from outside. Recorded as unidentified rather than guessed.
  type: unknown
- confidence: medium
  confirmed: false
  evidence:
    header: 'Vary: Accept, Cookie, origin'
    url: https://api.tvscientific.app/v1/
  id: session-cookie
  note: The API varies its response on the Cookie header, which means a session cookie is at least one of the inputs to authorization. This is consistent with the Campaign Management UI at https://tvscientific.app calling this API with a session. It does not rule out a token or key scheme also being accepted.
  type: cookie
slug: tvscientific-authentication
source_filename: tvscientific-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  Anonymous probes of https://api.tvscientific.app on 2026-08-12. No OpenAPI securitySchemes\n  exist to derive from (tvScientific publishes no spec) and no public authentication\n  documentation exists to search, so this profile is what the wire actually showed.\napi: tvScientific Campaign Management API\ndocs: null\ndocs_note: >-\n  There is no public auth page. help.tvscientific.com 301s to an Atlassian Service Desk\n  login (https://tvscientific.atlassian.net/servicedesk/customer/portal/2/user/login) and\n  support.tvscientific.com redirects into a Salesforce Community SAML request, so any\n  authentication guide tvScientific has written sits behind a customer login.\nposture: credentialed\npublic_access: partial\npublic_access_detail: >-\n  The version root indexes (/v1/, /v2/), the health endpoint (/health) and one collection\n  (/v1/terms_and_conditions/) are readable anonymously. Everything else — campaigns,\n  creatives,\
  \ lineitems, audiences, advertisers, billing, users — requires credentials.\nschemes:\n- id: unidentified\n  type: unknown\n  confirmed: false\n  evidence:\n    status: 403\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n    url: https://api.tvscientific.app/v1/campaigns/\n  note: >-\n    Django REST Framework returns 403 with this message when no authentication class\n    successfully authenticated the request AND none of them advertises a challenge. Because\n    no WWW-Authenticate header is sent, the accepted credential type cannot be named from\n    outside. Recorded as unidentified rather than guessed.\n- id: session-cookie\n  type: cookie\n  confirmed: false\n  confidence: medium\n  evidence:\n    header: 'Vary: Accept, Cookie, origin'\n    url: https://api.tvscientific.app/v1/\n  note: >-\n    The API varies its response on the Cookie header, which means a session cookie is at\n    least one of the inputs to authorization. This is consistent with the\
  \ Campaign Management\n    UI at https://tvscientific.app calling this API with a session. It does not rule out a\n    token or key scheme also being accepted.\noauth2: false\noidc: false\nmutual_tls: false\nnegative_probes:\n  # every published OAuth/OIDC/token discovery surface MISSED\n- url: https://api.tvscientific.app/.well-known/oauth-authorization-server\n  status: 404\n- url: https://api.tvscientific.app/.well-known/openid-configuration\n  status: 404\n- url: https://api.tvscientific.app/.well-known/oauth-protected-resource\n  status: 404\n- url: https://api.tvscientific.app/o/token/\n  status: 404\n- url: https://api.tvscientific.app/o/authorize/\n  status: 404\n- url: https://api.tvscientific.app/token/\n  status: 404\n- url: https://api.tvscientific.app/api-token-auth/\n  status: 404\n- url: https://api.tvscientific.app/v1/auth/\n  status: 404\n- url: https://api.tvscientific.app/v1/login/\n  status: 404\n- url: https://api.tvscientific.app/v1/register/\n  status: 404\nscopes:\
  \ null\nscopes_note: >-\n  No OAuth surface exists, so there is no scope vocabulary to capture and no\n  scopes/ artifact is written. Authorization appears to be tenant- and role-based —\n  /v1/tenants/, /v1/organizations/, /v1/organization_users/, /v1/user_types/ and\n  /v1/advertiser_users/ are all first-class collections — but the model is not published.\nonboarding:\n  self_serve: false\n  path: >-\n    Access is arranged through the tvScientific account team. The public site offers a demo\n    request (https://www.tvscientific.com/ctv-demo) and a contact form\n    (https://www.tvscientific.com/contact); there is no developer sign-up, no API key\n    self-issuance page and no public credential lifecycle documentation.\npointer_emitted: false\npointer_note: >-\n  No `type: Authentication` pointer is wired into apis.yml. The scorer's check is\n  `authentication_documented`, and tvScientific documents nothing publicly — this artifact\n  records an observed 403 and a named absence, not\
  \ a provider-published auth guide. Emitting\n  the pointer would credit tvScientific with auth documentation it has not published. Same\n  rule as the well-known and agent-card probes: the pointer asserts the PROVIDER serves the\n  surface.\ngaps:\n- No public authentication documentation.\n- No WWW-Authenticate challenge, so the scheme is undiscoverable from the wire.\n- 403 returned where 401 is semantically correct for a missing credential.\n- No OAuth 2.0 or OpenID Connect metadata document on any host.\n- No documented key rotation, expiry or revocation policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvscientific/refs/heads/main/authentication/tvscientific-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- Connected TV
- CTV
- Streaming
- Performance Marketing
- AdTech
- Measurements
- Campaign Management
- Real-Time Bidding
- Attribution
---
