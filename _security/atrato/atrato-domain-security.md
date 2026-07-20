---
api_specs:
- filename: atrato-partners-openapi.yml
  format: yaml
  label: Atrato Partners API
  slug: atrato-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atrato/refs/heads/main/openapi/atrato-partners-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atratopago.com
  spf: true
hosts:
- cert_expires: Sep 10 19:19:30 2026 GMT
  host: www.atratopago.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atrato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atrato, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atrato
provider_slug: atrato
slug: atrato-domain-security
source_filename: atrato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atratopago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 19:19:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atratopago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atrato/refs/heads/main/security/atrato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Buy Now Pay Later
- Lending
- Mexico
- Point of Sale
- Ecommerce
---
