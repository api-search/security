---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adastec.com
  spf: true
hosts:
- cert_expires: Dec  1 06:15:41 2026 GMT
  host: www.adastec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adastec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adastec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Adastec
provider_slug: adastec
slug: adastec-domain-security
source_filename: adastec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adastec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 06:15:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adastec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adastec/refs/heads/main/security/adastec-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Autonomous Vehicles
- Automated Driving
- Public Transit
- Transportation
- Mobility
- Fleet Management
- Automotive
- Robotics
---
