---
api_specs:
- filename: v2api.yaml
  format: yaml
  label: Sezzle API v2
  slug: sezzle-api-v2
  spec_type: OpenAPI
  url: https://gateway.sezzle.com/v2api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sezzle.com
  spf: true
hosts:
- cert_expires: Oct  6 14:10:33 2026 GMT
  host: docs.sezzle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 02:00:11 2026 GMT
  host: gateway.sezzle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 10:00:13 2026 GMT
  host: sandbox.gateway.sezzle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sezzle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sezzle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sezzle
provider_slug: sezzle
slug: sezzle-domain-security
source_filename: sezzle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.sezzle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:10:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gateway.sezzle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 02:00:11 2026 GMT\n  hsts: null\n- host: sandbox.gateway.sezzle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 10:00:13 2026 GMT\n  hsts: null\ndomains:\n- domain: sezzle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sezzle/refs/heads/main/security/sezzle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Buy Now Pay Later
- BNPL
- Payments
- Installments
- Fintech
- Merchant Integration
- Checkout
---
