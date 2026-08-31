---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: starship.xyz
  spf: true
hosts:
- cert_expires: Oct 18 05:50:26 2026 GMT
  host: www.starship.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starship Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Starship Technologies
provider_slug: starship
slug: starship-domain-security
source_filename: starship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starship.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 05:50:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: starship.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starship/refs/heads/main/security/starship-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Autonomous Vehicles
- Last Mile Delivery
- Logistics
- Food Delivery
- Grocery
- Delivery as a Service
---
