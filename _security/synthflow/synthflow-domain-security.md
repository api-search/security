---
api_specs:
- filename: synthflow-default-api-openapi.yml
  format: yaml
  label: Synthflow Default API
  slug: synthflow-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-default-api-openapi.yml
- filename: synthflow-subpackage-chat-api-openapi.yml
  format: yaml
  label: Synthflow subpackage_chat API
  slug: synthflow-subpackage-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-subpackage-chat-api-openapi.yml
- filename: synthflow-subpackage-contacts-api-openapi.yml
  format: yaml
  label: Synthflow subpackage_contacts API
  slug: synthflow-subpackage-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-subpackage-contacts-api-openapi.yml
- filename: synthflow-subpackage-mcp-api-openapi.yml
  format: yaml
  label: Synthflow subpackage_mcp API
  slug: synthflow-subpackage-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-subpackage-mcp-api-openapi.yml
- filename: synthflow-subpackage-memorystores-api-openapi.yml
  format: yaml
  label: Synthflow subpackage_memoryStores API
  slug: synthflow-subpackage-memorystores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-subpackage-memorystores-api-openapi.yml
- filename: synthflow-subpackage-phonenumbers-api-openapi.yml
  format: yaml
  label: Synthflow subpackage_phoneNumbers API
  slug: synthflow-subpackage-phonenumbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-subpackage-phonenumbers-api-openapi.yml
- filename: synthflow-subpackage-webhooklogs-api-openapi.yml
  format: yaml
  label: Synthflow subpackage_webhookLogs API
  slug: synthflow-subpackage-webhooklogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-subpackage-webhooklogs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: synthflow.ai
  spf: true
hosts:
- cert_expires: Oct  1 01:03:42 2026 GMT
  host: synthflow.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 17:14:08 2026 GMT
  host: docs.synthflow.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 22:23:27 2026 GMT
  host: api.synthflow.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synthflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthflow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synthflow
provider_slug: synthflow
slug: synthflow-domain-security
source_filename: synthflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synthflow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:03:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.synthflow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 17:14:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.synthflow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:23:27 2026 GMT\n  hsts: null\ndomains:\n- domain: synthflow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/security/synthflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice
- Voice Agents
- No-Code
- Telephony
- Phone
- Outbound
- Inbound
- CRM
- Webhooks
- Custom Actions
- HIPAA
- SOC 2
- MCP
- Agent Skills
- Conversational AI
- SIP
- Simulations
- Knowledge Base
---
