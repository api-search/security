---
api_specs:
- filename: otakit-app-openapi-generated.yml
  format: yaml
  label: OtaKit API
  slug: otakit-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/otakit-app/openapi/_ae-authored/otakit-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: otakit.app
  spf: false
hosts:
- cert_expires: Jan 17 23:29:50 2027 GMT
  host: otakit.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OtaKit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OtaKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: OtaKit
provider_slug: otakit-app
slug: otakit-app-domain-security
source_filename: otakit-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otakit.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:29:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: otakit.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/otakit-app/security/otakit-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- OTA Updates
- Capacitor
- Over‑the‑air
- App updates
---
