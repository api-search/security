---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hevenaerotech.com
  spf: true
hosts:
- cert_expires: Dec  3 15:18:25 2026 GMT
  host: hevenaerotech.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Heven Aerotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heven AeroTech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Heven AeroTech
provider_slug: heven-aerotech
slug: heven-aerotech-domain-security
source_filename: heven-aerotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hevenaerotech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 15:18:25 2026 GMT\n  hsts: false\ndomains:\n- domain: hevenaerotech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heven-aerotech/refs/heads/main/security/heven-aerotech-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Drones
- Unmanned Aerial Systems
- Aerospace
- Defense
- National Security
- Public Safety
- Hydrogen
- Manufacturing
- Hardware
---
