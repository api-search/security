---
api_specs:
- filename: sysco-food-distribution-api-openapi.yml
  format: yaml
  label: Sysco Food Distribution API
  slug: food-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysco/refs/heads/main/openapi/sysco-food-distribution-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sysco.com
  spf: true
hosts:
- cert_expires: Jul 23 12:46:57 2026 GMT
  host: www.sysco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 12:13:04 2026 GMT
  host: apic-devportal.sysco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.sysco.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sysco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sysco, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sysco
provider_slug: sysco
slug: sysco-domain-security
source_filename: sysco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sysco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 23 12:46:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apic-devportal.sysco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 12:13:04 2026 GMT\n  hsts: false\n- host: api.sysco.com\n  https: false\ndomains:\n- domain: sysco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysco/refs/heads/main/security/sysco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- Food Distribution
- Food Service
- Supply Chain
- Fortune 100
- Wholesale
---
