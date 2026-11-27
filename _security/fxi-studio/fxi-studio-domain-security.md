---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fxi.studio
  spf: true
hosts:
- cert_expires: Dec 25 13:53:40 2026 GMT
  host: fxi.studio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FXI Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FXI Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FXI Studio
provider_slug: fxi-studio
slug: fxi-studio-domain-security
source_filename: fxi-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fxi.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 13:53:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fxi.studio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fxi-studio/security/fxi-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Filmmaking
- Platform
- Creative
- Video
---
