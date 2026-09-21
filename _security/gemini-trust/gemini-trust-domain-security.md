---
api_specs:
- filename: gemini-trust-rest-openapi.yml
  format: yaml
  label: Gemini Crypto Trading REST API
  slug: gemini-crypto-trading-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-rest-openapi.yml
- filename: gemini-trust-prediction-markets-openapi.yml
  format: yaml
  label: Gemini Prediction Markets REST API
  slug: gemini-prediction-markets-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-prediction-markets-openapi.yml
- filename: gemini-trust-websocket-asyncapi.yml
  format: yaml
  label: Gemini WebSocket API
  slug: gemini-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/asyncapi/gemini-trust-websocket-asyncapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@gemini.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gemini.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: www.gemini.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: developer.gemini.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.gemini.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Gemini Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gemini Trust Company, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gemini Trust Company
provider_slug: gemini-trust
slug: gemini-trust-domain-security
source_filename: gemini-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gemini.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.gemini.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\n- host: api.gemini.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gemini.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@gemini.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/security/gemini-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Order Management
- Clearing
- Custody
- Financial-Services
- Prediction Markets
- Staking
- Derivatives
- WebSocket
- FIX
---
