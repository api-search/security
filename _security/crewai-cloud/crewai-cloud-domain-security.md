---
api_specs:
- filename: crewai-amp-rest-api-openapi.yml
  format: yaml
  label: CrewAI AMP REST API
  slug: crewai-amp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crewai-cloud/refs/heads/main/openapi/crewai-amp-rest-api-openapi.yml
- filename: crewai-amp-webhooks-asyncapi.yml
  format: yaml
  label: CrewAI AMP Webhook Streaming
  slug: crewai-amp-webhook-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/crewai-cloud/refs/heads/main/asyncapi/crewai-amp-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crewai.com
  spf: true
hosts:
- cert_expires: Aug 24 16:10:20 2026 GMT
  host: www.crewai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 12:45:45 2026 GMT
  host: docs.crewai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crewai Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrewAI Cloud, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CrewAI Cloud
provider_slug: crewai-cloud
slug: crewai-cloud-domain-security
source_filename: crewai-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crewai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:10:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.crewai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crewai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crewai-cloud/refs/heads/main/security/crewai-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- AI Agent Platform
- Agent Orchestration
- Multi-Agent Systems
- Agent Management Platform
- Managed Agents
- Automations
- Observability
- Human In The Loop
---
