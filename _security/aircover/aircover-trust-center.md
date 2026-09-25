---
api_specs:
- filename: aircover-openapi.yml
  format: yaml
  label: Aircover Public Agent API
  slug: aircover-public-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aircover/refs/heads/main/openapi/aircover-openapi.yml
certification_count: 2
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Aircover Trust Center
name_suffix: Trust Center
overview: Aircover maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: Aircover
provider_slug: aircover
slug: aircover-trust-center
source_filename: aircover-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://www.aircover.ai/trust-center\nfetched: '2026-09-19'\nhttp_status: 200\nportal: false\nurl: https://www.aircover.ai/trust-center\nsummary: >-\n  A first-party trust page on the marketing site, not a trust portal — there is no Vanta/Drata/SafeBase\n  instance, no document request flow and no downloadable report. It names two compliance programs and four\n  security practices in prose, and it is the only place SOC 2 is asserted outside llms.txt.\ncertifications:\n- name: SOC 2 Type II\n  claimed: true\n  evidence: 'Trust center: \"Aircover is SOC 2 Type 2 certified, ensuring your data''s security and privacy with rigorous audits.\"'\n  report_available: false\n  auditor: not named\n- name: GDPR\n  claimed: true\n  evidence: 'Trust center: \"Aircover complies with GDPR, safeguarding your privacy with utmost care and transparency in handling personal information.\" Privacy policy adds SCCs, a Transfer Impact Assessment and\
  \ a DPA on request.'\n  report_available: false\npractices:\n- encryption: All data, authentication and tokens encrypted in transit and at rest.\n- single_sign_on: SSO authentication supported (Google, Microsoft, per-organization OIDC).\n- data_isolation: 'Data remains private and individually segmented by customer; \"Customer data is not sold or used to train third-party AI models.\"'\n- no_recording: Real-time transcription without audio or video recording by default, for regions and accounts where recorded sales calls are prohibited.\n- ai_governance: Internal AI committee; the page claims approval by AI committees at Fortune 500 companies.\ngaps:\n- The linked compliance sub-page https://www.aircover.ai/trust-center/compliance (named in llms.txt) returns 404.\n- No security.txt, no vulnerability disclosure policy and no bug bounty on any host (probed 2026-09-19).\n- No published SOC 2 report, auditor letter, penetration-test summary or subprocessor list (the subprocessor list is available\
  \ only on request).\n- No status page and no incident-history page.\nrelated:\n  conformance: conformance/aircover-conformance.yml\n  regulatory: regulatory/aircover-regulatory-posture.yml\n  domain_security: security/aircover-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircover/refs/heads/main/security/aircover-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Sales Enablement
- Conversation Intelligence
- Sales Coaching
- Revenue Intelligence
- AI Agents
- MCP
- Agent-Native
- CRM
- Meetings
- Transcription
- Authentication
trust_url: https://www.aircover.ai/trust-center
---
