---
api_key_in: []
auth_types:
- account-issued-identifier
- out-of-band-credential-exchange
- interactive-login
description: ''
kind: authentication
layout: security
method: searched
name: Pebblepost Authentication
name_suffix: Authentication
oauth_flows: []
overview: PebblePost secures its APIs with account-issued-identifier, out-of-band-credential-exchange, and interactive-login across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PebblePost
provider_slug: pebblepost
scheme_count: 5
schemes:
- description: A PebblePost-issued Brand ID embedded in the site tag; it also selects the per-brand collector script path on cdn.pbbl.co. Not a secret and not an authenticated credential — it identifies the brand, it does not authorize a caller.
  in: client-side-variable
  issued_by: PebblePost
  name: brand-id
  parameter: _pp.brid
  self_serve: false
  source: https://docs.pebblepost.com/article/6-pebblepost-javascript-tag-installation-guide
  surface: PebblePost JavaScript Tag
  type: account-issued-identifier
- description: The brand creates a Shopify private application and sends the generated URL, key and password to their PebblePost Account Manager. PebblePost authenticates to Shopify with the brand's credentials; the brand never authenticates to PebblePost.
  direction: inbound-to-pebblepost
  name: shopify-private-app
  self_serve: false
  source: https://docs.pebblepost.com/article/36-connect-pebblepost-to-shopify
  surface: Shopify data connector
  type: out-of-band-credential-exchange
- description: Browser login to the PebblePost customer platform. Accounts are activated by PebblePost, not by self-registration; the help article covering access is an account-activation and password-help article, not a sign-up flow.
  name: pdm-manager-login
  self_serve: false
  source: https://docs.pebblepost.com/article/61-account-activation-login-help
  surface: PDM Manager (Performance Dashboard)
  type: interactive-login
  url: https://pdm.pebblepost.com/#/login
- description: 'AWS API Gateway. Every path — including / and /openapi.json — returns HTTP 403 with {"message":"Missing Authentication Token"} and header x-amzn-errortype: MissingAuthenticationTokenException. The token type, header name and issuance flow are not published. Recorded as observed behaviour only; NOT an assertion about the scheme in use.'
  name: api-gateway-token
  observed:
    body: '{"message":"Missing Authentication Token"}'
    http_status: 403
  self_serve: false
  surface: api.pbbl.co
  type: unknown-bearer
- description: An Express service. GET /health returns 200 {"status":"UP"}; every other probed path returns 404 with {"message":"Resource not found", "errorType":"ResourceNotFoundError"}. No authentication challenge was returned on any anonymous path, so the auth model could not be observed and is not asserted.
  name: platform-api
  observed:
    health_status: 200
    unknown_path_status: 404
  self_serve: false
  surface: api.pebblepost.com
  type: undocumented
slug: pebblepost-authentication
source_filename: pebblepost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://docs.pebblepost.com/\ndocs: https://docs.pebblepost.com/collection/58-performance-dashboard-access\n# DERIVED FROM NOTHING MECHANICAL: PebblePost publishes no OpenAPI, so\n# derive-authentication.py has no securitySchemes to read. Everything below was\n# observed directly against live hosts or read from PebblePost's own help articles.\nsummary:\n  types: [account-issued-identifier, out-of-band-credential-exchange, interactive-login]\n  oauth2: false\n  openid_connect: false\n  api_key_self_serve: false\n  public_api_reference: false\n  note: 'PebblePost operates no public developer program. There is no self-serve API\n    key issuance, no OAuth authorization server, and no published API reference. Every\n    credential is issued or exchanged through a PebblePost account team.'\nschemes:\n- name: brand-id\n  surface: PebblePost JavaScript Tag\n  type: account-issued-identifier\n  in: client-side-variable\n  parameter:\
  \ _pp.brid\n  issued_by: PebblePost\n  self_serve: false\n  description: 'A PebblePost-issued Brand ID embedded in the site tag; it also selects\n    the per-brand collector script path on cdn.pbbl.co. Not a secret and not an\n    authenticated credential — it identifies the brand, it does not authorize a caller.'\n  source: https://docs.pebblepost.com/article/6-pebblepost-javascript-tag-installation-guide\n- name: shopify-private-app\n  surface: Shopify data connector\n  type: out-of-band-credential-exchange\n  direction: inbound-to-pebblepost\n  self_serve: false\n  description: 'The brand creates a Shopify private application and sends the generated\n    URL, key and password to their PebblePost Account Manager. PebblePost authenticates\n    to Shopify with the brand''s credentials; the brand never authenticates to PebblePost.'\n  source: https://docs.pebblepost.com/article/36-connect-pebblepost-to-shopify\n- name: pdm-manager-login\n  surface: PDM Manager (Performance Dashboard)\n\
  \  type: interactive-login\n  url: https://pdm.pebblepost.com/#/login\n  self_serve: false\n  description: 'Browser login to the PebblePost customer platform. Accounts are\n    activated by PebblePost, not by self-registration; the help article covering access\n    is an account-activation and password-help article, not a sign-up flow.'\n  source: https://docs.pebblepost.com/article/61-account-activation-login-help\n- name: api-gateway-token\n  surface: api.pbbl.co\n  type: unknown-bearer\n  self_serve: false\n  description: 'AWS API Gateway. Every path — including / and /openapi.json — returns\n    HTTP 403 with {\"message\":\"Missing Authentication Token\"} and header\n    x-amzn-errortype: MissingAuthenticationTokenException. The token type, header name\n    and issuance flow are not published. Recorded as observed behaviour only; NOT an\n    assertion about the scheme in use.'\n  observed:\n    http_status: 403\n    body: '{\"message\":\"Missing Authentication Token\"}'\n- name: platform-api\n\
  \  surface: api.pebblepost.com\n  type: undocumented\n  self_serve: false\n  description: 'An Express service. GET /health returns 200 {\"status\":\"UP\"}; every\n    other probed path returns 404 with {\"message\":\"Resource not found\",\n    \"errorType\":\"ResourceNotFoundError\"}. No authentication challenge was returned on\n    any anonymous path, so the auth model could not be observed and is not asserted.'\n  observed:\n    health_status: 200\n    unknown_path_status: 404\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - {url: 'https://api.pebblepost.com/health', status: 200}\n  - {url: 'https://api.pebblepost.com/openapi.json', status: 404}\n  - {url: 'https://api.pbbl.co/', status: 403}\n  - {url: 'https://pdm.pebblepost.com/', status: 200}\n  - {url: 'https://www.pebblepost.com/.well-known/openid-configuration', status: 404}\nx-gap:\n  - 'No published authentication reference of any kind. A prospective integrator cannot\n    learn how to obtain a credential, which header\
  \ carries it, or what its lifetime is\n    without first talking to a salesperson. Publishing an auth page — even one that\n    says \"credentials are issued by your account team, sent as `Authorization: Bearer`\"\n    — would close the single largest gap in this profile.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pebblepost/refs/heads/main/authentication/pebblepost-authentication.yml
summary_line: account-issued-identifier/out-of-band-credential-exchange/interactive-login · 5 schemes
tags:
- Company
- Marketing
- Advertising
- Direct Mail
- Connected TV
- Retail
- Commerce
- Identity
- Analytics
---
