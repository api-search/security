---
api_specs:
- filename: by-mason-openapi-generated.yml
  format: yaml
  label: By Mason API
  slug: by-mason-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/by-mason/openapi/_ae-authored/by-mason-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bymason.com
  spf: false
hosts:
- cert_expires: Dec 13 08:28:15 2026 GMT
  host: www.bymason.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: By Mason Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for By Mason, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: By Mason
provider_slug: by-mason
slug: by-mason-domain-security
source_filename: by-mason-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bymason.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 08:28:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bymason.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/by-mason/security/by-mason-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Device Management
- Enterprise Hardware
- Fleet Management
- Rugged Devices
- Healthcare
- Logistics
- Retail
---
