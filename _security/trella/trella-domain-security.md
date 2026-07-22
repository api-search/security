---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trella.app
  spf: false
hosts:
- cert_expires: Sep 13 08:58:26 2026 GMT
  host: www.trella.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trella Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trella, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trella
provider_slug: trella
slug: trella-domain-security
source_filename: trella-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trella.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:58:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trella.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trella/refs/heads/main/security/trella-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Trucking
- Freight
- Logistics
- Digital Freight Marketplace
- B2B Marketplace
- Shippers
- Carriers
- Supply Chain
- GPS Tracking
- Electronic Proof Of Delivery
- MENA
- Egypt
- Saudi Arabia
- United Arab Emirates
- Pakistan
---
