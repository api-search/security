---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: canopy-ad.com
  spf: true
hosts:
- cert_expires: Sep 23 08:50:11 2026 GMT
  host: www.canopy-ad.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canopy Aerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canopy Aerospace & Defense, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Canopy Aerospace & Defense
provider_slug: canopy-aerospace
slug: canopy-aerospace-domain-security
source_filename: canopy-aerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.canopy-ad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 08:50:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: canopy-ad.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canopy-aerospace/refs/heads/main/security/canopy-aerospace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Aerospace
- Defense
- Space
- Advanced Materials
- Thermal Protection Systems
- Hypersonics
- Additive Manufacturing
- Ceramics
---
