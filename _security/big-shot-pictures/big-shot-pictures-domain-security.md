---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bigshotpictures.com
  spf: true
hosts:
- cert_expires: Oct 29 20:13:46 2026 GMT
  host: bigshotpictures.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Big Shot Pictures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Big Shot Pictures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Big Shot Pictures
provider_slug: big-shot-pictures
slug: big-shot-pictures-domain-security
source_filename: big-shot-pictures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigshotpictures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 20:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bigshotpictures.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-shot-pictures/refs/heads/main/security/big-shot-pictures-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Entertainment
- Film
- Media
- Studio
---
