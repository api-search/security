---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Dock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dock declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Dock
provider_slug: dock
scheme_count: 0
schemes: []
slug: dock-authentication
source_filename: dock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  live unauthenticated HTTP probes of https://api.caradhras.io, https://auth.caradhras.io and\n  https://developers.dock.tech on 2026-08-12\ndocumented_publicly: false\nnote: >-\n  Dock's authentication model is NOT publicly documented and this artifact does not claim\n  otherwise — no `Authentication` pointer is wired into apis.yml for this provider, because\n  the scoring check reads \"authentication is documented\" and it is not. What follows is only\n  what could be observed anonymously.\nschemes: []\nobserved:\n  challenge_status: 430\n  www_authenticate: false\n  error_type_header: 'x-dock-errortype: AuthorizationError'\n  body: '{\"error\": \"access denied\"}'\n  note: >-\n    The gateway rejects anonymous traffic before routing and returns no WWW-Authenticate\n    header, so a client cannot discover the scheme (apiKey vs http bearer vs oauth2) from the\n    wire at all.\ndiscovery_attempts:\n- url: https://auth.caradhras.io/.well-known/openid-configuration\n\
  \  status: 430\n- url: https://auth.caradhras.io/.well-known/oauth-authorization-server\n  status: 430\n- url: https://api.caradhras.io/.well-known/openid-configuration\n  status: 430\n- url: https://api.caradhras.io/oauth2/token\n  status: 430\n- url: https://developers.dock.tech/reference/\n  status: 302\n  redirect: https://dash.readme.com/to/dock-tech?redirect=%2Freference%2F\ninference:\n  auth_host_exists: true\n  auth_host: https://auth.caradhras.io\n  note: >-\n    A dedicated auth host resolves and serves TLS, which is consistent with a token-issuing\n    endpoint, but the scheme, grant types, and scope model are all unverifiable from outside.\n    Nothing is asserted.\nrecommendation_to_provider: >-\n  Publish the OAuth authorization-server metadata (or an OIDC discovery document) anonymously\n  and allow /.well-known/ through the WAF. Discovery documents are designed to be public and\n  gating them buys no security while making the API undiscoverable to every SDK generator and\n\
  \  agent runtime.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dock/refs/heads/main/authentication/dock-authentication.yml
summary_line: 0 schemes
tags:
- Banking
- Payments
- Cards
- Card Issuing
- Banking as a Service
- Financial-Services
- Fintech
- Pix
- Digital Accounts
- Acquiring
- Anti-Fraud
- Embedded Finance
- Brazil
- Latin America
---
