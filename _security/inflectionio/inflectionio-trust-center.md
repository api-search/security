---
api_specs:
- filename: inflectionio-contact-activity-api-openapi.yml
  format: yaml
  label: Inflection.io Contact Activity API
  slug: inflectionio-contact-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-contact-activity-api-openapi.yml
- filename: inflectionio-contacts-api-openapi.yml
  format: yaml
  label: Inflection.io Contacts API
  slug: inflectionio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-contacts-api-openapi.yml
- filename: inflectionio-emails-api-openapi.yml
  format: yaml
  label: Inflection.io Emails API
  slug: inflectionio-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-emails-api-openapi.yml
- filename: inflectionio-email-versions-api-openapi.yml
  format: yaml
  label: Inflection.io Email Versions API
  slug: inflectionio-email-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-email-versions-api-openapi.yml
- filename: inflectionio-lists-and-members-api-openapi.yml
  format: yaml
  label: Inflection.io Lists and Members API
  slug: inflectionio-lists-and-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-lists-and-members-api-openapi.yml
certifications:
- SOC 2
- GDPR
- CCPA
- Penetration test
description: ''
kind: trust-center
layout: security
name: Inflectionio Trust Center
name_suffix: Trust Center
overview: Inflection.io maintains a public trust center documenting SOC 2, GDPR, CCPA, and Penetration test compliance.
provider_name: Inflection.io
provider_slug: inflectionio
slug: inflectionio-trust-center
source_filename: inflectionio-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://docs.inflection.io/agents/mcp-trust-security\nsource: https://docs.inflection.io/agents/mcp-trust-security\nsummary: >-\n  Inflection has no trust-center subdomain — trust.inflection.io does not resolve and\n  www.inflection.io/security is a 404. What it does publish is a scoped, unusually specific\n  Trust & Security page inside the developer docs, covering the MCP service: deployment model,\n  encryption, OAuth 2.1 posture, tenant isolation, data retention, named subprocessors, a reasoned\n  CORS justification, and a compliance section with named certifications. It is a real published\n  compliance posture, but it is written about the MCP endpoint rather than the platform as a whole,\n  and every artifact behind it (SOC 2 report, pen-test summary, DPA) is NDA/request-gated.\ncertifications:\n- name: SOC 2\n  type: Type II\n  status: attested\n  year: 2026\n  evidence_availability: report available under\
  \ NDA on request from support@inflection.io\n- name: GDPR\n  status: DPA available on request\n  evidence_availability: Data Processing Addendum on request from support@inflection.io\n- name: CCPA\n  status: compliant\n  evidence_availability: data subject rights honored per the published Privacy Policy\n- name: Penetration test\n  status: independent third-party test conducted 2026\n  evidence_availability: summary available under NDA on request\nout_of_scope:\n- {name: PCI DSS, note: Not in scope — Inflection does not process payment card data.}\n- {name: HIPAA, note: Not in scope — Inflection does not process protected health information.}\nposture:\n  deployment: multi-tenant SaaS, single global region\n  cloud: Amazon Web Services, US region\n  encryption_in_transit: TLS 1.2 minimum, HSTS enabled\n  encryption_at_rest: AES-256 via AWS KMS\n  authentication: OAuth 2.1 with PKCE, S256 only (plain rejected)\n  token_lifetime: 15-minute access tokens; refresh-token rotation with reuse\
  \ detection\n  per_call_verification: every MCP tool call re-verifies the bearer token with the authorization server\n  tenant_isolation: every MCP tool call scoped to the caller's tenant id; cross-tenant reads not possible\n  token_handling: verified tokens cached in memory for their lifetime; raw tokens not logged or persisted\n  cors: wildcard Access-Control-Allow-Origin with Access-Control-Allow-Credentials false, documented and justified\nretention:\n  assets_days: 30\n  agent_outputs_days: 7\n  intermediate_results_hours: 24\n  tracing: LangSmith traces include user_email, tenant_id, session_id and user-agent; retention follows LangSmith defaults\nsubprocessors:\n- {name: Amazon Web Services, purpose: infrastructure (compute, storage, network, managed database), data: all tenant data at rest and in transit}\n- {name: OpenAI, purpose: LLM inference for AI agents, data: prompts and conversation context}\n- {name: LangSmith, purpose: agent trace observability, data: user email, tenant\
  \ id, prompts, tool calls}\ndata_subject_rights:\n  url: https://docs.inflection.io/settings/data-subject-erasure-requests\n  note: Self-serve Data Subject Erasure Requests (DSRs) for GDPR/CCPA deletion requests.\nprivacy_policy: https://www.inflection.io/legal/privacy-policy\nterms: https://www.inflection.io/legal/terms\nevidence:\n- source: https://docs.inflection.io/agents/mcp-trust-security\n  http_status: 200\n  keywords: [soc 2 type ii, gdpr, ccpa, penetration test, encryption, tenant isolation, subprocessors]\n- {source: 'https://trust.inflection.io', http_status: 0, note: does not resolve}\n- {source: 'https://www.inflection.io/security', http_status: 404}\npage_changelog:\n- {date: '2026-06-02', change: Initial publication.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/security/inflectionio-trust-center.yml
summary_line: SOC 2, GDPR, CCPA, Penetration test
tags:
- Company
- Saas
- Marketing
- Marketing Automation
- Email Marketing
- Customer Data
- B2B
- Contacts
- MCP
- Agents
- Artificial Intelligence
- Customer Journeys
- Webhook
trust_url: https://docs.inflection.io/agents/mcp-trust-security
---
