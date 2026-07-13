---
api_specs:
- filename: regal-events-api-openapi.yml
  format: yaml
  label: Regal Events API
  slug: regal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-events-api-openapi.yml
- filename: regal-branded-phone-numbers-api-openapi.yml
  format: yaml
  label: Regal Branded Phone Numbers API
  slug: regal-branded-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-branded-phone-numbers-api-openapi.yml
- filename: regal-management-api-openapi.yml
  format: yaml
  label: Regal Management API
  slug: regal-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-management-api-openapi.yml
- filename: regal-messages-api-openapi.yml
  format: yaml
  label: Regal Messages API
  slug: regal-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-messages-api-openapi.yml
- filename: regal-reporting-webhooks-asyncapi.yml
  format: yaml
  label: Regal Reporting Webhooks
  slug: regal-reporting-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/asyncapi/regal-reporting-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: regal.ai
  spf: true
hosts:
- cert_expires: Aug 16 22:29:38 2026 GMT
  host: www.regal.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:15:31 2026 GMT
  host: developer.regal.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: api.regal.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regal Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Regal
provider_slug: regal-ai
slug: regal-ai-domain-security
source_filename: regal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 22:29:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.regal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:15:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.regal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: regal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/security/regal-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- AI Agents
- Voice AI
- Contact Center
- Outbound Calling
- Inbound Calling
- Phone Agents
- SMS
- Chat
- WebRTC
- Conversation Intelligence
- Journey Orchestration
- Branded Caller ID
- CCaaS
- CPaaS
- Sales Dialer
- Customer Engagement
---
