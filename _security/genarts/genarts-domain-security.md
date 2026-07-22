---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: genarts.com
  spf: true
hosts:
- cert_expires: Sep 23 11:41:56 2026 GMT
  host: www.genarts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Genarts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenArts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GenArts
provider_slug: genarts
slug: genarts-domain-security
source_filename: genarts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genarts.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 11:41:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genarts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genarts/refs/heads/main/security/genarts-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Visual Effects
- VFX
- Video Editing
- Plugins
- Media and Entertainment
- Software
- Acquired
---
