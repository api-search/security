---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: goshipyard.app
  spf: false
hosts:
- cert_expires: Jan 28 21:18:40 2027 GMT
  host: goshipyard.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shipyard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shipyard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Shipyard
provider_slug: goshipyard-app
slug: goshipyard-app-domain-security
source_filename: goshipyard-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goshipyard.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 21:18:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goshipyard.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/goshipyard-app/security/goshipyard-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Directory
- Marketplace
- Community
- Growth
---
