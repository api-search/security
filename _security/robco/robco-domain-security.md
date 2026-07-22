---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rob.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: robco.studio
  spf: false
hosts:
- cert_expires: Sep 25 13:55:51 2026 GMT
  host: www.rob.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: robco.studio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robco, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Robco
provider_slug: robco
slug: robco-domain-security
source_filename: robco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rob.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:55:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: robco.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rob.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: robco.studio\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robco/refs/heads/main/security/robco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Industrial Automation
- Robotics-as-a-Service
- Manufacturing
- No-Code
- Computer Vision
- Physical AI
- Automation
---
