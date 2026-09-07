---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: picklerobot.com
  spf: true
hosts:
- cert_expires: Oct  3 18:44:18 2026 GMT
  host: www.picklerobot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pickle Robot Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pickle Robot Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pickle Robot Company
provider_slug: pickle-robot-company
slug: pickle-robot-company-domain-security
source_filename: pickle-robot-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.picklerobot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:44:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: picklerobot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pickle-robot-company/refs/heads/main/security/pickle-robot-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Physical AI
- Supply Chain
- Logistics
- Warehouse Automation
- Artificial Intelligence
- Autonomous Systems
---
