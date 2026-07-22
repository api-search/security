---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zocks.io
  spf: true
hosts:
- cert_expires: Oct 15 16:02:50 2026 GMT
  host: www.zocks.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zocks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zocks
provider_slug: zocks
slug: zocks-domain-security
source_filename: zocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 16:02:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zocks.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zocks/refs/heads/main/security/zocks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Wealthtech
- Financial Advisors
- Artificial Intelligence
- MCP
- Meeting Intelligence
- CRM
---
