---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clarity.ai
  spf: true
hosts:
- cert_expires: Sep 29 22:14:19 2026 GMT
  host: clarity.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clarity Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clarity AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clarity AI
provider_slug: clarity-ai
slug: clarity-ai-domain-security
source_filename: clarity-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clarity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:14:19 2026 GMT\n  hsts: false\ndomains:\n- domain: clarity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarity-ai/refs/heads/main/security/clarity-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Sustainability
- ESG
- Climate
- Fintech
- Regulatory Compliance
- Data
---
