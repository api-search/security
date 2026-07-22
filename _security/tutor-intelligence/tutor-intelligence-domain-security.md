---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tutorintelligence.com
  spf: true
hosts:
- cert_expires: Oct  9 23:58:29 2026 GMT
  host: tutorintelligence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tutor Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tutor Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tutor Intelligence
provider_slug: tutor-intelligence
slug: tutor-intelligence-domain-security
source_filename: tutor-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tutorintelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:58:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tutorintelligence.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tutor-intelligence/refs/heads/main/security/tutor-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Automation
- Warehouse Automation
- Logistics
- Manufacturing
- Artificial Intelligence
- Robots-as-a-Service
---
