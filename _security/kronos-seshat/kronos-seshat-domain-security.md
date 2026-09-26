---
api_specs:
- filename: kronos-seshat-agent-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Agent API
  slug: kronos-seshat-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-agent-api-openapi.yml
- filename: kronos-seshat-agent-intelligence-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Agent Intelligence API
  slug: kronos-seshat-agent-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-agent-intelligence-api-openapi.yml
- filename: kronos-seshat-analysis-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Analysis API
  slug: kronos-seshat-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-analysis-api-openapi.yml
- filename: kronos-seshat-discovery-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Discovery API
  slug: kronos-seshat-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-discovery-api-openapi.yml
- filename: kronos-seshat-experimental-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Experimental API
  slug: kronos-seshat-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-experimental-api-openapi.yml
- filename: kronos-seshat-forecast-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Forecast API
  slug: kronos-seshat-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-forecast-api-openapi.yml
- filename: kronos-seshat-market-intelligence-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Market Intelligence API
  slug: kronos-seshat-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-market-intelligence-api-openapi.yml
- filename: kronos-seshat-semantic-similarity-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Semantic Similarity API
  slug: kronos-seshat-semantic-similarity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-semantic-similarity-api-openapi.yml
- filename: kronos-seshat-signal-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Signal API
  slug: kronos-seshat-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-signal-api-openapi.yml
- filename: kronos-seshat-verification-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Verification API
  slug: kronos-seshat-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-verification-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild ";"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
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
name: Kronos Seshat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kronos Quant Signal API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kronos Quant Signal API
provider_slug: kronos-seshat
slug: kronos-seshat-domain-security
source_filename: kronos-seshat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kronos.seshat.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 02:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seshat.markets\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \";\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/security/kronos-seshat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Crypto
- Financial Forecast
- API
- Market Data
- Auditing
- Micropayments
---
