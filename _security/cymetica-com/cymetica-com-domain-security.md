---
api_specs:
- filename: cymetica-com-eventtrader-public-api-openapi.yml
  format: yaml
  label: EventTrader Public API
  slug: eventtrader-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cymetica-com/refs/heads/main/openapi/cymetica-com-eventtrader-public-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:contact@cymetica.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cymetica.com
  spf: true
hosts:
- cert_expires: Oct 21 03:01:08 2026 GMT
  host: cymetica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cymetica Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cymetica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cymetica
provider_slug: cymetica-com
slug: cymetica-com-domain-security
source_filename: cymetica-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cymetica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 03:01:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cymetica.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:contact@cymetica.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cymetica-com/refs/heads/main/security/cymetica-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Prediction Markets
- Cryptocurrency Exchange
- Trading
- AI Agents
- MCP
- Agent-Native
- Blockchain
- DeFi
- Financial Services
- Market Data
- A2A
- Real-Time
---
