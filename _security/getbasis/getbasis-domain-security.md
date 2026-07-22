---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getbasis.ai
  spf: true
hosts:
- cert_expires: Oct  2 12:21:03 2026 GMT
  host: www.getbasis.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getbasis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getbasis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Getbasis
provider_slug: getbasis
slug: getbasis-domain-security
source_filename: getbasis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getbasis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:21:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getbasis.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getbasis/refs/heads/main/security/getbasis-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Accounting
- Artificial Intelligence
- AI Agents
- Accounting Automation
- Fintech
- Tax
- Audit
---
