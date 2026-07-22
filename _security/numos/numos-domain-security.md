---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: numos.ai
  spf: false
hosts:
- cert_expires: Aug 28 10:02:21 2026 GMT
  host: numos.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Numos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Numos
provider_slug: numos
slug: numos-domain-security
source_filename: numos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: numos.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numos/refs/heads/main/security/numos-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- AI Agents
- Accounting
- Finance
- FP&A
- Fintech
- Automation
- ERP
---
