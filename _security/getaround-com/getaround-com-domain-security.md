---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getaround.com
  spf: true
hosts:
- cert_expires: Sep 26 19:08:20 2026 GMT
  host: getaround.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getaround Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getaround, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Getaround
provider_slug: getaround-com
slug: getaround-com-domain-security
source_filename: getaround-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getaround.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:08:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getaround.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaround-com/refs/heads/main/security/getaround-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Car Sharing
- Peer To Peer
- Mobility
- Connected Car
- Telematics
- Marketplace
- Transportation
- Fleet
- Carsharing Europe
- Keyless Entry
- Vehicle Rental
- Getaround Connect
---
