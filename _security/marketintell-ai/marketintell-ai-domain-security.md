---
api_specs:
- filename: marketintell-ai-agent-execution-api-openapi.yml
  format: yaml
  label: MarketIntell Agent Execution API
  slug: marketintell-ai-agent-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-agent-execution-api-openapi.yml
- filename: marketintell-ai-agents-api-openapi.yml
  format: yaml
  label: MarketIntell Agents API
  slug: marketintell-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-agents-api-openapi.yml
- filename: marketintell-ai-alpha-api-openapi.yml
  format: yaml
  label: MarketIntell Alpha API
  slug: marketintell-ai-alpha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-alpha-api-openapi.yml
- filename: marketintell-ai-billing-api-openapi.yml
  format: yaml
  label: MarketIntell Billing API
  slug: marketintell-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-billing-api-openapi.yml
- filename: marketintell-ai-brain-api-openapi.yml
  format: yaml
  label: MarketIntell Brain API
  slug: marketintell-ai-brain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-brain-api-openapi.yml
- filename: marketintell-ai-brokers-api-openapi.yml
  format: yaml
  label: MarketIntell Brokers API
  slug: marketintell-ai-brokers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-brokers-api-openapi.yml
- filename: marketintell-ai-leaderboard-api-openapi.yml
  format: yaml
  label: MarketIntell Leaderboard API
  slug: marketintell-ai-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-leaderboard-api-openapi.yml
- filename: marketintell-ai-proof-api-openapi.yml
  format: yaml
  label: MarketIntell Proof API
  slug: marketintell-ai-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-proof-api-openapi.yml
- filename: marketintell-ai-screener-api-openapi.yml
  format: yaml
  label: MarketIntell Screener API
  slug: marketintell-ai-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-screener-api-openapi.yml
- filename: marketintell-ai-sessions-api-openapi.yml
  format: yaml
  label: MarketIntell Sessions API
  slug: marketintell-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-sessions-api-openapi.yml
- filename: marketintell-ai-signals-api-openapi.yml
  format: yaml
  label: MarketIntell Signals API
  slug: marketintell-ai-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-signals-api-openapi.yml
- filename: marketintell-ai-system-api-openapi.yml
  format: yaml
  label: MarketIntell System API
  slug: marketintell-ai-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-system-api-openapi.yml
- filename: marketintell-ai-trades-api-openapi.yml
  format: yaml
  label: MarketIntell Trades API
  slug: marketintell-ai-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-trades-api-openapi.yml
- filename: marketintell-ai-webhooks-api-openapi.yml
  format: yaml
  label: MarketIntell Webhooks API
  slug: marketintell-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketintell-ai/openapi/marketintell-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:postmaster@marketintell.ai"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: marketintell.ai
  spf: true
hosts:
- cert_expires: Jan 24 23:06:17 2027 GMT
  host: marketintell.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MarketIntell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketIntell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MarketIntell
provider_slug: marketintell-ai
slug: marketintell-ai-domain-security
source_filename: marketintell-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketintell.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:06:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marketintell.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:postmaster@marketintell.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/marketintell-ai/security/marketintell-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Market Intelligence
- Cryptocurrency
- Stocks
- Trading Signals
---
