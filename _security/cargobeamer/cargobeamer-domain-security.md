---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cargobeamer.com
  spf: true
hosts:
- cert_expires: Dec  9 08:04:08 2026 GMT
  host: www.cargobeamer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cargobeamer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cargobeamer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cargobeamer
provider_slug: cargobeamer
slug: cargobeamer-domain-security
source_filename: cargobeamer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cargobeamer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 08:04:08 2026 GMT\n  hsts: false\ndomains:\n- domain: cargobeamer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargobeamer/refs/heads/main/security/cargobeamer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Intermodal
- Rail
- Sustainability
---
