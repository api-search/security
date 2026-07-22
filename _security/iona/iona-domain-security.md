---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ionadrones.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: ionadrones.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IONA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IONA
provider_slug: iona
slug: iona-domain-security
source_filename: iona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ionadrones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ionadrones.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iona/refs/heads/main/security/iona-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Drones
- Logistics
- Delivery
- Autonomous Vehicles
- Aviation
- Robotics
- Healthcare Logistics
---
