---
api_specs:
- filename: synthflow-default-api-openapi.yml
  format: yaml
  label: Synthflow Default API
  slug: synthflow-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-default-api-openapi.yml
- filename: synthflow-chat-api-openapi.yml
  format: yaml
  label: Synthflow Chat API
  slug: synthflow-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-chat-api-openapi.yml
- filename: synthflow-contacts-api-openapi.yml
  format: yaml
  label: Synthflow Contacts API
  slug: synthflow-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-contacts-api-openapi.yml
- filename: synthflow-mcp-api-openapi.yml
  format: yaml
  label: Synthflow MCP API
  slug: synthflow-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-mcp-api-openapi.yml
- filename: synthflow-memorystores-api-openapi.yml
  format: yaml
  label: Synthflow Memory Stores API
  slug: synthflow-memorystores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-memorystores-api-openapi.yml
- filename: synthflow-phonenumbers-api-openapi.yml
  format: yaml
  label: Synthflow Phone Numbers API
  slug: synthflow-phonenumbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-phonenumbers-api-openapi.yml
- filename: synthflow-webhooklogs-api-openapi.yml
  format: yaml
  label: Synthflow Webhook Logs API
  slug: synthflow-webhooklogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-webhooklogs-api-openapi.yml
certifications:
- ISO 27001:2022
- SOC 2
- GDPR
- HIPAA
- PCI DSS v4.0.1
description: Synthflow operates a Trust Vault at security.synthflow.ai holding compliance documents, subprocessors and control details. The vault itself renders client-side (an unauthenticated fetch returns only the title "Trust Vault"), and some documents require Login / Get Access, so the certification list below is taken from Synthflow's own documentation page, which names them explicitly.
kind: trust-center
layout: security
name: Synthflow Trust Center
name_suffix: Trust Center
overview: Synthflow maintains a public trust center documenting ISO 27001:2022, SOC 2, GDPR, HIPAA, and PCI DSS v4.0.1 compliance.
provider_name: Synthflow
provider_slug: synthflow
slug: synthflow-trust-center
source_filename: synthflow-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://security.synthflow.ai/\nname: Synthflow Trust Vault\ndescription: >-\n  Synthflow operates a Trust Vault at security.synthflow.ai holding compliance documents,\n  subprocessors and control details. The vault itself renders client-side (an\n  unauthenticated fetch returns only the title \"Trust Vault\"), and some documents require\n  Login / Get Access, so the certification list below is taken from Synthflow's own\n  documentation page, which names them explicitly.\ncertifications:\n  - ISO 27001:2022\n  - SOC 2\n  - GDPR\n  - HIPAA\n  - PCI DSS v4.0.1\naccess:\n  public_landing: true\n  documents_gated: true\n  gate: 'Login / Get Access on the vault for private documents'\n  subprocessors_published: true\nrelated:\n  baa: https://docs.synthflow.ai/baa\n  baa_note: 'Business Associate Agreement available for HIPAA customers.'\n  agent_level_controls: https://docs.synthflow.ai/security-and-compliance\n  ai_transparency:\
  \ https://docs.synthflow.ai/ai-transparency\n  gdpr: https://synthflow.ai/gdpr\nenterprise_controls:\n  sso:\n    available: true\n    plan: Enterprise\n    provider: WorkOS\n    protocols: [SAML]\n    identity_providers: [Okta, Entra ID, Google SAML, Auth0]\n  two_factor:\n    available: true\n    type: TOTP\n    workspace_enforcement: true\n    note: 'Where a workspace mandates 2FA, a user must enable it before creating or viewing API keys.'\n  allowed_email_domains: true\n  msa_dpa: 'MSA/DPA support and data-handling review are scoped in enterprise contracts.'\ndata_protection:\n  pii_redaction: true\n  pii_redaction_api_field: redact_pii\n  redacted_types: ['credit card numbers, expiry and CVV', 'social security numbers', 'names', 'email addresses', 'phone numbers', 'physical addresses']\n  retention_control: 'Optional 30-day auto-delete of transcripts, recordings and caller IDs.'\n  regional_residency: ['Global', 'United States', 'European Union']\n  residency_note: >-\n    Region\
  \ is enforced at the API and MCP host level. WhatsApp and SMS chat channels are\n    US-only because Twilio does not offer EU data residency for those Conversations APIs.\nevidence:\n  - {source: 'https://docs.synthflow.ai/security', kind: docs, detail: 'Names ISO 27001:2022, SOC 2, GDPR, HIPAA and PCI DSS V4.0.1 and links the Trust Vault.'}\n  - {source: 'https://security.synthflow.ai/', kind: trust-center, http_status: 200, detail: 'Client-rendered Trust Vault; body served to an anonymous fetch contains only the page title.'}\n  - {source: 'https://synthflow.ai/pricing', kind: marketing, detail: 'Footer links Security; enterprise security review named in contract scope.'}\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n    - {url: 'https://security.synthflow.ai/', status: 200}\n    - {url: 'https://docs.synthflow.ai/security.md', status: 200}\n    - {url: 'https://docs.synthflow.ai/security-and-compliance.md', status: 200}\nnote: >-\n  The mechanical probe (0-working/probe-security-programs.py)\
  \ recorded trust=none because\n  the Trust Vault is a single-page app and its keyword check found no compliance terms in\n  the served HTML. This file is written from the provider's own documentation instead,\n  which states the certifications in plain text.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/security/synthflow-trust-center.yml
summary_line: ISO 27001:2022, SOC 2, GDPR, HIPAA, PCI DSS v4.0.1
tags:
- Voice
- Voice Agents
- No-Code
- Telephony
- Phone
- Outbound
- Inbound
- CRM
- Webhook
- Custom Actions
- HIPAA
- SOC 2
- MCP
- Agent Skills
- Conversational AI
- SIP
- Simulations
- Knowledge Base
trust_url: https://security.synthflow.ai/
---
