---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: camion.energy
  spf: true
hosts:
- cert_expires: Sep 17 08:45:48 2026 GMT
  host: www.camion.energy
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Camion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Camion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Camion
provider_slug: camion
slug: camion-domain-security
source_filename: camion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.camion.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:45:48 2026 GMT\n  hsts: false\ndomains:\n- domain: camion.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camion/refs/heads/main/security/camion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy And Environmental
- Electrification
- Real Estate
- EV Charging
- Cleantech
- Infrastructure Intelligence
- Energy Transition
---
