---
api_specs:
- filename: fireflies-ai-apps-api-openapi.yml
  format: yaml
  label: Fireflies.ai AI Apps API
  slug: fireflies-ai-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-ai-apps-api-openapi.yml
- filename: fireflies-audio-upload-api-openapi.yml
  format: yaml
  label: Fireflies.ai Audio Upload API
  slug: fireflies-audio-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-audio-upload-api-openapi.yml
- filename: fireflies-bites-api-openapi.yml
  format: yaml
  label: Fireflies.ai Bites API
  slug: fireflies-bites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-bites-api-openapi.yml
- filename: fireflies-live-meetings-api-openapi.yml
  format: yaml
  label: Fireflies.ai Live Meetings API
  slug: fireflies-live-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-live-meetings-api-openapi.yml
- filename: fireflies-transcripts-api-openapi.yml
  format: yaml
  label: Fireflies.ai Transcripts API
  slug: fireflies-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-transcripts-api-openapi.yml
- filename: fireflies-users-api-openapi.yml
  format: yaml
  label: Fireflies.ai Users API
  slug: fireflies-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-users-api-openapi.yml
certifications:
- SOC 2 Type II
- HIPAA
- GDPR
description: ''
kind: trust-center
layout: security
name: Fireflies Trust Center
name_suffix: Trust Center
overview: Fireflies.ai maintains a public trust center documenting SOC 2 Type II, HIPAA, and GDPR compliance.
provider_name: Fireflies.ai
provider_slug: fireflies
slug: fireflies-trust-center
source_filename: fireflies-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://trust.fireflies.ai/\nurl: https://trust.fireflies.ai/\nsecondary_url: https://fireflies.ai/security\ncertifications:\n- SOC 2 Type II\n- HIPAA\n- GDPR\ncertification_detail:\n- name: SOC 2 Type II\n  source: https://fireflies.ai/security\n  note: '\"Fireflies follows industry standards for data security, privacy, and confidentiality.\"'\n- name: HIPAA\n  source: https://fireflies.ai/security\n  note: 'HIPAA - BAA Compliant. Complete PHI protection with a Business Associate Agreement — Enterprise plan only.'\n- name: GDPR\n  source: https://fireflies.ai/security\n  note: Data protection and privacy standards aligned to European regulation.\npractices:\n- '256-bit AES encryption at rest for meeting notes and transcripts; TLS in transit'\n- 'OWASP alignment across development, staging and production, with peer-reviewed code'\n- '0-day data retention policy with all vendors and partners'\n- 'No customer meeting\
  \ data used for AI model training by default'\n- 'Private storage — customer-chosen data location (Enterprise)'\n- 'Custom data retention policies (Enterprise)'\n- 'Single Sign-On (SSO) and SCIM provisioning (Enterprise)'\n- 'Rules Engine for admin control over meeting access and privacy'\n- 'Super Admin role for full workspace oversight'\n- 'Uptime logging / continuous availability tracking'\n- 'OCSF-compliant audit event log via the API (Enterprise, Beta)'\ndata_governance:\n  customer_owns_data: true\n  training_on_customer_data: false\n  deletion: 'Customer can delete transcripts at any time (deleteTranscript mutation)'\n  dpa: https://fireflies.ai/dpa\nevidence:\n- source: https://trust.fireflies.ai/\n  http_status: 200\n  note: 'Dedicated trust center on its own subdomain; page title \"Fireflies Trust Center\". Content is JS-rendered, so certification detail below is read from https://fireflies.ai/security.'\n- source: https://fireflies.ai/security\n  http_status: 200\n  keywords:\
  \ [soc 2 type ii, hipaa, gdpr, baa, owasp, encryption, sso, bug bounty, trust page]\nx-evidence:\n  fetched: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/security/fireflies-trust-center.yml
summary_line: SOC 2 Type II, HIPAA, GDPR
tags:
- Artificial Intelligence
- Meeting Assistant
- Transcription
- Summary
- Action Items
- GraphQL
- Meetings
- Productivity
- Collaboration
- Conversation Intelligence
trust_url: https://trust.fireflies.ai/
---
