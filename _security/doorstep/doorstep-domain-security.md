---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doorstep.ai
  spf: true
hosts:
- cert_expires: Oct  4 08:21:58 2026 GMT
  host: www.doorstep.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doorstep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doorstep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Doorstep
provider_slug: doorstep
slug: doorstep-domain-security
source_filename: doorstep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doorstep.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:21:58 2026 GMT\n  hsts: false\ndomains:\n- domain: doorstep.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doorstep/refs/heads/main/security/doorstep-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Delivery
- Last-Mile Logistics
- Indoor Positioning
- Location Tracking
- Mobile SDK
- Delivery Tracking
- Fraud Prevention
- Proof of Delivery
---
