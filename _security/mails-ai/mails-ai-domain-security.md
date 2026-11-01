---
api_specs:
- filename: mails-ai-account-api-openapi.yml
  format: yaml
  label: mails-ai Account API
  slug: mails-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-account-api-openapi.yml
- filename: mails-ai-agents-api-openapi.yml
  format: yaml
  label: mails-ai Agents API
  slug: mails-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-agents-api-openapi.yml
- filename: mails-ai-api-keys-api-openapi.yml
  format: yaml
  label: mails-ai API Keys API
  slug: mails-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-api-keys-api-openapi.yml
- filename: mails-ai-billing-api-openapi.yml
  format: yaml
  label: mails-ai Billing API
  slug: mails-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-billing-api-openapi.yml
- filename: mails-ai-connected-apps-api-openapi.yml
  format: yaml
  label: mails-ai Connected Apps API
  slug: mails-ai-connected-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-connected-apps-api-openapi.yml
- filename: mails-ai-domains-api-openapi.yml
  format: yaml
  label: mails-ai Domains API
  slug: mails-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-domains-api-openapi.yml
- filename: mails-ai-drafts-api-openapi.yml
  format: yaml
  label: mails-ai Drafts API
  slug: mails-ai-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-drafts-api-openapi.yml
- filename: mails-ai-events-api-openapi.yml
  format: yaml
  label: mails-ai Events API
  slug: mails-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-events-api-openapi.yml
- filename: mails-ai-inbound-api-openapi.yml
  format: yaml
  label: mails-ai Inbound API
  slug: mails-ai-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-inbound-api-openapi.yml
- filename: mails-ai-labels-api-openapi.yml
  format: yaml
  label: mails-ai Labels API
  slug: mails-ai-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-labels-api-openapi.yml
- filename: mails-ai-logs-api-openapi.yml
  format: yaml
  label: mails-ai Logs API
  slug: mails-ai-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-logs-api-openapi.yml
- filename: mails-ai-messages-api-openapi.yml
  format: yaml
  label: mails-ai Messages API
  slug: mails-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-messages-api-openapi.yml
- filename: mails-ai-metrics-api-openapi.yml
  format: yaml
  label: mails-ai Metrics API
  slug: mails-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-metrics-api-openapi.yml
- filename: mails-ai-public-api-openapi.yml
  format: yaml
  label: mails-ai Public API
  slug: mails-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-public-api-openapi.yml
- filename: mails-ai-reputation-api-openapi.yml
  format: yaml
  label: mails-ai Reputation API
  slug: mails-ai-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-reputation-api-openapi.yml
- filename: mails-ai-search-api-openapi.yml
  format: yaml
  label: mails-ai Search API
  slug: mails-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-search-api-openapi.yml
- filename: mails-ai-suppression-api-openapi.yml
  format: yaml
  label: mails-ai Suppression API
  slug: mails-ai-suppression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-suppression-api-openapi.yml
- filename: mails-ai-threads-api-openapi.yml
  format: yaml
  label: mails-ai Threads API
  slug: mails-ai-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-threads-api-openapi.yml
- filename: mails-ai-webhooks-api-openapi.yml
  format: yaml
  label: mails-ai Webhooks API
  slug: mails-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mails.ai
  spf: true
hosts:
- cert_expires: Jan  7 13:42:48 2027 GMT
  host: mails.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mails Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mails-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: mails-ai
provider_slug: mails-ai
slug: mails-ai-domain-security
source_filename: mails-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mails.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 13:42:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mails.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mails-ai/security/mails-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Email
- Infrastructure
- Agents
---
