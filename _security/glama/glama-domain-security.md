---
api_specs:
- filename: glama-openapi.yml
  format: yaml
  label: Glama MCP Marketplace & Gateway
  slug: mcp-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: glama.ai
  spf: true
hosts:
- cert_expires: Oct  4 21:51:01 2026 GMT
  host: glama.ai
  hsts: true
  hsts_max_age: 31536000
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
name: Glama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glama AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Glama AI
provider_slug: glama
slug: glama-domain-security
source_filename: glama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glama.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:51:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.glama.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:48:31 2026 GMT\n  hsts: false\ndomains:\n- domain: glama.ai\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/security/glama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- MCP
- Model Context Protocol
- MCP Marketplace
- MCP Gateway
- MCP Hosting
- MCP Inspector
- AI Gateway
- LLM Gateway
- Connectors
- OAuth
- Observability
- Multi-Provider
---
