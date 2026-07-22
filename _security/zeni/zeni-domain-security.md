---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zeni.ai
  spf: true
hosts:
- cert_expires: Sep  5 21:31:05 2026 GMT
  host: zeni.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zeni
provider_slug: zeni
slug: zeni-domain-security
source_filename: zeni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeni.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 21:31:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zeni.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeni/refs/heads/main/security/zeni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Bookkeeping
- Accounting
- Financial Operations
- Startups
- MCP
- AI Agents
---
