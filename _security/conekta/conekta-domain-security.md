---
api_specs:
- filename: conekta-api-openapi.yml
  format: yaml
  label: Conekta API
  slug: conekta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conekta/refs/heads/main/openapi/conekta-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conekta.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conekta.io
  spf: false
hosts:
- cert_expires: Sep 30 05:30:15 2026 GMT
  host: www.conekta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 06:01:25 2026 GMT
  host: developers.conekta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.conekta.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conekta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conekta, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Conekta
provider_slug: conekta
slug: conekta-domain-security
source_filename: conekta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conekta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:30:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.conekta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:01:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.conekta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: conekta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: conekta.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conekta/refs/heads/main/security/conekta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Cards
- Cash
- OXXO
- SPEI
- Mexico
- Latin America
- LATAM
- Fintech
- Subscriptions
- Antifraud
- Checkout
- BNPL
- 3D Secure
---
