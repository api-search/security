---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: equipboard.com
  spf: true
hosts:
- cert_expires: Sep  3 06:58:21 2026 GMT
  host: equipboard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Equipboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equipboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Equipboard
provider_slug: equipboard
slug: equipboard-domain-security
source_filename: equipboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equipboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 06:58:21 2026 GMT\n  hsts: null\ndomains:\n- domain: equipboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equipboard/refs/heads/main/security/equipboard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Musical Instruments
- Music Gear
- Community
- Discovery
- Reviews
- Consumer
- Entertainment
- Affiliate
---
