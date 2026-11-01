---
api_specs:
- filename: pops4-com-well-known-openapi.json
  format: json
  label: Edgar & Edgarette SEC Filing Boards .well-known API
  slug: edgar-edgarette-sec-filing-boards-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pops4-com/openapi/_original/pops4-com-well-known-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pops4.com
  spf: true
hosts:
- cert_expires: Dec 10 17:59:57 2026 GMT
  host: pops4.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pops4 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pops4-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: pops4-com
provider_slug: pops4-com
slug: pops4-com-domain-security
source_filename: pops4-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pops4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 17:59:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: pops4.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pops4-com/security/pops4-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wholesale
- Corporate Gifts
- Branding
- B2B
---
