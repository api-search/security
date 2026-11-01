---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: windowai.io
  spf: false
hosts:
- cert_expires: Jan 14 04:43:04 2027 GMT
  host: windowai.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Windowai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Window.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Window.ai
provider_slug: windowai
slug: windowai-domain-security
source_filename: windowai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: windowai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 04:43:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: windowai.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/windowai/security/windowai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Browser Extension
- Privacy
- UserControl
---
