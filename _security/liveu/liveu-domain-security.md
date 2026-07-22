---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liveu.tv
  spf: true
hosts:
- cert_expires: Sep  7 11:51:53 2026 GMT
  host: www.liveu.tv
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liveu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liveu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liveu
provider_slug: liveu
slug: liveu-domain-security
source_filename: liveu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liveu.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:51:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liveu.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveu/refs/heads/main/security/liveu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Live Video
- Video Streaming
- Broadcast
- Bonded Cellular
- Video Contribution
- Media & Entertainment
- Sports Production
- Public Safety
- 5G
---
