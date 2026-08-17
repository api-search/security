---
api_specs:
- filename: heron-openapi.json
  format: json
  label: Heron API
  slug: heron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heron/refs/heads/main/openapi/heron-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: herondata.io
  spf: true
hosts:
- cert_expires: Sep 21 22:58:04 2026 GMT
  host: www.herondata.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:12:21 2026 GMT
  host: docs.herondata.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:12:21 2026 GMT
  host: app.herondata.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heron, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Heron
provider_slug: heron
slug: heron-domain-security
source_filename: heron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.herondata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 22:58:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.herondata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:12:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.herondata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:12:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: herondata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heron/refs/heads/main/security/heron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Document Automation
- Underwriting
- Lending
- Cashflow Analytics
- Fintech
- Data Enrichment
- Bank Statements
- Transaction Enrichment
- Agent Ready
---
