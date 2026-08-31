---
api_specs:
- filename: samaya-ai-organizations-api-openapi.yml
  format: yaml
  label: Samaya AI Organizations API
  slug: samaya-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-organizations-api-openapi.yml
- filename: samaya-ai-teams-api-openapi.yml
  format: yaml
  label: Samaya AI Teams API
  slug: samaya-ai-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-teams-api-openapi.yml
- filename: samaya-ai-users-api-openapi.yml
  format: yaml
  label: Samaya AI Users API
  slug: samaya-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-users-api-openapi.yml
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Samaya Ai Trust Center
name_suffix: Trust Center
overview: Samaya AI maintains a public trust center documenting SOC 2 compliance.
provider_name: Samaya AI
provider_slug: samaya-ai
slug: samaya-ai-trust-center
source_filename: samaya-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.samaya.ai/\ntrust_center:\n  url: https://trust.samaya.ai/\n  status: 200\n  vendor: Vanta\n  vendor_evidence: >-\n    The page loads assets.vanta.com/static/index-trust-report-*.js, carries\n    data-slugid=\"it86lsjv4nvr81b4qzc24m\", and its og:image is served from app.vanta.com/doc.\n  title: Samaya AI Trust Center\n  canonical: https://trust.samaya.ai\ncertifications:\n- name: SOC 2\n  claimed: true\n  verified: false\n  source: https://samaya.ai/llms.txt\n  quote: SOC 2 compliant with user-level access controls\n  note: >-\n    First-party claim published by Samaya in its own llms.txt. The report itself sits behind the\n    trust center's document-access request, so type (I vs II), scope and audit period were not\n    verified.\ncertifications_note: >-\n  The Vanta trust center renders its control and certification list client-side; a server-side fetch\n  returns only the 6.4KB React shell, so the full framework\
  \ list could not be read without executing\n  JavaScript. Recorded as unreadable rather than absent — the surface exists and is live.\nsubprocessors:\n  published: unknown\n  note: Not readable from the server-rendered shell.\ndocuments:\n  access: request\n  note: Vanta trust centers gate report downloads behind an NDA/email request flow.\nrelated:\n  privacy_policy: https://samaya.ai/privacy/privacy\n  applicant_privacy: https://samaya.ai/privacy/applicants\n  security_contact: null\n  security_contact_note: >-\n    No /.well-known/security.txt on any Samaya host (404 on samaya.ai, api.samaya.ai,\n    mcp.samaya.ai), and no dedicated security or vulnerability-disclosure page exists. The only\n    published contacts are hello@samaya.ai and feedback@samaya.ai.\nevidence:\n- url: https://trust.samaya.ai/\n  status: 200\n- url: https://samaya.ai/llms.txt\n  status: 200\n- url: https://samaya.ai/.well-known/security.txt\n  status: 404\n- url: https://api.samaya.ai/.well-known/security.txt\n\
  \  status: 404\n- url: https://mcp.samaya.ai/.well-known/security.txt\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/security/samaya-ai-trust-center.yml
summary_line: SOC 2
tags:
- Artificial Intelligence
- Financial Services
- Investment Research
- AI Agents
- MCP
- agent-native
- Capital Markets
- Enterprise Search
- Retrieval
- GraphQL
trust_url: ''
---
