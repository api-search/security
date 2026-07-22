---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orbitfab.com
  spf: true
hosts:
- cert_expires: Sep 27 12:20:18 2026 GMT
  host: orbitfab.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbit Fab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbit Fab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orbit Fab
provider_slug: orbit-fab
slug: orbit-fab-domain-security
source_filename: orbit-fab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbitfab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:20:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orbitfab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbit-fab/refs/heads/main/security/orbit-fab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Space
- Aerospace
- Satellite
- Refueling
- Space Logistics
- In-Space Servicing
- Propellant
- Hardware
---
