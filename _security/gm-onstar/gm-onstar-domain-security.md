---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onstar.com
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: www.onstar.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gm Onstar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GM OnStar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GM OnStar
provider_slug: gm-onstar
slug: gm-onstar-domain-security
source_filename: gm-onstar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: onstar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gm-onstar/refs/heads/main/security/gm-onstar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Connected Vehicle
- Telematics
- Fleet Management
- Vehicle Data
- Vehicle Location
- Vehicle Diagnostics
- Driver Behavior
- Electric Vehicle
- EV Charging
- OnStar
- General Motors
- Embedded Connectivity
- OEM Telematics
---
