---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: glama.ai
  spf: true
hosts:
- cert_expires: Oct  4 21:51:01 2026 GMT
  host: glama.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 17:48:31 2026 GMT
  host: gateway.glama.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glama Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glama, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Glama
provider_slug: glama-ai
slug: glama-ai-domain-security
source_filename: glama-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glama.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:51:01 2026 GMT\n  hsts: null\n- host: gateway.glama.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:48:31 2026 GMT\n  hsts: false\ndomains:\n- domain: glama.ai\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glama-ai/refs/heads/main/security/glama-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- MCP
- Model Context Protocol
- LLM Gateway
- MCP Gateway
- MCP Marketplace
- AI Workspace
- Multi-Provider
- OAuth
- Observability
---
