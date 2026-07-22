---
api_specs:
- filename: modernfi-openapi-original.json
  format: json
  label: ModernFi Digital Banking API
  slug: modernfi-digital-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/openapi/modernfi-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modernfi.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.modernfi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.uat.modernfi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 16:11:40 2026 GMT
  host: auth.modernfi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modernfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModernFi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ModernFi
provider_slug: modernfi
slug: modernfi-domain-security
source_filename: modernfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.modernfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\n- host: api.uat.modernfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\n- host: auth.modernfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 16:11:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: modernfi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modernfi/refs/heads/main/security/modernfi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Deposits
- Fintech
- Credit Unions
- Financial Services
- Deposit Network
- Treasury
---
