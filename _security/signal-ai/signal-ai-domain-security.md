---
api_specs:
- filename: signal-ai-affinity-api-openapi.yml
  format: yaml
  label: Signal AI Affinity API
  slug: signal-ai-affinity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-affinity-api-openapi.yml
- filename: signal-ai-categories-api-openapi.yml
  format: yaml
  label: Signal AI Categories API
  slug: signal-ai-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-categories-api-openapi.yml
- filename: signal-ai-content-metrics-api-openapi.yml
  format: yaml
  label: Signal AI Content Metrics API
  slug: signal-ai-content-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-content-metrics-api-openapi.yml
- filename: signal-ai-content-search-api-openapi.yml
  format: yaml
  label: Signal AI Content Search API
  slug: signal-ai-content-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-content-search-api-openapi.yml
- filename: signal-ai-entities-api-openapi.yml
  format: yaml
  label: Signal AI Entities API
  slug: signal-ai-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-entities-api-openapi.yml
- filename: signal-ai-events-api-openapi.yml
  format: yaml
  label: Signal AI Events API
  slug: signal-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-events-api-openapi.yml
- filename: signal-ai-openapi-json-api-openapi.yml
  format: yaml
  label: Signal AI Openapi.json API
  slug: signal-ai-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-openapi-json-api-openapi.yml
- filename: signal-ai-publication-sources-api-openapi.yml
  format: yaml
  label: Signal AI Publication sources API
  slug: signal-ai-publication-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-publication-sources-api-openapi.yml
- filename: signal-ai-risk-events-api-openapi.yml
  format: yaml
  label: Signal AI Risk Events API
  slug: signal-ai-risk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-risk-events-api-openapi.yml
- filename: signal-ai-topics-api-openapi.yml
  format: yaml
  label: Signal AI Topics API
  slug: signal-ai-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-topics-api-openapi.yml
- filename: signal-ai-organisation-api-openapi.yml
  format: yaml
  label: Signal AI Organisation API
  slug: signal-ai-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-organisation-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: signal-ai.com
  spf: true
hosts:
- cert_expires: Nov  5 17:56:24 2026 GMT
  host: signal-ai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 17:56:24 2026 GMT
  host: api.signal-ai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signal Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signal AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Signal AI
provider_slug: signal-ai
slug: signal-ai-domain-security
source_filename: signal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signal-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 17:56:24 2026 GMT\n  hsts: false\n- host: api.signal-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 17:56:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: signal-ai.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/security/signal-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Media Intelligence
- Reputation Management
- Risk Intelligence
- News
- Content Search
- Knowledge Graph
- ESG
- Artificial Intelligence
- Analytics
---
