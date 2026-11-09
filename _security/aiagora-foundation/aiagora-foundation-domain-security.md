---
api_specs:
- filename: aiagora-foundation-agents-api-openapi.yml
  format: yaml
  label: AIAgora Agents API
  slug: aiagora-foundation-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-agents-api-openapi.yml
- filename: aiagora-foundation-health-api-openapi.yml
  format: yaml
  label: AIAgora Health API
  slug: aiagora-foundation-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-health-api-openapi.yml
- filename: aiagora-foundation-hosts-api-openapi.yml
  format: yaml
  label: AIAgora Hosts API
  slug: aiagora-foundation-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-hosts-api-openapi.yml
- filename: aiagora-foundation-receipts-api-openapi.yml
  format: yaml
  label: AIAgora Receipts API
  slug: aiagora-foundation-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-receipts-api-openapi.yml
- filename: aiagora-foundation-sandbox-api-openapi.yml
  format: yaml
  label: AIAgora Sandbox API
  slug: aiagora-foundation-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-sandbox-api-openapi.yml
- filename: aiagora-foundation-stats-api-openapi.yml
  format: yaml
  label: AIAgora Stats API
  slug: aiagora-foundation-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aiagora.foundation
  spf: true
hosts:
- cert_expires: Dec 24 03:50:49 2026 GMT
  host: aiagora.foundation
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiagora Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIAgora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AIAgora
provider_slug: aiagora-foundation
slug: aiagora-foundation-domain-security
source_filename: aiagora-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiagora.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 03:50:49 2026 GMT\n  hsts: null\ndomains:\n- domain: aiagora.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aiagora-foundation/security/aiagora-foundation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Agents
- Collaboration
- Sandbox
- Open Platform
---
