---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: braincorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brainos.com
  spf: false
hosts:
- cert_expires: Sep 26 18:05:46 2026 GMT
  host: www.braincorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 17:01:17 2026 GMT
  host: brainos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brain Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brain Corp, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brain Corp
provider_slug: brain-corp
slug: brain-corp-domain-security
source_filename: brain-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.braincorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:05:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: brainos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:01:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: braincorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: brainos.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brain-corp/refs/heads/main/security/brain-corp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Autonomous Mobile Robots
- Autonomy
- BrainOS
- Cleaning Robots
- Floor Care
- Inventory Management
- RFID
- Retail Robotics
- Robotics
- Scanning as a Service
---
