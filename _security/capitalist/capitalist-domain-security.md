---
api_specs:
- filename: capitalist-openapi.yml
  format: yaml
  label: Capitalist API
  slug: capitalist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: capitalist.net
  spf: true
hosts:
- cert_expires: Sep  5 07:29:09 2026 GMT
  host: capitalist.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 07:29:09 2026 GMT
  host: api.capitalist.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capitalist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capitalist, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Capitalist
provider_slug: capitalist
slug: capitalist-domain-security
source_filename: capitalist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capitalist.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 07:29:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.capitalist.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 07:29:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capitalist.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/security/capitalist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Bulk Payouts
- Cryptocurrency
- Finance
- Mass Payments
- Payment Platform
- Payments
- Payouts
- Remittance
---
