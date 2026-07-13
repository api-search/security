---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Feathery REST API
  slug: feathery-rest-api
  spec_type: OpenAPI
  url: https://api-docs.feathery.io/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: feathery.io
  spf: true
hosts:
- cert_expires: Oct  2 15:16:34 2026 GMT
  host: www.feathery.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 23:42:41 2026 GMT
  host: api-docs.feathery.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.feathery.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Feathery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feathery, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Feathery
provider_slug: feathery
slug: feathery-domain-security
source_filename: feathery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.feathery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:16:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.feathery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.feathery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: feathery.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/security/feathery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Form Builder
- Multi-Step Forms
- Document Intelligence
- AI
- Financial Services
- Insurance
- Wealth Management
- eSignature
- Workflows
- Data Intake
- Submissions
- Payments
- Authentication
---
