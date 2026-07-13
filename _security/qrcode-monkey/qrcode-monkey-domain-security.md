---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qrcode-monkey.com
  spf: false
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: www.qrcode-monkey.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qrcode Monkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qrcode Monkey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Qrcode Monkey
provider_slug: qrcode-monkey
slug: qrcode-monkey-domain-security
source_filename: qrcode-monkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qrcode-monkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: qrcode-monkey.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qrcode-monkey/refs/heads/main/security/qrcode-monkey-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---
