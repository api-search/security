---
api_specs:
- filename: apurata-acuotaz-pos-openapi.yml
  format: yaml
  label: Apurata aCuotaz POS REST API
  slug: apurata-acuotaz-pos-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apurata/refs/heads/main/openapi/apurata-acuotaz-pos-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apurata.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: apurata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: docs.apurata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apurata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apurata, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apurata
provider_slug: apurata
slug: apurata-domain-security
source_filename: apurata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apurata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\n- host: docs.apurata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: apurata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apurata/refs/heads/main/security/apurata-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- Buy Now Pay Later
- Installment Payments
- Consumer Credit
- Payments
- E-commerce
- Peru
- Latin America
---
