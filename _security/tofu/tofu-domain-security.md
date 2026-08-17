---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tofuhq.com
  spf: true
hosts:
- cert_expires: Sep 28 21:20:24 2026 GMT
  host: tofuhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 20:25:31 2026 GMT
  host: enrich.tofuhq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 19:47:34 2026 GMT
  host: api.enrich.tofuhq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tofu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tofu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tofu
provider_slug: tofu
slug: tofu-domain-security
source_filename: tofu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tofuhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:20:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: enrich.tofuhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:25:31 2026 GMT\n  hsts: false\n- host: api.enrich.tofuhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:47:34 2026 GMT\n  hsts: false\ndomains:\n- domain: tofuhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tofu/refs/heads/main/security/tofu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Marketing
- Go-To-Market
- Sales
- Automation
- CRM
- Campaigns
- Data Enrichment
- Company Data
- People Data
- Lead Generation
- Agents
- Contact Data
---
