---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hw.energy
  spf: true
hosts:
- cert_expires: Sep 14 07:14:35 2026 GMT
  host: hw.energy
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hydro Wind Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydro Wind Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hydro Wind Energy
provider_slug: hydro-wind-energy
slug: hydro-wind-energy-domain-security
source_filename: hydro-wind-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hw.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:14:35 2026 GMT\n  hsts: false\ndomains:\n- domain: hw.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-wind-energy/refs/heads/main/security/hydro-wind-energy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Renewable Energy
- Offshore Wind
- Energy Storage
- Desalination
- Clean Technology
- Climate Tech
- Hardware
---
