---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: harvey.ai
  spf: true
hosts:
- cert_expires: Sep 18 11:48:08 2026 GMT
  host: www.harvey.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harvey Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harvey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Harvey
provider_slug: harvey-ai
slug: harvey-ai-domain-security
source_filename: harvey-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harvey.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: harvey.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harvey-ai/refs/heads/main/security/harvey-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LegalTech
- Law Firms
- Legal Research
- Contract Analysis
- Due Diligence
- Litigation
- Workflow Agents
- Enterprise
- Vault
---
