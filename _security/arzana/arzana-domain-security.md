---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arzana.com
  spf: true
hosts:
- cert_expires: Aug 23 18:22:49 2026 GMT
  host: www.arzana.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arzana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arzana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arzana
provider_slug: arzana
slug: arzana-domain-security
source_filename: arzana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arzana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arzana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arzana/refs/heads/main/security/arzana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- ERP
- AI Agents
- Automation
- CRM
- Office Automation
- Distribution
- Y Combinator
---
