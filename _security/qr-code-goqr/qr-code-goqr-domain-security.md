---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: goqr.me
  spf: false
hosts:
- cert_expires: Aug 19 21:28:06 2026 GMT
  host: goqr.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Qr Code Goqr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QR code, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: QR code
provider_slug: qr-code-goqr
slug: qr-code-goqr-domain-security
source_filename: qr-code-goqr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goqr.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 19 21:28:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goqr.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qr-code-goqr/refs/heads/main/security/qr-code-goqr-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Development
- Public APIs
---
