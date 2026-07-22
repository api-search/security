---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: bunkerhillhealth.com
  spf: false
hosts:
- cert_expires: Sep 30 14:44:42 2026 GMT
  host: bunkerhillhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bunkerhillhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bunkerhill Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present.'
provider_name: Bunkerhill Health
provider_slug: bunkerhillhealth
slug: bunkerhillhealth-domain-security
source_filename: bunkerhillhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bunkerhillhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:44:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bunkerhillhealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunkerhillhealth/refs/heads/main/security/bunkerhillhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- AI Agents
- Health Systems
- Clinical
- Medical Imaging
---
