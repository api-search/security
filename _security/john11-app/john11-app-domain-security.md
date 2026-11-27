---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: john11.app
  spf: false
hosts:
- cert_expires: Dec 24 10:53:49 2026 GMT
  host: john11.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: John 11 App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for John 11 App, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: John 11 App
provider_slug: john11-app
slug: john11-app-domain-security
source_filename: john11-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: john11.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 10:53:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: john11.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/john11-app/security/john11-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Bible
- iOS
- Reading
- Offline
---
