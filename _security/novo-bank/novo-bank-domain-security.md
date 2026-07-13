---
api_specs:
- filename: novo-bank-openapi.yml
  format: yaml
  label: Novo Accounts
  slug: novo-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novo-bank/refs/heads/main/openapi/novo-bank-openapi.yml
- filename: novo-bank-openapi.yml
  format: yaml
  label: Novo Transactions
  slug: novo-transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novo-bank/refs/heads/main/openapi/novo-bank-openapi.yml
- filename: novo-bank-openapi.yml
  format: yaml
  label: Novo Payments
  slug: novo-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novo-bank/refs/heads/main/openapi/novo-bank-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: novo.co
  spf: true
hosts:
- cert_expires: Sep 22 11:45:12 2026 GMT
  host: www.novo.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novo Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Novo
provider_slug: novo-bank
slug: novo-bank-domain-security
source_filename: novo-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.novo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:45:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: novo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novo-bank/refs/heads/main/security/novo-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Business Banking
- Fintech
- Small Business
- Freelancers
- Payments
---
