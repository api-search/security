---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: breathebatteries.com
  spf: true
hosts:
- cert_expires: Oct 14 14:31:55 2026 GMT
  host: www.breathebatteries.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: docs.breathebatteries.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Breathe Battery Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breathe Battery Technologies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Breathe Battery Technologies
provider_slug: breathe-battery-technologies
slug: breathe-battery-technologies-domain-security
source_filename: breathe-battery-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breathebatteries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 14:31:55 2026 GMT\n  hsts: false\n- host: docs.breathebatteries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: breathebatteries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breathe-battery-technologies/refs/heads/main/security/breathe-battery-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Battery
- Battery Simulation
- Electric Vehicles
- Energy Storage
- Cell Design
- Physics-Based Modeling
- Automotive
- Deep Tech
- Developer Tools
---
