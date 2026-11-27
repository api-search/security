---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fabricate.build
  spf: true
hosts:
- cert_expires: Jan  4 01:45:19 2027 GMT
  host: fabricate.build
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fabricate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fabricate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Fabricate
provider_slug: fabricate-build
slug: fabricate-build-domain-security
source_filename: fabricate-build-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabricate.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 01:45:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fabricate.build\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fabricate-build/security/fabricate-build-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- No-Code
- App Builder
- Cloudflare
- Web Development
---
