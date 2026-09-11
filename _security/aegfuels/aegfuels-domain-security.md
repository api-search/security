---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aegfuels.com
  spf: false
hosts:
- cert_expires: Nov 13 10:04:25 2026 GMT
  host: www.aegfuels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aegfuels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AEG Fuels, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AEG Fuels
provider_slug: aegfuels
slug: aegfuels-domain-security
source_filename: aegfuels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aegfuels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 10:04:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aegfuels.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aegfuels/refs/heads/main/security/aegfuels-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Aviation
- Aviation Fuel
- Fuel
- Energy
- Logistics
- Supply Chain
- Flight Support
- Sustainable Aviation Fuel
- Marine Fuel
- Transportation
- Business Aviation
---
