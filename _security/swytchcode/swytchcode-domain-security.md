---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: swytchcode.com
  spf: true
hosts:
- cert_expires: Aug 16 12:30:50 2026 GMT
  host: docs.swytchcode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swytchcode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swytchcode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Swytchcode
provider_slug: swytchcode
slug: swytchcode-domain-security
source_filename: swytchcode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.swytchcode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 12:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: swytchcode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swytchcode/refs/heads/main/security/swytchcode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI agent tooling
- agentic middleware
- API integration
- API orchestration
- API execution layer
- LLM tool execution
- MCP server
- developer tools
- API documentation
- API playground
---
