---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mobilityhouse.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tmh.energy
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.mobilityhouse.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 15:00:19 2026 GMT
  host: vdv-docs.tmh.energy
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 18:39:54 2026 GMT
  host: tmh-help.freshdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Mobility House Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Mobility House, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Mobility House
provider_slug: the-mobility-house
slug: the-mobility-house-domain-security
source_filename: the-mobility-house-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mobilityhouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: vdv-docs.tmh.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 15:00:19 2026 GMT\n  hsts: false\n- host: tmh-help.freshdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 18:39:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mobilityhouse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tmh.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-mobility-house/refs/heads/main/security/the-mobility-house-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Energy Management
- Vehicle-to-Grid
- Load Management
- Fleet
- OCPP
- VDV 463
- Modbus
- Germany
---
