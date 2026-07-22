---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: innostic.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.innostic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Innostic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for innostic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: innostic
provider_slug: innostic
slug: innostic-domain-security
source_filename: innostic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.innostic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: innostic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innostic/refs/heads/main/security/innostic-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Healthcare
- Medical Devices
- Supply Chain
- Distribution
- In Vitro Diagnostics
- Hospital
- China
---
