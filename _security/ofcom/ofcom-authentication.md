---
api_key_in:
- header
- query
api_specs:
- filename: ofcom-connected-nations-broadband-api-openapi.yml
  format: yaml
  label: Ofcom Connected Nations Broadband API
  slug: ofcom-connected-nations-broadband-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofcom/refs/heads/main/openapi/ofcom-connected-nations-broadband-api-openapi.yml
- filename: ofcom-connected-nations-mobile-api-openapi.yml
  format: yaml
  label: Ofcom Connected Nations Mobile API
  slug: ofcom-connected-nations-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofcom/refs/heads/main/openapi/ofcom-connected-nations-mobile-api-openapi.yml
auth_types:
- apiKey
description: 'Azure API Management subscription key, and nothing else. There is no OAuth, no

  OpenID Connect, no mTLS and no bearer-token option anywhere in Ofcom''s surface —

  /.well-known/openid-configuration and /.well-known/oauth-authorization-server both

  return 404 on every Ofcom host. Keys are scoped to a PRODUCT, not to the provider:

  a Broadband key does not call the Mobile API. Issuance is self-serve to request but

  human-approved to grant.

  '
kind: authentication
layout: security
method: searched
name: Ofcom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ofcom secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ofcom
provider_slug: ofcom
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/ofcom-connected-nations-broadband-api-openapi.yml
  - openapi/ofcom-connected-nations-mobile-api-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/ofcom-connected-nations-broadband-api-openapi.yml
  - openapi/ofcom-connected-nations-mobile-api-openapi.yml
  type: apiKey
slug: ofcom-authentication
source_filename: ofcom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/ofcom-connected-nations-broadband-api-openapi.yml, openapi/ofcom-connected-nations-mobile-api-openapi.yml\ndocs: https://api.ofcom.org.uk/\nevidence:\n- source: https://api.ofcom.org.uk/mapi/apis?api-version=2021-08-01\n  status: 200\n  finding: >-\n    Both APIs report subscriptionRequired=true, authenticationSettings.oAuth2=null,\n    authenticationSettings.openid=null and\n    subscriptionKeyParameterNames={header: Ocp-Apim-Subscription-Key,\n    query: subscription-key, bearer: null}. Confirms API-key-only, anonymously.\n- source: https://api.ofcom.org.uk/mapi/products?api-version=2021-08-01\n  status: 200\n  finding: All four products carry subscriptionRequired=true and approvalRequired=true.\n- source: https://api-proxy.ofcom.org.uk/broadband/coverage/SW1A1AA\n  status: 401\n  finding: 'Anonymous call returns \"Access denied due to missing subscription key.\"'\ndescription: |\n  Azure API Management subscription\
  \ key, and nothing else. There is no OAuth, no\n  OpenID Connect, no mTLS and no bearer-token option anywhere in Ofcom's surface —\n  /.well-known/openid-configuration and /.well-known/oauth-authorization-server both\n  return 404 on every Ofcom host. Keys are scoped to a PRODUCT, not to the provider:\n  a Broadband key does not call the Mobile API. Issuance is self-serve to request but\n  human-approved to grant.\nissuance:\n  sign_up: https://api.ofcom.org.uk/signup\n  sign_in: https://api.ofcom.org.uk/signin\n  self_serve: true\n  approval_required: true\n  approval_note: >-\n    All four products are approvalRequired=true — an Ofcom person approves the\n    subscription before a key is issued. Discovery, documentation and OpenAPI\n    download are anonymous; only key issuance is gated.\n  key_scope: per product (broadband, broadband-premium, mobile, mobile-premium)\n  support: cnapisupport@ofcom.org.uk\noauth: false\noidc: false\nmtls: false\nscopes: false\nscopes_note: >-\n  No OAuth\
  \ scope surface exists — this is a key-auth API, so scopes/ is\n  deliberately absent rather than empty.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/ofcom-connected-nations-broadband-api-openapi.yml\n  - openapi/ofcom-connected-nations-mobile-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/ofcom-connected-nations-broadband-api-openapi.yml\n  - openapi/ofcom-connected-nations-mobile-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofcom/refs/heads/main/authentication/ofcom-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Telecommunications
- United Kingdom
- Regulator
- Broadband
- Mobile Network Coverage
- Spectrum
- Open Data
- Connected Nations
---
