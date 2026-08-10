---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: galactic-energy.cn
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.galactic-energy.cn
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Galactic Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galactic Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Galactic Energy
provider_slug: galactic-energy
slug: galactic-energy-domain-security
source_filename: galactic-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.galactic-energy.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: galactic-energy.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galactic-energy/refs/heads/main/security/galactic-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Space
- Spaceflight
- Launch Services
- Small Satellite Launch
- Rocket Engines
- Reusable Launch Vehicles
- Manufacturing
- China
---
