---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: revnu.com
  spf: true
hosts:
- cert_expires: Oct  5 19:35:43 2026 GMT
  host: revnu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revnu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revnu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Revnu
provider_slug: revnu
slug: revnu-domain-security
source_filename: revnu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revnu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:35:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: revnu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revnu/refs/heads/main/security/revnu-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Growth Automation
- Marketing
- Artificial Intelligence
- SaaS
- Startups
- Lead Generation
- SEO
- MCP
- Agents
- Commerce
- A/B Testing
---
