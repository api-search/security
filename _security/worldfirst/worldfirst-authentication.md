---
api_key_in:
- header
auth_types:
- signature
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Worldfirst Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: WorldFirst secures its APIs with signature and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: WorldFirst
provider_slug: worldfirst
scheme_count: 2
schemes:
- format: algorithm=RSA256,keyVersion=1,signature=<base64(sign(content))>
  header: Signature
  in: header
  key_management: Partner generates an RSA (or ECC) key pair and uploads the public key in the Developer Center Key Management section (separately for sandbox and production). WorldFirst signs its asynchronous notifications so the partner verifies them with WorldFirst's public key.
  name: RequestSignature
  required_headers:
  - Client-Id
  - Signature
  - request-time
  - Content-Type
  scheme: RSA256
  signed_content: '<HTTP-METHOD> <request-URI>

    <Client-Id>.<request-time>.<request-body>'
  sources:
  - docs: cashier_payment/getting_started
  type: signature
- description: The Enterprise Solution (World Account) additionally carries an OAuth 2.0 Access-Token obtained through partner authorization; the Pay Solution (Cashier Payment) is signature-only. Scopes are not published in the public docs.
  name: OAuth2AccessToken
  scheme: bearer
  sources:
  - docs: worldfirst_enterprise_solution/api_overview
  type: oauth2
slug: worldfirst-authentication
source_filename: worldfirst-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://developers.worldfirst.com/docs/alipay-worldfirst/cashier_payment/getting_started\ndocs: https://developers.worldfirst.com/docs/alipay-worldfirst/overview/apis\nnote: >-\n  WorldFirst does not publish a downloadable OpenAPI, so this profile is captured\n  from the developer documentation rather than derived from a spec. The gateway is\n  Ant Group's Antom-style platform (open-sea/open-eu/open-na hosts, /amsin/api/v1\n  paths). Every request is authenticated with an asymmetric digital signature; an\n  OAuth 2.0 access token is additionally used on the Enterprise Solution.\nsummary:\n  types: [signature, oauth2]\n  signature_algorithms: [RSA256, ECC224]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: RequestSignature\n  type: signature\n  scheme: RSA256\n  in: header\n  header: Signature\n  format: \"algorithm=RSA256,keyVersion=1,signature=<base64(sign(content))>\"\n  signed_content: \"\
  <HTTP-METHOD> <request-URI>\\n<Client-Id>.<request-time>.<request-body>\"\n  key_management: >-\n    Partner generates an RSA (or ECC) key pair and uploads the public key in the\n    Developer Center Key Management section (separately for sandbox and production).\n    WorldFirst signs its asynchronous notifications so the partner verifies them\n    with WorldFirst's public key.\n  required_headers:\n  - Client-Id        # merchant/partner identifier issued in the Developer Center\n  - Signature        # RSA256/ECC224 signature over the canonical request\n  - request-time     # request timestamp (replay protection)\n  - Content-Type     # application/json\n  sources: [docs: cashier_payment/getting_started]\n- name: OAuth2AccessToken\n  type: oauth2\n  scheme: bearer\n  description: >-\n    The Enterprise Solution (World Account) additionally carries an OAuth 2.0\n    Access-Token obtained through partner authorization; the Pay Solution (Cashier\n    Payment) is signature-only. Scopes are\
  \ not published in the public docs.\n  sources: [docs: worldfirst_enterprise_solution/api_overview]\nalternatives:\n  ecc224: >-\n    ECC224 is supported as an alternative to RSA256 for the request signature; the\n    Signature header algorithm token changes accordingly (algorithm=ECC224,...).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldfirst/refs/heads/main/authentication/worldfirst-authentication.yml
summary_line: signature/oauth2 · 2 schemes
tags:
- Payments
- United Kingdom
- Cross-Border
- Money Transfer
- Foreign Exchange
- Payouts
- Payment Gateway
- E-commerce
- Multi-Currency
- Card Issuing
---
