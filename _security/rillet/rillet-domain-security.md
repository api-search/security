---
api_specs:
- filename: rillet-accounting-api-openapi.json
  format: json
  label: Rillet Accounting API
  slug: rillet-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rillet/refs/heads/main/openapi/rillet-accounting-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rillet.com
  spf: true
hosts:
- cert_expires: Oct 15 12:03:45 2026 GMT
  host: rillet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.rillet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: sandbox.api.rillet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rillet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rillet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rillet
provider_slug: rillet
slug: rillet-domain-security
source_filename: rillet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rillet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rillet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox.api.rillet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rillet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rillet/refs/heads/main/security/rillet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- ERP
- Accounting
- Finance
- General Ledger
- Accounts Receivable
- Accounts Payable
- Invoicing
- SaaS
---
