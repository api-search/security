---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: irisonboard.com
  spf: true
hosts:
- cert_expires: Oct  6 23:05:49 2026 GMT
  host: www.irisonboard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iris Automation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iris Automation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Iris Automation
provider_slug: iris-automation
slug: iris-automation-domain-security
source_filename: iris-automation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.irisonboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:05:49 2026 GMT\n  hsts: null\ndomains:\n- domain: irisonboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iris-automation/refs/heads/main/security/iris-automation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deep Tech
- Drones
- UAS
- Detect and Avoid
- Collision Avoidance
- Computer Vision
- Aviation
- BVLOS
---
