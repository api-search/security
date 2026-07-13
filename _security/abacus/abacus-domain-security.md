---
api_specs:
- filename: abacus-api-openapi.yaml
  format: yaml
  label: Abacus API
  slug: abacus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/openapi/abacus-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abacus.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.abacus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 25 20:27:51 2026 GMT
  host: support.abacus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.abacus.com
  https: false
kind: domain-security
layout: security
method: probed
name: Abacus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abacus, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Abacus
provider_slug: abacus
slug: abacus-domain-security
source_filename: abacus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abacus.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.abacus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:27:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.abacus.com\n  https: false\ndomains:\n- domain: abacus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/security/abacus-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
---
