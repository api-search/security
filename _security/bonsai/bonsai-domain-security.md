---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hellobonsai.com
  spf: true
hosts:
- cert_expires: Sep 18 04:20:32 2026 GMT
  host: hellobonsai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bonsai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonsai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bonsai
provider_slug: bonsai
slug: bonsai-domain-security
source_filename: bonsai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hellobonsai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:20:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hellobonsai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonsai/refs/heads/main/security/bonsai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B
- Business Management
- Freelancing
- Agencies
- CRM
- Project Management
- Time Tracking
- Invoicing
- Proposals
- Contracts
- Accounting
- MCP
---
