---
api_specs:
- filename: mastercard-gateway-api-openapi.yml
  format: yaml
  label: Mastercard Gateway API
  slug: mastercard-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-gateway-api/refs/heads/main/openapi/mastercard-gateway-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mastercard.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: developer.mastercard.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: ap-gateway.mastercard.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mastercard Gateway Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mastercard Gateway API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mastercard Gateway API
provider_slug: mastercard-gateway-api
slug: mastercard-gateway-api-domain-security
source_filename: mastercard-gateway-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.mastercard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: ap-gateway.mastercard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mastercard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastercard-gateway-api/refs/heads/main/security/mastercard-gateway-api-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Credit Cards
- Gateway
- Payment Processing
- Payments
---
