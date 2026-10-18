---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: llmscout.com
  spf: false
hosts:
- cert_expires: Jan  2 22:45:02 2027 GMT
  host: llmscout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmscout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLM Scout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LLM Scout
provider_slug: llmscout
slug: llmscout-domain-security
source_filename: llmscout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 22:45:02 2027 GMT\n  hsts: false\ndomains:\n- domain: llmscout.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmscout/refs/heads/main/security/llmscout-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Verification
- Safety
- Compliance
---
