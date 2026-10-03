---
api_specs:
- filename: itsgloria-ai-api-keys-api-openapi.yml
  format: yaml
  label: Gloria API Keys API
  slug: itsgloria-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-api-keys-api-openapi.yml
- filename: itsgloria-ai-articles-api-openapi.yml
  format: yaml
  label: Gloria Articles API
  slug: itsgloria-ai-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-articles-api-openapi.yml
- filename: itsgloria-ai-authentication-api-openapi.yml
  format: yaml
  label: Gloria Authentication API
  slug: itsgloria-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-authentication-api-openapi.yml
- filename: itsgloria-ai-bots-api-openapi.yml
  format: yaml
  label: Gloria Bots API
  slug: itsgloria-ai-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-bots-api-openapi.yml
- filename: itsgloria-ai-categories-api-openapi.yml
  format: yaml
  label: Gloria Categories API
  slug: itsgloria-ai-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-categories-api-openapi.yml
- filename: itsgloria-ai-health-api-openapi.yml
  format: yaml
  label: Gloria Health API
  slug: itsgloria-ai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-health-api-openapi.yml
- filename: itsgloria-ai-narratives-api-openapi.yml
  format: yaml
  label: Gloria Narratives API
  slug: itsgloria-ai-narratives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-narratives-api-openapi.yml
- filename: itsgloria-ai-news-api-openapi.yml
  format: yaml
  label: Gloria News API
  slug: itsgloria-ai-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-news-api-openapi.yml
- filename: itsgloria-ai-recaps-api-openapi.yml
  format: yaml
  label: Gloria Recaps API
  slug: itsgloria-ai-recaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-recaps-api-openapi.yml
- filename: itsgloria-ai-websocket-api-openapi.yml
  format: yaml
  label: Gloria WebSocket API
  slug: itsgloria-ai-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/openapi/itsgloria-ai-websocket-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: itsgloria.ai
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cryptobriefing.com
  spf: true
hosts:
- cert_expires: Dec 11 15:26:20 2026 GMT
  host: itsgloria.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 21:29:17 2026 GMT
  host: docs.itsgloria.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 05:19:35 2026 GMT
  host: ai-hub.cryptobriefing.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Itsgloria Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gloria, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gloria
provider_slug: itsgloria-ai
slug: itsgloria-ai-domain-security
source_filename: itsgloria-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itsgloria.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 15:26:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.itsgloria.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 21:29:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: ai-hub.cryptobriefing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 05:19:35 2026 GMT\n  hsts: null\ndomains:\n- domain: itsgloria.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cryptobriefing.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itsgloria-ai/refs/heads/main/security/itsgloria-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- News
- Crypto
- Cryptocurrency
- Market Intelligence
- Sentiment Analysis
- Prediction Markets
- Artificial Intelligence
- MCP
- x402
- WebSocket
- Agents
---
