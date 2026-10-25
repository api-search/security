---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sursatech.com
  spf: true
hosts:
- cert_expires: Dec 14 07:48:54 2026 GMT
  host: www.sursatech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 07:51:31 2026 GMT
  host: api.sursatech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Sursatech Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SursaTech, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SursaTech
provider_slug: sursatech-com
slug: sursatech-com-domain-security
source_filename: sursatech-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sursatech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 07:48:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sursatech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 07:51:31 2026 GMT\n  hsts: null\ndomains:\n- domain: sursatech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sursatech-com/refs/heads/main/security/sursatech-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- A2A
- AI Consulting
- Product Engineering
- Software Development
- RAG
- QA Automation
- Nepal
- Agent-Native
- Company
---
