---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gojek.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gobiz.com
  spf: false
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.gojek.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: developer.gobiz.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.gobiz.co.id
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gojek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoJek, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GoJek
provider_slug: gojek
slug: gojek-domain-security
source_filename: gojek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gojek.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\n- host: developer.gobiz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: api.gobiz.co.id\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gojek.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gobiz.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojek/refs/heads/main/security/gojek-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Super App
- Ride Hailing
- Food Delivery
- Point of Sale
- Merchant Platform
- Payments
- QRIS
- Logistics
- Indonesia
- Southeast Asia
- Webhooks
- OAuth
---
