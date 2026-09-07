---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: inaccord.com
  spf: true
hosts:
- cert_expires: Oct 24 19:03:29 2026 GMT
  host: inaccord.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 22:16:20 2026 GMT
  host: developers.inaccord.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 16:33:25 2026 GMT
  host: api2.inaccord.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Accordacff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accord, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Accord
provider_slug: accordacff
slug: accordacff-domain-security
source_filename: accordacff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inaccord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 19:03:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.inaccord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 22:16:20 2026 GMT\n  hsts: false\n- host: api2.inaccord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:33:25 2026 GMT\n  hsts: null\ndomains:\n- domain: inaccord.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accordacff/refs/heads/main/security/accordacff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Sales Enablement
- Revenue Operations
- Customer Collaboration
- Sales Engagement
- Customer Onboarding
- Mutual Action Plans
- CRM
- GraphQL
- MCP
- agent-native
- SaaS
- Company
---
