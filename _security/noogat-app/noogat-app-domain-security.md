---
api_specs:
- filename: noogat-app-openapi-generated.yml
  format: yaml
  label: Noogat API
  slug: noogat-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noogat-app/openapi/_ae-authored/noogat-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: noogat.app
  spf: false
hosts:
- cert_expires: Feb  6 14:05:18 2027 GMT
  host: noogat.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Noogat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noogat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Noogat
provider_slug: noogat-app
slug: noogat-app-domain-security
source_filename: noogat-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noogat.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 14:05:18 2027 GMT\n  hsts: false\ndomains:\n- domain: noogat.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/noogat-app/security/noogat-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Voice Notes
- Artificial Intelligence
- Productivity
- iOS
- Privacy
---
