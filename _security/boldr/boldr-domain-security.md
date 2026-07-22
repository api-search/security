---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopboldr.com
  spf: false
hosts:
- cert_expires: Sep  9 20:44:04 2026 GMT
  host: shopboldr.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boldr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boldr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Boldr
provider_slug: boldr
slug: boldr-domain-security
source_filename: boldr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shopboldr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 20:44:04 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: shopboldr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boldr/refs/heads/main/security/boldr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Home
- Energy
- Climate Control
- IoT
- Consumer Hardware
- Thermostat
- HVAC
- Ecommerce
---
