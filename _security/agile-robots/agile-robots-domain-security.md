---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agile-robots.com
  spf: true
hosts:
- cert_expires: Nov 23 07:18:15 2026 GMT
  host: www.agile-robots.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agile Robots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agile Robots, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agile Robots
provider_slug: agile-robots
slug: agile-robots-domain-security
source_filename: agile-robots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agile-robots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 07:18:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agile-robots.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agile-robots/refs/heads/main/security/agile-robots-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Technology
- Robotics
- Artificial Intelligence
- Automation
- Industrial Robots
- Manufacturing
- Germany
---
