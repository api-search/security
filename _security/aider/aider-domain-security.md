---
api_specs:
- filename: aider-cli-openapi.yml
  format: yaml
  label: Aider CLI
  slug: cli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-cli-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: true
  domain: aider.chat
  spf: false
hosts:
- cert_expires: Sep 26 20:23:51 2026 GMT
  host: aider.chat
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aider Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aider, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Aider
provider_slug: aider
slug: aider-domain-security
source_filename: aider-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aider.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:23:51 2026 GMT\n  hsts: false\ndomains:\n- domain: aider.chat\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/security/aider-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- AI
- AI Pair Programming
- Developer Tools
- CLI
- Command Line
- Coding Assistant
- Code Generation
- Open Source
- Python
- Apache 2.0
- LLM
- Git
- BYO LLM
- Terminal
- Polyglot
- Tree Sitter
- Repository Map
- Pair Programming
---
