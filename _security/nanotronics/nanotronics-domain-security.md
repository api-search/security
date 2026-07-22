---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nanotronics.co
  spf: true
hosts:
- cert_expires: Oct  2 21:13:07 2026 GMT
  host: www.nanotronics.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nanotronics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanotronics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nanotronics
provider_slug: nanotronics
slug: nanotronics-domain-security
source_filename: nanotronics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nanotronics.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nanotronics.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanotronics/refs/heads/main/security/nanotronics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Manufacturing
- Artificial Intelligence
- Machine Learning
- Industrial Automation
- Inspection
---
