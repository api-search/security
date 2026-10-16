---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: syngenta.com
  spf: true
hosts:
- cert_expires: Jan  6 19:12:27 2027 GMT
  host: www.syngenta.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Syngenta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syngenta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Syngenta
provider_slug: syngenta
slug: syngenta-domain-security
source_filename: syngenta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syngenta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 19:12:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: syngenta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syngenta/refs/heads/main/security/syngenta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Seeds
- Crop Protection
- Digital Farming
---
