---
api_specs:
- filename: pointcheckout-merchant-api-openapi.yml
  format: yaml
  label: PointCheckout Merchant API
  slug: pointcheckout-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointcheckout/refs/heads/main/openapi/pointcheckout-merchant-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pointcheckout.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paymennt.com
  spf: true
hosts:
- host: pointcheckout.com
  https: false
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.paymennt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.test.paymennt.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pointcheckout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PointCheckout, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PointCheckout
provider_slug: pointcheckout
slug: pointcheckout-domain-security
source_filename: pointcheckout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pointcheckout.com\n  https: false\n- host: api.paymennt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\n- host: api.test.paymennt.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pointcheckout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: paymennt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointcheckout/refs/heads/main/security/pointcheckout-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Checkout
- Subscriptions
- Rewards
- Loyalty
- Webhooks
- MENA
- E-Commerce
---
