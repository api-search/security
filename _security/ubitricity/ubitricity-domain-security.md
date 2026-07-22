---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: ubitricity.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: ubitricity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubitricity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubitricity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Ubitricity
provider_slug: ubitricity
slug: ubitricity-domain-security
source_filename: ubitricity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ubitricity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ubitricity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubitricity/refs/heads/main/security/ubitricity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- EV Charging
- Electric Vehicles
- Charging Infrastructure
- Lamppost Charging
- Smart Charging
- Mobility
- OCPP
---
