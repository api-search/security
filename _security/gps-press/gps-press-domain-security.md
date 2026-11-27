---
api_specs:
- filename: gps-press-openapi.json
  format: json
  label: Public Data API
  slug: public-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gps-press/openapi/gps-press-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gps.press
  spf: true
hosts:
- cert_expires: Jan 22 15:23:55 2027 GMT
  host: gps.press
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Georgia Prisoners' Speak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Georgia Prisoners'' Speak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Georgia Prisoners' Speak
provider_slug: gps-press
slug: gps-press-domain-security
source_filename: gps-press-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gps.press\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 15:23:55 2027 GMT\n  hsts: false\ndomains:\n- domain: gps.press\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gps-press/security/gps-press-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Non-Profit
- Research
- Georgia
- Prison
- Accountability
---
