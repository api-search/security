---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: calibratevc.com
  spf: true
hosts:
- cert_expires: Sep 12 03:33:08 2026 GMT
  host: www.calibratevc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calibrate Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calibrate Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Calibrate Ventures
provider_slug: calibrate-ventures
slug: calibrate-ventures-domain-security
source_filename: calibrate-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.calibratevc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:33:08 2026 GMT\n  hsts: false\ndomains:\n- domain: calibratevc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calibrate-ventures/refs/heads/main/security/calibrate-ventures-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Venture Capital
- Deep Tech
- Artificial Intelligence
- Robotics
- Automation
- Machine Learning
- Computer Vision
---
