---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: homebridgepc.com
  spf: true
hosts:
- cert_expires: Jan 22 21:43:32 2027 GMT
  host: homebridgepc.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GFRC Precast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GFRC Precast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GFRC Precast
provider_slug: homebridgepc-com
slug: homebridgepc-com-domain-security
source_filename: homebridgepc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homebridgepc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 21:43:32 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: homebridgepc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/homebridgepc-com/security/homebridgepc-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fire Pits
- Garden Beds
- Culvert Covers
- Retaining Walls
- GFRC Concrete
- Outdoor Products
- Wholesale
---
