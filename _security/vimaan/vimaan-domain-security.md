---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vimaan.ai
  spf: true
hosts:
- cert_expires: Aug 27 12:13:29 2026 GMT
  host: vimaan.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vimaan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vimaan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vimaan
provider_slug: vimaan
slug: vimaan-domain-security
source_filename: vimaan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vimaan.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:13:29 2026 GMT\n  hsts: false\ndomains:\n- domain: vimaan.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vimaan/refs/heads/main/security/vimaan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Autonomous Apps
- Computer Vision
- Machine Learning
- Inventory
- Warehouse
- Supply Chain
- Robotics
- Drones
---
