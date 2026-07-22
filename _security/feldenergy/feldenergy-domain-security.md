---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: feld.energy
  spf: true
hosts:
- cert_expires: Sep 26 15:24:49 2026 GMT
  host: www.feld.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Feldenergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for feld.energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: feld.energy
provider_slug: feldenergy
slug: feldenergy-domain-security
source_filename: feldenergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.feld.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:24:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: feld.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feldenergy/refs/heads/main/security/feldenergy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Climate Energy
- Agri-PV
- Agrivoltaics
- Solar Energy
- Renewable Energy
- Agriculture
- Photovoltaics
- Germany
---
