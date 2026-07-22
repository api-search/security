---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sense.com
  spf: true
hosts:
- cert_expires: Oct  3 17:45:52 2026 GMT
  host: sense.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sense Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sense, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sense
provider_slug: sense-energy
slug: sense-energy-domain-security
source_filename: sense-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:45:52 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: sense.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sense-energy/refs/heads/main/security/sense-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Home Energy
- Energy Monitoring
- Electricity
- Smart Meters
- AMI
- Grid Edge
- Utilities
- Demand Response
- Virtual Power Plant
- Disaggregation
- Machine Learning
- Smart Home
- IoT
- Solar
- Sustainability
---
