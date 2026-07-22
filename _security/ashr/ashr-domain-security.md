---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ashr.io
  spf: true
hosts:
- cert_expires: Jul 24 23:59:59 2026 GMT
  host: ashr.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ashr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ashr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ashr
provider_slug: ashr
slug: ashr-domain-security
source_filename: ashr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ashr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ashr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ashr/refs/heads/main/security/ashr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Agents
- Agent Testing
- Evaluation
- Observability
- LLM
- Developer Tools
- SDK
---
