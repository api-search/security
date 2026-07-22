---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crewline.ai
  spf: true
hosts:
- cert_expires: Oct  4 03:38:09 2026 GMT
  host: crewline.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crewline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crewline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crewline
provider_slug: crewline
slug: crewline-domain-security
source_filename: crewline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crewline.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:38:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crewline.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crewline/refs/heads/main/security/crewline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Autonomous Equipment
- Construction Technology
- Heavy Machinery
- Robotics
- Self-Driving
- Retrofit
---
