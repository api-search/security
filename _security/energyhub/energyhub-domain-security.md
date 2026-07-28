---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: energyhub.com
  spf: true
hosts:
- cert_expires: Sep 28 09:28:55 2026 GMT
  host: www.energyhub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: mec.energyhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Energyhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnergyHub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EnergyHub
provider_slug: energyhub
slug: energyhub-domain-security
source_filename: energyhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energyhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 09:28:55 2026 GMT\n  hsts: false\n- host: mec.energyhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: energyhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energyhub/refs/heads/main/security/energyhub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Grid
- DERMS
- Distributed Energy Resources
- Demand Response
- Virtual Power Plant
- OpenADR
- EV Charging
- Solar
- Energy Storage
- Smart Thermostats
---
