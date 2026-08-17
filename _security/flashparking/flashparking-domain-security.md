---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flashparking.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flashos.com
  spf: true
hosts:
- cert_expires: Nov  5 23:11:43 2026 GMT
  host: www.flashparking.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 18:55:16 2026 GMT
  host: help.flashos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flashparking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flashparking, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flashparking
provider_slug: flashparking
slug: flashparking-domain-security
source_filename: flashparking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flashparking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:11:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.flashos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 18:55:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flashparking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: flashos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flashparking/refs/heads/main/security/flashparking-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Parking
- Mobility
- Transportation
- Payments
- Internet of Things
- Computer Vision
- Real Estate
- Electric Vehicle Charging
- Reservations
---
