---
api_specs:
- filename: trucker-tools-openapi-generated.yml
  format: yaml
  label: Trucker Tools API
  slug: trucker-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trucker-tools/openapi/_ae-authored/trucker-tools-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: truckertools.com
  spf: true
hosts:
- cert_expires: Dec 23 16:28:38 2026 GMT
  host: truckertools.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trucker Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trucker Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trucker Tools
provider_slug: trucker-tools
slug: trucker-tools-domain-security
source_filename: trucker-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truckertools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 16:28:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: truckertools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/trucker-tools/security/trucker-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Freight
- Load Tracking
- Carrier Tools
---
