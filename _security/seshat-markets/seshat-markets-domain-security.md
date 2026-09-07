---
api_specs:
- filename: seshat-markets-kronos-quant-signal-api-openapi.json
  format: json
  label: Kronos Quant Signal REST API
  slug: kronos-quant-signal-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-kronos-quant-signal-api-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:admin@seshat.markets"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: seshat.markets
  spf: true
hosts:
- cert_expires: Dec  3 02:15:03 2026 GMT
  host: kronos.seshat.markets
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seshat Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seshat Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Seshat Markets
provider_slug: seshat-markets
slug: seshat-markets-domain-security
source_filename: seshat-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kronos.seshat.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 02:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seshat.markets\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:admin@seshat.markets\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/security/seshat-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- finance
- fintech
- crypto
- commodities
- forecasting
- prediction
- market-data
- trading-signals
- research
- ai-agents
- mcp
- a2a
- x402
- llms-txt
- agent-skills
---
