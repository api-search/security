---
api_specs:
- filename: observeai-ack-dispute-flow-api-openapi.yml
  format: yaml
  label: Observe.AI Ack Dispute Flow API
  slug: observeai-ack-dispute-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/openapi/observeai-ack-dispute-flow-api-openapi.yml
- filename: observeai-authentication-api-openapi.yml
  format: yaml
  label: Observe.AI Authentication API
  slug: observeai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/openapi/observeai-authentication-api-openapi.yml
- filename: observeai-coachings-api-openapi.yml
  format: yaml
  label: Observe.AI Coachings API
  slug: observeai-coachings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/openapi/observeai-coachings-api-openapi.yml
- filename: observeai-dsr-api-openapi.yml
  format: yaml
  label: Observe.AI DSR API
  slug: observeai-dsr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/openapi/observeai-dsr-api-openapi.yml
- filename: observeai-evaluations-api-openapi.yml
  format: yaml
  label: Observe.AI Evaluations API
  slug: observeai-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/openapi/observeai-evaluations-api-openapi.yml
- filename: observeai-interactions-api-openapi.yml
  format: yaml
  label: Observe.AI Interactions API
  slug: observeai-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/openapi/observeai-interactions-api-openapi.yml
- filename: observeai-summary-api-openapi.yml
  format: yaml
  label: Observe.AI Summary API
  slug: observeai-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/openapi/observeai-summary-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: observe.ai
  spf: true
hosts:
- cert_expires: Oct 30 07:17:18 2026 GMT
  host: www.observe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api-docs.observe.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: kong.observe.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Observeai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Observe.AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Observe.AI
provider_slug: observeai
slug: observeai-domain-security
source_filename: observeai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.observe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 07:17:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.observe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: kong.observe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: observe.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/security/observeai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Contact Center
- Conversation Intelligence
- Customer-Support
- Agentic AI
- Voice AI
- Quality Assurance
- Reporting
- OpenAPI
- Speech Analytics
---
