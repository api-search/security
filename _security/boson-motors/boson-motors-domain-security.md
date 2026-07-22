---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bosonmotors.com
  spf: true
hosts:
- cert_expires: Aug 19 03:07:56 2026 GMT
  host: bosonmotors.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boson Motors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boson Motors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Boson Motors
provider_slug: boson-motors
slug: boson-motors-domain-security
source_filename: boson-motors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bosonmotors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 03:07:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bosonmotors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boson-motors/refs/heads/main/security/boson-motors-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Electric Vehicles
- Robotics
- Automotive
- Agriculture
- Automation
- Manufacturing
- Off-Road
---
