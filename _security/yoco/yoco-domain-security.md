---
api_specs:
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Checkout API
  slug: yoco-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Refunds API
  slug: yoco-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Webhooks API
  slug: yoco-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Payments API
  slug: yoco-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Payment Links API
  slug: yoco-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: reject
  dnssec: false
  domain: yoco.com
  spf: not_probed
hosts:
- cert_expires: Aug 17 22:44:48 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  cert_not_before: May 19 21:44:52 2026 GMT
  host: payments.yoco.com
  hsts: not observed on 303 response
  http_version: HTTP/2
  https: true
  note: Checkout API and webhooks host. Root path returns 303.
  tls_versions:
  - TLSv1.2
  - TLSv1.3
- cert_expires: Aug 17 22:44:48 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  cert_not_before: May 19 21:44:52 2026 GMT
  host: api.yoco.com
  hsts: not observed on 303 response
  http_version: HTTP/2
  https: true
  note: Versioned Yoco API (v1) host. Root path returns 303.
- cert_expires: Aug 17 22:44:48 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  cert_not_before: May 19 21:44:52 2026 GMT
  host: developer.yoco.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_version: HTTP/2
  https: true
  note: Developer hub (Fern-hosted docs).
- cert_expires: Aug 17 22:44:48 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  cert_not_before: May 19 21:44:52 2026 GMT
  host: yoco.com
  hsts: not observed on 301 response
  http_version: HTTP/2
  https: true
  note: Marketing root; redirects (301).
kind: domain-security
layout: security
method: probed
name: Yoco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yoco, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yoco
provider_slug: yoco
slug: yoco-domain-security
source_filename: yoco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payments.yoco.com\n  https: true\n  http_version: HTTP/2\n  tls_versions:\n  - TLSv1.2\n  - TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_not_before: May 19 21:44:52 2026 GMT\n  cert_expires: Aug 17 22:44:48 2026 GMT\n  hsts: not observed on 303 response\n  note: Checkout API and webhooks host. Root path returns 303.\n- host: api.yoco.com\n  https: true\n  http_version: HTTP/2\n  cert_issuer: Google Trust Services (WE1)\n  cert_not_before: May 19 21:44:52 2026 GMT\n  cert_expires: Aug 17 22:44:48 2026 GMT\n  hsts: not observed on 303 response\n  note: Versioned Yoco API (v1) host. Root path returns 303.\n- host: developer.yoco.com\n  https: true\n  http_version: HTTP/2\n  cert_issuer: Google Trust Services (WE1)\n  cert_not_before: May 19 21:44:52 2026 GMT\n  cert_expires: Aug 17 22:44:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains:\
  \ true\n  hsts_preload: true\n  note: Developer hub (Fern-hosted docs).\n- host: yoco.com\n  https: true\n  http_version: HTTP/2\n  cert_issuer: Google Trust Services (WE1)\n  cert_not_before: May 19 21:44:52 2026 GMT\n  cert_expires: Aug 17 22:44:48 2026 GMT\n  hsts: not observed on 301 response\n  note: Marketing root; redirects (301).\ndomains:\n- domain: yoco.com\n  dnssec: false\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_pct: 100\n  caa:\n  - '0 issuewild \"comodoca.com\"'\n  - '0 issuewild \"digicert.com; cansignhttpexchanges=yes\"'\n  - '0 issuewild \"letsencrypt.org\"'\n  spf: not_probed\nnotes: >-\n  All four probed hosts presented the same Google Trust Services (WE1)\n  certificate (consistent with a wildcard *.yoco.com), TLS 1.2 and 1.3, over\n  HTTP/2. HSTS with a two-year max-age, includeSubDomains, and preload was\n  observed on developer.yoco.com; it was not present on the redirect responses\n  from the API hosts at probe time. yoco.com publishes a strict DMARC policy\n\
  \  (p=reject, pct=100) and a CAA record limiting issuance. _dmarc / CAA lookups\n  on the API subdomains returned no records at probe time (they inherit the\n  organizational domain policy). Probes run 2026-07-12.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/security/yoco-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Payments
- Fintech
- Payment Gateway
- Card Payments
- South Africa
- Online Payments
- Checkout
- Point of Sale
- SMB
- Financial Infrastructure
---
