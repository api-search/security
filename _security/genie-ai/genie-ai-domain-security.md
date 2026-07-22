---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: genieai.co
  spf: true
hosts:
- cert_expires: Sep 21 07:49:00 2026 GMT
  host: www.genieai.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genie Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genie AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Genie AI
provider_slug: genie-ai
slug: genie-ai-domain-security
source_filename: genie-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genieai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:49:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genieai.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genie-ai/refs/heads/main/security/genie-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Legal
- LegalTech
- Contracts
- Contract Management
- Legal AI
- Document Automation
- Compliance
- Agents
---
