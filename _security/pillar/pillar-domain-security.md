---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pillar.it
  spf: true
hosts:
- cert_expires: Aug 24 05:25:08 2026 GMT
  host: pillar.it
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pillar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pillar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pillar
provider_slug: pillar
slug: pillar-domain-security
source_filename: pillar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pillar.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:25:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pillar.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pillar/refs/heads/main/security/pillar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Construction Technology
- ConTech
- Vertical SaaS
- Invoicing
- Cash Flow Management
- Procurement
- Project Management
- Field Management
- Artificial Intelligence
- Italy
---
