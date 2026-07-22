---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: craterstudios.ai
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: craterstudiosgames.com
  spf: true
hosts:
- cert_expires: Oct  7 11:03:13 2026 GMT
  host: craterstudios.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 17:40:13 2026 GMT
  host: www.craterstudiosgames.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crater Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crater Studios, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Crater Studios
provider_slug: crater-studios
slug: crater-studios-domain-security
source_filename: crater-studios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craterstudios.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:03:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.craterstudiosgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:40:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: craterstudios.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: craterstudiosgames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crater-studios/refs/heads/main/security/crater-studios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Games
- Game Development
- Artificial Intelligence
- AI Agents
- Live Operations
- Venture Backed
---
