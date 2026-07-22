---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bolt.earth
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: bolt.earth
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boltearth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolt.Earth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bolt.Earth
provider_slug: boltearth
slug: boltearth-domain-security
source_filename: boltearth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bolt.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bolt.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltearth/refs/heads/main/security/boltearth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Electric Vehicles
- EV Charging
- Charging Infrastructure
- Clean Energy
- Mobility
- India
---
