---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jamcity.com
  spf: true
hosts:
- cert_expires: Dec  6 14:35:59 2026 GMT
  host: www.jamcity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jam City Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jam City, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jam City
provider_slug: jam-city
slug: jam-city-domain-security
source_filename: jam-city-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jamcity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 14:35:59 2026 GMT\n  hsts: false\ndomains:\n- domain: jamcity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jam-city/refs/heads/main/security/jam-city-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Games
- Mobile Games
- Gaming
- Entertainment
- Mobile Apps
- Free To Play
- Consumer
---
