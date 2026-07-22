---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zarnaai.com
  spf: true
hosts:
- cert_expires: Oct 18 22:03:55 2026 GMT
  host: www.zarnaai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zarna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zarna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zarna
provider_slug: zarna
slug: zarna-domain-security
source_filename: zarna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zarnaai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zarnaai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zarna/refs/heads/main/security/zarna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Private Equity
- Investments
- Financial Services
- Deal Management
---
