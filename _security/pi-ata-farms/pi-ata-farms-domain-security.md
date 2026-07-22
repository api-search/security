---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pinatafarm.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: www.pinatafarm.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pi Ata Farms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Piñata Farms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Piñata Farms
provider_slug: pi-ata-farms
slug: pi-ata-farms-domain-security
source_filename: pi-ata-farms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinatafarm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pinatafarm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pi-ata-farms/refs/heads/main/security/pi-ata-farms-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Entertainment
- AI Video
- Memes
- Consumer App
- Mobile
- Video Generation
---
