---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flick.art
  spf: true
hosts:
- cert_expires: Aug 31 07:31:45 2026 GMT
  host: flick.art
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flick
provider_slug: flick
slug: flick-domain-security
source_filename: flick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flick.art\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:31:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flick.art\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flick/refs/heads/main/security/flick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video
- Filmmaking
- Media and Entertainment
- Creative Tools
- Content Creation
---
