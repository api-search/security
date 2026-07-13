---
api_specs:
- filename: anrok-api-openapi.yml
  format: yaml
  label: Anrok API
  slug: anrok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anrok/refs/heads/main/openapi/anrok-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anrok.com
  spf: true
hosts:
- cert_expires: Sep 30 18:18:46 2026 GMT
  host: www.anrok.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 18:55:19 2026 GMT
  host: apidocs.anrok.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 06:29:11 2026 GMT
  host: api.anrok.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anrok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anrok, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anrok
provider_slug: anrok
slug: anrok-domain-security
source_filename: anrok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anrok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:18:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.anrok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:55:19 2026 GMT\n  hsts: false\n- host: api.anrok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:29:11 2026 GMT\n  hsts: null\ndomains:\n- domain: anrok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anrok/refs/heads/main/security/anrok-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Tax
- VAT
- Tax Compliance
- SaaS
- Fintech
- Tax Automation
- Nexus
- E-Invoicing
---
