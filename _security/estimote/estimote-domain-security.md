---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: estimote.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: estimote.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Estimote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estimote, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Estimote
provider_slug: estimote
slug: estimote-domain-security
source_filename: estimote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estimote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: estimote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estimote/refs/heads/main/security/estimote-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Location
- Proximity
- Beacons
- Bluetooth
- IoT
- Indoor Location
- UWB
- Asset Tracking
- Developer Tools
---
