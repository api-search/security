---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: twisty.ai
  spf: false
hosts:
- cert_expires: Sep  6 23:21:20 2026 GMT
  host: twisty.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twisty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twisty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Twisty
provider_slug: twisty
slug: twisty-domain-security
source_filename: twisty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: twisty.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:21:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: twisty.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twisty/refs/heads/main/security/twisty-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Video
- Content Creation
- AI Characters
- Media
- Consumer
---
