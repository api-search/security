---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentic-prompt.com
  spf: false
hosts:
- cert_expires: Jan  9 12:20:50 2027 GMT
  host: agentic-prompt.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentic Prompt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentic Prompt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Agentic Prompt
provider_slug: agentic-prompt-com
slug: agentic-prompt-com-domain-security
source_filename: agentic-prompt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentic-prompt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 12:20:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: agentic-prompt.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentic-prompt-com/security/agentic-prompt-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Trading
- Prompts
- Claude
- Robinhood
---
