---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Fevo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fevo declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Fevo
provider_slug: fevo
scheme_count: 3
schemes:
- api: FEVO Order API
  credentials:
  - description: Identifies the requesting team. An organization that manages more than one team receives a distinct User ID per team.
    name: User ID
  - description: The secret paired with the User ID. Distinct per team.
    name: Access Key
  docs: https://intercom.help/fevoenterprise/en/articles/8912590-api-faqs
  failure_mode: 'FEVO documents that an HTTP 502 Server Error means the credentials are wrong, specifically the User ID when an organization manages more than one key. Returning a gateway status for an authentication failure is a defect on its own terms: 502 is indistinguishable from a genuine upstream outage, and FEVO''s own CDN was in fact returning 502 across www.fevo.com/api/v1 and sdk.fevo.com on 2026-08-12.'
  id: order-api-user-id-access-key
  issuance: '"Connect with your FEVO Representative to capture your unique User ID(s) and Access Key(s) in order to connect." There is no self-service key issuance, no developer console for keys, and no documented key lifecycle.'
  location: not published
  model: static credential pair
  reference_note: '"Order API definitions" are linked from the FAQ to a Salesforce content-delivery URL (fevo.my.salesforce.com/sfc/p/...). Probed 2026-08-12: HTTP 200 but the body is a 1,359-byte Salesforce contentDistribution shell with x-robots-tag noindex,nofollow — a JavaScript-rendered viewer, not a fetchable document.'
  revocation: not published
  rotation_policy: not published
  scopes: none published
  transport: not published
  type: apiKey
- api: Fevo Button SDK (legacy)
  credentials:
  - description: Passed to Fevo.init({ publisherKey, env }). Public by construction — it ships in the page source. Issued by a FEVO account manager.
    name: publisherKey
  - description: Environment selector; 'prod' is the documented value.
    name: env
  docs: https://www.fevo.com/docs/v1
  id: fevojs-publisher-key
  issuance: contact your FEVO account manager
  model: public publishable key, browser-side
  rotation_policy: not published
  scopes: none published
  status_note: https://www.fevo.com/docs/v1 returned HTTP 502 on 2026-08-12.
  transport: JavaScript initialization argument, embedded in the host page
  type: apiKey
- api: FEVO Embedded Checkout (Distributed Commerce Button)
  docs: https://intercom.help/fevoenterprise/en/articles/8986183-distributed-commerce-button
  id: gmwidget-domain-allowlist
  issuance: Send the embedding URL to your FEVO Success Rep or to marketingservices@fevo.com.
  model: No credential at all. The Distributed Commerce Button carries no key; authorization is enforced by FEVO allow-listing the embedding domain. "If you have not implemented the FEVO drawer on your website before, your domain may need to be whitelisted."
  rotation_policy: not applicable
  scopes: none
  type: origin-allowlist
slug: fevo-authentication
source_filename: fevo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://intercom.help/fevoenterprise/en/articles/8912590-api-faqs (Order API),\n  https://intercom.help/fevoenterprise/en/articles/8986183-distributed-commerce-button\n  (embed), https://www.fevo.com/docs/v1 (legacy Fevo.js publisher key, page currently 502)\nnote: >-\n  Derived from no OpenAPI — FEVO publishes no machine-readable contract, so every scheme\n  below is transcribed from the provider's own prose documentation. No OAuth 2.0, no\n  OpenID Connect, no scopes, no token endpoint and no key-rotation or revocation guidance\n  is published anywhere on FEVO's public surface. Credential issuance is a human process\n  routed through a FEVO representative.\n\nschemes:\n\n  - id: order-api-user-id-access-key\n    api: FEVO Order API\n    type: apiKey\n    model: static credential pair\n    credentials:\n      - name: User ID\n        description: >-\n          Identifies the requesting team. An organization that manages\
  \ more than one team\n          receives a distinct User ID per team.\n      - name: Access Key\n        description: The secret paired with the User ID. Distinct per team.\n    issuance: >-\n      \"Connect with your FEVO Representative to capture your unique User ID(s) and Access\n      Key(s) in order to connect.\" There is no self-service key issuance, no developer\n      console for keys, and no documented key lifecycle.\n    transport: not published\n    location: not published\n    rotation_policy: not published\n    revocation: not published\n    scopes: none published\n    failure_mode: >-\n      FEVO documents that an HTTP 502 Server Error means the credentials are wrong,\n      specifically the User ID when an organization manages more than one key. Returning a\n      gateway status for an authentication failure is a defect on its own terms: 502 is\n      indistinguishable from a genuine upstream outage, and FEVO's own CDN was in fact\n      returning 502 across www.fevo.com/api/v1\
  \ and sdk.fevo.com on 2026-08-12.\n    docs: https://intercom.help/fevoenterprise/en/articles/8912590-api-faqs\n    reference_note: >-\n      \"Order API definitions\" are linked from the FAQ to a Salesforce content-delivery URL\n      (fevo.my.salesforce.com/sfc/p/...). Probed 2026-08-12: HTTP 200 but the body is a\n      1,359-byte Salesforce contentDistribution shell with x-robots-tag noindex,nofollow\n      — a JavaScript-rendered viewer, not a fetchable document.\n\n  - id: fevojs-publisher-key\n    api: Fevo Button SDK (legacy)\n    type: apiKey\n    model: public publishable key, browser-side\n    credentials:\n      - name: publisherKey\n        description: >-\n          Passed to Fevo.init({ publisherKey, env }). Public by construction — it ships in\n          the page source. Issued by a FEVO account manager.\n      - name: env\n        description: Environment selector; 'prod' is the documented value.\n    issuance: contact your FEVO account manager\n    transport: JavaScript\
  \ initialization argument, embedded in the host page\n    rotation_policy: not published\n    scopes: none published\n    docs: https://www.fevo.com/docs/v1\n    status_note: https://www.fevo.com/docs/v1 returned HTTP 502 on 2026-08-12.\n\n  - id: gmwidget-domain-allowlist\n    api: FEVO Embedded Checkout (Distributed Commerce Button)\n    type: origin-allowlist\n    model: >-\n      No credential at all. The Distributed Commerce Button carries no key; authorization\n      is enforced by FEVO allow-listing the embedding domain. \"If you have not implemented\n      the FEVO drawer on your website before, your domain may need to be whitelisted.\"\n    issuance: >-\n      Send the embedding URL to your FEVO Success Rep or to marketingservices@fevo.com.\n    rotation_policy: not applicable\n    scopes: none\n    docs: https://intercom.help/fevoenterprise/en/articles/8986183-distributed-commerce-button\n\nsummary:\n  oauth2: false\n  openid_connect: false\n  api_key: true\n  mutual_tls: false\n\
  \  scopes_published: false\n  self_service_credentials: false\n  credential_issuance: human, via a FEVO representative\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fevo/refs/heads/main/authentication/fevo-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Ticketing
- Events
- Group Sales
- Social Commerce
- E-Commerce
- Checkout
- Sports
- Live Entertainment
- Embedded Commerce
---
