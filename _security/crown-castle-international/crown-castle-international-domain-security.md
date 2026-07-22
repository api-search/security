---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crowncastle.com
  spf: true
hosts:
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: www.crowncastle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crown Castle International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crown Castle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crown Castle
provider_slug: crown-castle-international
slug: crown-castle-international-domain-security
source_filename: crown-castle-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crowncastle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: crowncastle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crown-castle-international/refs/heads/main/security/crown-castle-international-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- 5G
- Cell Towers
- Cloud Connect
- Communications Infrastructure
- Dark Fiber
- DDoS Defense
- Ethernet
- Fiber
- Managed Networks
- Private Networks
- SD-WAN
- Small Cells
- Telecommunications
- Wireless
- Fortune 1000
---
