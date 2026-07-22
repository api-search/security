---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: salesape.ai
  spf: true
hosts:
- cert_expires: Oct 16 18:48:05 2026 GMT
  host: www.salesape.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salesape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Salesape
provider_slug: salesape
slug: salesape-domain-security
source_filename: salesape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.salesape.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 18:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: salesape.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesape/refs/heads/main/security/salesape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Artificial Intelligence
- Sales
- Lead Qualification
- AI Agents
- CRM
- Conversational AI
---
