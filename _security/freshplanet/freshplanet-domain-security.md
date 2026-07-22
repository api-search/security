---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: freshplanet.com
  spf: true
hosts:
- cert_expires: Sep 19 07:40:12 2026 GMT
  host: freshplanet.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshplanet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreshPlanet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: FreshPlanet
provider_slug: freshplanet
slug: freshplanet-domain-security
source_filename: freshplanet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freshplanet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:40:12 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: freshplanet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshplanet/refs/heads/main/security/freshplanet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Mobile Games
- Gaming
- Entertainment
- Music
- Consumer Apps
- New York
---
