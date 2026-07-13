---
api_specs:
- filename: basiq-api-openapi.yml
  format: yaml
  label: Basiq API
  slug: basiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  - 0 issue "usertrust.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: basiq.io
  spf: true
hosts:
- cert_expires: Sep  9 00:32:57 2026 GMT
  host: basiq.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: dashboard.basiq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:30:57 2026 GMT
  host: api.basiq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basiq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Basiq
provider_slug: basiq
slug: basiq-domain-security
source_filename: basiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basiq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:32:57 2026 GMT\n  hsts: false\n- host: dashboard.basiq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.basiq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:30:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: basiq.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issue \"usertrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/security/basiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
---
