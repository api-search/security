---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: atherenergy.com
  spf: true
hosts:
- cert_expires: Nov 15 09:48:50 2026 GMT
  host: www.atherenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ather Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ather Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ather Energy
provider_slug: ather-energy
slug: ather-energy-domain-security
source_filename: ather-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atherenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 09:48:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atherenergy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ather-energy/refs/heads/main/security/ather-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Electric Vehicles
- Automotive
- Transportation
- Manufacturing
- Energy
- EV Charging
- Mobility
- Internet of Things
- India
---
