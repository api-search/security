---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: proximitty.ai
  spf: true
hosts:
- cert_expires: Aug 20 02:43:18 2026 GMT
  host: www.proximitty.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proximitty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proximitty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Proximitty
provider_slug: proximitty
slug: proximitty-domain-security
source_filename: proximitty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proximitty.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 02:43:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: proximitty.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proximitty/refs/heads/main/security/proximitty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Financial Services
- Commercial Lending
- Banking
- Fintech
- Underwriting
- Regulatory Compliance
---
