---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: droneintelligence.ai
  spf: true
hosts:
- cert_expires: Jan 14 14:15:26 2027 GMT
  host: droneintelligence.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Droneintelligence Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drone Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Drone Intelligence
provider_slug: droneintelligence-ai
slug: droneintelligence-ai-domain-security
source_filename: droneintelligence-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: droneintelligence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 14:15:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: droneintelligence.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/droneintelligence-ai/security/droneintelligence-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Drone
- Intelligence
- Research
- Markets
- Analytics
---
