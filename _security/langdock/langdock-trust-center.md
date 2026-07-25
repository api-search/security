---
api_specs:
- filename: langdock-agent-api-openapi.yml
  format: yaml
  label: Langdock Agent API
  slug: langdock-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-agent-api-openapi.yml
- filename: langdock-agent-build-api-openapi.yml
  format: yaml
  label: Langdock Agent Build API
  slug: langdock-agent-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-agent-build-api-openapi.yml
- filename: langdock-assistant-api-openapi.yml
  format: yaml
  label: Langdock Assistant API
  slug: langdock-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-assistant-api-openapi.yml
- filename: langdock-assistant-build-api-openapi.yml
  format: yaml
  label: Langdock Assistant Build API
  slug: langdock-assistant-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-assistant-build-api-openapi.yml
- filename: langdock-attachments-api-openapi.yml
  format: yaml
  label: Langdock Attachments API
  slug: langdock-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-attachments-api-openapi.yml
- filename: langdock-audit-logs-api-openapi.yml
  format: yaml
  label: Langdock Audit Logs API
  slug: langdock-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-audit-logs-api-openapi.yml
- filename: langdock-chat-api-openapi.yml
  format: yaml
  label: Langdock Chat API
  slug: langdock-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-chat-api-openapi.yml
- filename: langdock-embeddings-api-openapi.yml
  format: yaml
  label: Langdock Embeddings API
  slug: langdock-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-embeddings-api-openapi.yml
- filename: langdock-fim-api-openapi.yml
  format: yaml
  label: Langdock fim API
  slug: langdock-fim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-fim-api-openapi.yml
- filename: langdock-google-api-openapi.yml
  format: yaml
  label: Langdock Google API
  slug: langdock-google-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-google-api-openapi.yml
- filename: langdock-knowledge-api-openapi.yml
  format: yaml
  label: Langdock Knowledge API
  slug: langdock-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-knowledge-api-openapi.yml
- filename: langdock-messages-api-openapi.yml
  format: yaml
  label: Langdock Messages API
  slug: langdock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-messages-api-openapi.yml
- filename: langdock-skills-api-openapi.yml
  format: yaml
  label: Langdock Skills API
  slug: langdock-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-skills-api-openapi.yml
- filename: langdock-usage-export-api-openapi.yml
  format: yaml
  label: Langdock Usage Export API
  slug: langdock-usage-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-usage-export-api-openapi.yml
- filename: langdock-user-management-api-openapi.yml
  format: yaml
  label: Langdock User Management API
  slug: langdock-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-user-management-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
- GDPR
description: Langdock publishes a dedicated trust center at trust.langdock.com plus a security overview page at langdock.com/security covering certifications, deployment and data-residency options, subprocessor management, and penetration testing.
kind: trust-center
layout: security
name: Langdock Trust Center
name_suffix: Trust Center
overview: Langdock maintains a public trust center documenting SOC 2 Type II, ISO 27001, and GDPR compliance.
provider_name: Langdock
provider_slug: langdock
slug: langdock-trust-center
source_filename: langdock-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.langdock.com/security\nurl: https://trust.langdock.com/\ndescription: >-\n  Langdock publishes a dedicated trust center at trust.langdock.com plus a security\n  overview page at langdock.com/security covering certifications, deployment and\n  data-residency options, subprocessor management, and penetration testing.\npages:\n- url: https://trust.langdock.com/\n  label: Trust center\n  status: 200\n- url: https://www.langdock.com/security\n  label: Security overview\n  status: 200\ncertifications:\n- SOC 2 Type II\n- ISO 27001\n- GDPR\ncertification_detail:\n- name: ISO 27001\n  claim: Certified to the global standard for information management.\n- name: SOC 2 Type II\n  claim: Independently audited to ensure secure, reliable data handling.\n- name: GDPR\n  claim: Fully aligned with GDPR for strong data privacy and user protection.\nhosting:\n  cloud: Microsoft Azure\n  data_residency: EU — the application\
  \ and most models (configurable) are hosted entirely\n    in the EU.\ndeployment_options:\n- name: Multi-tenant SaaS\n  detail: Hosted via Microsoft Azure on EU servers.\n- name: Single-tenant SaaS\n  detail: Dedicated deployment managed by Langdock (Enterprise, 2,000+ seats).\n- name: Bring your own cloud\n  detail: Customer cloud deployment (Enterprise, 5,000+ seats).\n- name: On-premise\n  detail: Custom Kubernetes via Helm charts (Enterprise, 5,000+ seats).\npenetration_testing: Frequent independent third-party penetration testing.\nsubprocessors:\n  published: true\n  detail: >-\n    Langdock regularly reviews subprocessors and maintains a published list; all\n    subprocessors must adhere to equivalent security standards.\nevidence:\n- source: https://www.langdock.com/security\n  keywords:\n  - soc 2\n  - iso 27001\n  - gdpr\n  - trust center\n  - penetration testing\nrelated:\n  vulnerability_disclosure: security/langdock-vulnerability-disclosure.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/security/langdock-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, GDPR
tags:
- Company
- Artificial Intelligence
- Enterprise AI
- LLM
- Agents
- Model Context Protocol
- Workflows
- Knowledge Management
- Germany
- Europe
trust_url: https://trust.langdock.com/
---
