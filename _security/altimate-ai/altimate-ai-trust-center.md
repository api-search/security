---
api_specs:
- filename: altimate-ai-openapi-original.json
  format: json
  label: Altimate AI Platform API
  slug: altimate-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altimate-ai/refs/heads/main/openapi/altimate-ai-openapi-original.json
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Altimate Ai Trust Center
name_suffix: Trust Center
overview: Altimate AI maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Altimate AI
provider_slug: altimate-ai
slug: altimate-ai-trust-center
source_filename: altimate-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://help.altimate.ai/datamates/faq/security/\n# Compliance posture documented in Altimate's Security & Compliance FAQ. No dedicated\n# trust.altimate.ai portal was found (probe-security-programs found none), but the FAQ\n# publishes a named certification and concrete controls.\ncertifications:\n  - SOC 2 Type II\ncompliance:\n  - GDPR\nposture:\n  soc2: Audited annually for security, availability, and confidentiality controls.\n  gdpr: >-\n    No customer data is stored (metadata-only); DPAs available on request; deletion\n    requests do not need to be propagated to Altimate.\n  infrastructure: AWS private VPC, network isolation, IAM access controls, AWS SSO + MFA for production access.\n  data_handling: >-\n    Customer credentials encrypted locally in IDE secure storage and never transmitted;\n    BYOK sends data directly to the customer's chosen LLM provider; Altimate LLM Gateway\n    retains only anonymized metadata;\
  \ no customer code/SQL/PII retained; no data used for training.\nevidence:\n  - source: https://help.altimate.ai/datamates/faq/security/\n    keywords: [soc 2 type ii, gdpr, byok, private vpc, aws sso, mfa]\ncontact: https://www.altimate.ai/support\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altimate-ai/refs/heads/main/security/altimate-ai-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Data
- Data Engineering
- Artificial Intelligence
- Agents
- MCP
- dbt
- Data Governance
- Data Contracts
- Analytics Engineering
trust_url: ''
---
