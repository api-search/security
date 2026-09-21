---
api_specs:
- filename: avis-budget-rental-cars-openapi.yml
  format: yaml
  label: Avis Budget Group Rental Cars API
  slug: avis-budget-group-rental-cars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avis-budget/refs/heads/main/openapi/avis-budget-rental-cars-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avisbudgetgroup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avis.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.avisbudgetgroup.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: developer.avis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: stage.abgapiservices.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Avis Budget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avis Budget Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Avis Budget Group
provider_slug: avis-budget
slug: avis-budget-domain-security
source_filename: avis-budget-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avisbudgetgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.avis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: stage.abgapiservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: avisbudgetgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: avis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avis-budget/refs/heads/main/security/avis-budget-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Car Rental
- Travel
- Mobility
- Fleet Management
- Transportation
- Reservations
- Vehicle Rental
- Partner API
- Hospitality
---
