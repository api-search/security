---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Mai Authentication
name_suffix: Authentication
oauth_flows: []
overview: MAI declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: MAI
provider_slug: mai
scheme_count: 0
schemes: []
slug: mai-authentication
source_filename: mai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: >-\n  npm @mai-co/pixel@1.0.5 — dist/mai-pixel.es.js (transport + config modules),\n  dist/types.d.ts, dist/config.d.ts, and the published README integration guide\ndocs: https://www.npmjs.com/package/@mai-co/pixel\nsummary: >-\n  MAI's one publicly reachable API — the Pixel Event Collection endpoint at\n  POST https://pixel.mai.co/api/collect — is UNAUTHENTICATED. There is no API\n  key, no bearer token, no signature and no securityScheme of any kind. The\n  request carries no credential; the tenant is named in the body as a plaintext\n  Shopify store domain, and the visitor is identified by a first-party cookie\n  the SDK itself mints. Every other MAI surface (the Shopify embedded app, the\n  web application) sits behind Shopify OAuth or an application login that is not\n  publicly documented.\nsecurity_scheme_count: 0\nschemes: []\nmodel:\n  authenticated: false\n  credential: none\n  transport_security: TLS 1.3 (HTTPS enforced)\n\
  \  tenant_identification:\n    field: shop.myshopifyDomain\n    location: request body\n    source: MaiConfig.storeDomain, supplied by the embedding site\n    secret: false\n    note: >-\n      The store domain is configuration, not a credential. It is visible in page\n      source on every storefront that installs the pixel, so it identifies the\n      tenant but does not authenticate it.\n  subject_identification:\n    field: client_id\n    location: request body\n    source: '_mai_cid cookie — UUID v4 minted client-side, 2-year max-age'\n    note: >-\n      Anonymous pseudonymous identifier. Upgraded to a named identity only when\n      the merchant calls MaiPixel('setCustomer', ...) with an email or phone.\n  consent_gate:\n    mechanism: MaiPixel('consent', ...)\n    aligned_with: Shopify CustomerPrivacy API\n    fields:\n      - analytics_processing_allowed\n      - marketing_allowed\n      - preferences_processing_allowed\n      - sale_of_data_allowed\n    default: >-\n      Tracking\
  \ is ALLOWED by default. If consent() is never called the SDK sends\n      events. Setting analytics_processing_allowed to false halts all sends.\n    note: >-\n      This is the only client-side gate on the endpoint, and it is enforced in\n      the browser by the SDK — not by the server.\nobservations:\n  - >-\n    Because the endpoint is unauthenticated and accepts a caller-supplied store\n    domain, nothing in the published contract prevents a third party from\n    posting events attributed to another merchant's store. MAI may apply\n    server-side validation that is not visible from the client bundle; none is\n    documented.\n  - >-\n    The SDK sends the body with Content-Type text/plain (both the\n    navigator.sendBeacon Blob and the XHR fallback), which keeps the request a\n    CORS simple request and avoids a preflight. A consequence is that no\n    Authorization header could be added without changing that property.\n  - >-\n    MaiConfig exposes an apiEndpoint override documented\
  \ as \"for debug/staging\n    only\", so the collection host is configurable by the embedding site.\ngaps:\n  - No published authentication documentation for any MAI API.\n  - No OAuth 2.0 / OpenID Connect metadata on any host (all /.well-known/ probes miss).\n  - No API key issuance, rotation, or revocation story is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mai/refs/heads/main/authentication/mai-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Artificial Intelligence
- Marketing
- Advertising
- Performance Marketing
- AI Agents
- Digital Advertising
- MarTech
- Google Ads
- Shopify
- E-Commerce
- Attribution
- Analytics
- Event Tracking
---
