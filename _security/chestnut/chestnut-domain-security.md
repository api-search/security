---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chestnutfi.com
  spf: true
hosts:
- cert_expires: Oct  7 10:26:18 2026 GMT
  host: www.chestnutfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chestnut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chestnut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chestnut
provider_slug: chestnut
slug: chestnut-domain-security
source_filename: chestnut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chestnutfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:26:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chestnutfi.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chestnut/refs/heads/main/security/chestnut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Insurance Distribution
- Producer Management
- Incentive Compensation
- Agentic AI
- MCP
- API-First
---
