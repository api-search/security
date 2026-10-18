---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: llmpricecheck.com
  spf: false
hosts:
- cert_expires: Nov 25 05:42:56 2026 GMT
  host: llmpricecheck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmpricecheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLM Price Check, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LLM Price Check
provider_slug: llmpricecheck
slug: llmpricecheck-domain-security
source_filename: llmpricecheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmpricecheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 05:42:56 2026 GMT\n  hsts: false\ndomains:\n- domain: llmpricecheck.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmpricecheck/refs/heads/main/security/llmpricecheck-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Pricing
- LLM
- Comparison
---
