---
api_specs:
- filename: prestmit-openapi.yml
  format: yaml
  label: Prestmit Partner API
  slug: prestmit-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prestmit.io
  spf: true
hosts:
- cert_expires: Aug 23 05:58:20 2026 GMT
  host: prestmit.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 13:46:15 2026 GMT
  host: api.prestmit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 06:14:01 2026 GMT
  host: dev-api.prestmit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prestmit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prestmit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prestmit
provider_slug: prestmit
slug: prestmit-domain-security
source_filename: prestmit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prestmit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 05:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prestmit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 13:46:15 2026 GMT\n  hsts: false\n- host: dev-api.prestmit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:14:01 2026 GMT\n  hsts: false\ndomains:\n- domain: prestmit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/security/prestmit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bills
- Crypto
- Fintech
- Gift Cards
- Payments
---
