---
api_specs:
- filename: langdock-openapi-original.yml
  format: yaml
  label: Langdock API
  slug: langdock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-openapi-original.yml
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
