---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: inuru.com
  spf: true
hosts:
- cert_expires: Oct  2 21:57:16 2026 GMT
  host: www.inuru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inuru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INURU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: INURU
provider_slug: inuru
slug: inuru-domain-security
source_filename: inuru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inuru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:57:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inuru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inuru/refs/heads/main/security/inuru-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Printed Electronics
- OLED
- Smart Packaging
- Hardware
- Internet of Things
- Sustainability
- Manufacturing
- Medical
- Germany
---
