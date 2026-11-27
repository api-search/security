---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mentor.energy
  spf: true
hosts:
- cert_expires: Jan 14 09:06:20 2027 GMT
  host: mentor.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mentor.energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mentor.energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: mentor.energy
provider_slug: mentor-energy
slug: mentor-energy-domain-security
source_filename: mentor-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mentor.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 09:06:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mentor.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mentor-energy/security/mentor-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Mentorship
- Careers
- Learning
- Platform
---
