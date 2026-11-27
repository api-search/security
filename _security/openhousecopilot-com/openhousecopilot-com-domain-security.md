---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openhousecopilot.com
  spf: true
hosts:
- cert_expires: Feb  8 03:53:43 2027 GMT
  host: openhousecopilot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open House Copilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open House Copilot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open House Copilot
provider_slug: openhousecopilot-com
slug: openhousecopilot-com-domain-security
source_filename: openhousecopilot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openhousecopilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 03:53:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openhousecopilot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openhousecopilot-com/security/openhousecopilot-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Artificial Intelligence
- Lead Management
- OpenHouse
- Software-as-a-Service
---
