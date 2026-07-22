---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zipline.com
  spf: true
hosts:
- cert_expires: Sep  9 20:02:01 2026 GMT
  host: www.zipline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zipline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zipline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zipline
provider_slug: zipline
slug: zipline-domain-security
source_filename: zipline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zipline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 20:02:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zipline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zipline/refs/heads/main/security/zipline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drones
- Autonomous Aircraft
- Drone Delivery
- Unmanned Aerial Systems
- Autonomous Logistics
- Last Mile Delivery
- Quick Commerce
- Healthcare Logistics
- Medical Delivery
- Blood Delivery
- Vaccine Delivery
- Retail Delivery
- Restaurant Delivery
- Aviation
- BVLOS
- Detect And Avoid
- VTOL
- Robotics
- Hardware
---
