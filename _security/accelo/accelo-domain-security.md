---
api_specs:
- filename: accelo-openapi.yml
  format: yaml
  label: Accelo REST API
  slug: accelo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: accelo.com
  spf: true
hosts:
- cert_expires: Sep 28 21:09:13 2026 GMT
  host: www.accelo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.accelo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accelo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accelo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Accelo
provider_slug: accelo
slug: accelo-domain-security
source_filename: accelo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:09:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.accelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: accelo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/security/accelo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Professional Services Automation
- Project Management
- CRM
- Time Tracking
- Invoicing
- Service Operations
---
