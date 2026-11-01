---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zovo.one
  spf: true
hosts:
- cert_expires: Jan 24 01:41:08 2027 GMT
  host: zovo.one
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zovo One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zovo-one, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: zovo-one
provider_slug: zovo-one
slug: zovo-one-domain-security
source_filename: zovo-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zovo.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 01:41:08 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: zovo.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zovo-one/security/zovo-one-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Chrome Extensions
- Productivity
- Privacy
- Free Tools
- Developer
---
