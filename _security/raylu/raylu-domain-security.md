---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: raylu.dev
  spf: true
hosts:
- cert_expires: Dec 14 08:35:13 2026 GMT
  host: www.raylu.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Raylu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raylu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Raylu
provider_slug: raylu
slug: raylu-domain-security
source_filename: raylu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.raylu.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 08:35:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: raylu.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://artifacts.apis.io/raylu/security/raylu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- PrivateMarkets
- Investment
- Origination
---
