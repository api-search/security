---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: focal.systems
  spf: true
hosts:
- cert_expires: Sep 22 14:01:43 2026 GMT
  host: focal.systems
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Focal Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Focal Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Focal Systems
provider_slug: focal-systems
slug: focal-systems-domain-security
source_filename: focal-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: focal.systems\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:01:43 2026 GMT\n  hsts: false\ndomains:\n- domain: focal.systems\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/focal-systems/refs/heads/main/security/focal-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Computer Vision
- Artificial Intelligence
- Deep Learning
- Retail Automation
- Inventory Management
- On-Shelf Availability
- Grocery
---
