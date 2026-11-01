---
api_specs:
- filename: satoshidata-ai-batch-api-openapi.yml
  format: yaml
  label: satoshidata-ai Batch API
  slug: satoshidata-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-batch-api-openapi.yml
- filename: satoshidata-ai-billing-api-openapi.yml
  format: yaml
  label: satoshidata-ai Billing API
  slug: satoshidata-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-billing-api-openapi.yml
- filename: satoshidata-ai-chain-api-openapi.yml
  format: yaml
  label: satoshidata-ai Chain API
  slug: satoshidata-ai-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-chain-api-openapi.yml
- filename: satoshidata-ai-community-api-openapi.yml
  format: yaml
  label: satoshidata-ai Community API
  slug: satoshidata-ai-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-community-api-openapi.yml
- filename: satoshidata-ai-discovery-api-openapi.yml
  format: yaml
  label: satoshidata-ai Discovery API
  slug: satoshidata-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-discovery-api-openapi.yml
- filename: satoshidata-ai-entities-api-openapi.yml
  format: yaml
  label: satoshidata-ai Entities API
  slug: satoshidata-ai-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-entities-api-openapi.yml
- filename: satoshidata-ai-feedback-api-openapi.yml
  format: yaml
  label: satoshidata-ai Feedback API
  slug: satoshidata-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-feedback-api-openapi.yml
- filename: satoshidata-ai-health-api-openapi.yml
  format: yaml
  label: satoshidata-ai Health API
  slug: satoshidata-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-health-api-openapi.yml
- filename: satoshidata-ai-labels-api-openapi.yml
  format: yaml
  label: satoshidata-ai Labels API
  slug: satoshidata-ai-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-labels-api-openapi.yml
- filename: satoshidata-ai-market-api-openapi.yml
  format: yaml
  label: satoshidata-ai Market API
  slug: satoshidata-ai-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-market-api-openapi.yml
- filename: satoshidata-ai-metrics-api-openapi.yml
  format: yaml
  label: satoshidata-ai Metrics API
  slug: satoshidata-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-metrics-api-openapi.yml
- filename: satoshidata-ai-risk-api-openapi.yml
  format: yaml
  label: satoshidata-ai Risk API
  slug: satoshidata-ai-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-risk-api-openapi.yml
- filename: satoshidata-ai-sanctions-api-openapi.yml
  format: yaml
  label: satoshidata-ai Sanctions API
  slug: satoshidata-ai-sanctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-sanctions-api-openapi.yml
- filename: satoshidata-ai-timestamping-api-openapi.yml
  format: yaml
  label: satoshidata-ai Timestamping API
  slug: satoshidata-ai-timestamping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-timestamping-api-openapi.yml
- filename: satoshidata-ai-wallets-api-openapi.yml
  format: yaml
  label: satoshidata-ai Wallets API
  slug: satoshidata-ai-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-wallets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:radotz@gmail.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: satoshidata.ai
  spf: true
hosts:
- cert_expires: Dec  9 05:02:38 2026 GMT
  host: satoshidata.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Satoshidata Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for satoshidata-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: satoshidata-ai
provider_slug: satoshidata-ai
slug: satoshidata-ai-domain-security
source_filename: satoshidata-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: satoshidata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 05:02:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: satoshidata.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:radotz@gmail.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/satoshidata-ai/security/satoshidata-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bitcoin
- API
- AI
- Finance
- Chain-Intelligence
- Company
---
