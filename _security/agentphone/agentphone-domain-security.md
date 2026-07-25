---
api_specs:
- filename: agentphone-agent-webhooks-api-openapi.yml
  format: yaml
  label: AgentPhone agent-webhooks API
  slug: agentphone-agent-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-agent-webhooks-api-openapi.yml
- filename: agentphone-agents-api-openapi.yml
  format: yaml
  label: AgentPhone agents API
  slug: agentphone-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-agents-api-openapi.yml
- filename: agentphone-calls-api-openapi.yml
  format: yaml
  label: AgentPhone calls API
  slug: agentphone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-calls-api-openapi.yml
- filename: agentphone-contactcards-api-openapi.yml
  format: yaml
  label: AgentPhone contactCards API
  slug: agentphone-contactcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-contactcards-api-openapi.yml
- filename: agentphone-contacts-api-openapi.yml
  format: yaml
  label: AgentPhone contacts API
  slug: agentphone-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-contacts-api-openapi.yml
- filename: agentphone-conversations-api-openapi.yml
  format: yaml
  label: AgentPhone conversations API
  slug: agentphone-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-conversations-api-openapi.yml
- filename: agentphone-location-api-openapi.yml
  format: yaml
  label: AgentPhone location API
  slug: agentphone-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-location-api-openapi.yml
- filename: agentphone-messages-api-openapi.yml
  format: yaml
  label: AgentPhone messages API
  slug: agentphone-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-messages-api-openapi.yml
- filename: agentphone-numbers-api-openapi.yml
  format: yaml
  label: AgentPhone numbers API
  slug: agentphone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-numbers-api-openapi.yml
- filename: agentphone-registration-api-openapi.yml
  format: yaml
  label: AgentPhone registration API
  slug: agentphone-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-registration-api-openapi.yml
- filename: agentphone-sub-accounts-api-openapi.yml
  format: yaml
  label: AgentPhone sub-accounts API
  slug: agentphone-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-sub-accounts-api-openapi.yml
- filename: agentphone-usage-api-openapi.yml
  format: yaml
  label: AgentPhone usage API
  slug: agentphone-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-usage-api-openapi.yml
- filename: agentphone-webhooks-api-openapi.yml
  format: yaml
  label: AgentPhone webhooks API
  slug: agentphone-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentphone.ai
  spf: true
hosts:
- cert_expires: Oct  1 10:23:20 2026 GMT
  host: api.agentphone.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentphone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentPhone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AgentPhone
provider_slug: agentphone
slug: agentphone-domain-security
source_filename: agentphone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.agentphone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:23:20 2026 GMT\n  hsts: null\ndomains:\n- domain: agentphone.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/security/agentphone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telephony
- Phone Numbers
- SMS
- Voice
- AI Agents
- Messaging
- Communications
- Webhooks
- MCP
- iMessage
---
