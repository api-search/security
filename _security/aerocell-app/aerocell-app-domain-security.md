---
api_specs:
- filename: aerocell-app-api-openapi.json
  format: json
  label: 'AeroCell: Affordable eSIMs — Read-only API API'
  slug: aerocell-affordable-esims-read-only-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aerocell-app/openapi/_original/aerocell-app-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aerocell.app
  spf: true
hosts:
- cert_expires: Dec 11 22:17:21 2026 GMT
  host: aerocell.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AeroCell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AeroCell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AeroCell
provider_slug: aerocell-app
slug: aerocell-app-domain-security
source_filename: aerocell-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aerocell.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 22:17:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aerocell.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aerocell-app/security/aerocell-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- eSIM
- Mobile Data
- International
- Connectivity
- Telecommunications
---
