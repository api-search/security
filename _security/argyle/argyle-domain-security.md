---
api_specs:
- filename: api-reference
  format: yaml
  label: Argyle API
  slug: argyle-api
  spec_type: OpenAPI
  url: https://docs.argyle.com/api-reference
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: argyle.com
  spf: true
hosts:
- cert_expires: Aug 25 11:43:24 2026 GMT
  host: www.argyle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:21:38 2026 GMT
  host: docs.argyle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 15:40:12 2026 GMT
  host: api.argyle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argyle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argyle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Argyle
provider_slug: argyle
slug: argyle-domain-security
source_filename: argyle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.argyle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:43:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.argyle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:21:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.argyle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:40:12 2026 GMT\n  hsts: null\ndomains:\n- domain: argyle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argyle/refs/heads/main/security/argyle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Employment Data
- Payroll
- Income Verification
- Gig Economy
- Financial Data
- Employment History
- Earned Wage Access
- Direct Deposit
---
