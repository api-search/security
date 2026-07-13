---
api_specs:
- filename: salla-merchant-api-openapi.yml
  format: yaml
  label: Salla Merchant API
  slug: salla-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-merchant-api-openapi.yml
- filename: salla-apps-api-openapi.yml
  format: yaml
  label: Salla Apps API
  slug: salla-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-apps-api-openapi.yml
- filename: salla-shipping-fulfillment-api-openapi.yml
  format: yaml
  label: Salla Shipping and Fulfillment API
  slug: salla-shipping-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-shipping-fulfillment-api-openapi.yml
- filename: salla-webhooks-asyncapi.yml
  format: yaml
  label: Salla Webhooks
  slug: salla-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/openapi/salla-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salla.com
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: salla.dev
  spf: true
hosts:
- cert_expires: Sep 19 08:34:23 2026 GMT
  host: salla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:29:42 2026 GMT
  host: docs.salla.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:29:42 2026 GMT
  host: api.salla.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salla, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salla
provider_slug: salla
slug: salla-domain-security
source_filename: salla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: salla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:34:23 2026 GMT\n  hsts: null\n- host: docs.salla.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:29:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.salla.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:29:42 2026 GMT\n  hsts: null\ndomains:\n- domain: salla.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: salla.dev\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\
  \n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/security/salla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Arabic
- E-Commerce
- GCC
- Headless Commerce
- Merchant
- MENA
- Online Stores
- Retail
- Saudi Arabia
- SMB
- Storefront
---
