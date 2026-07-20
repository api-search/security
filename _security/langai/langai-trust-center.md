---
api_specs:
- filename: langai-api-openapi.yml
  format: yaml
  label: Lang.ai API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/openapi/langai-api-openapi.yml
certifications:
- SOC 2 Type II
- HIPAA
- GDPR
description: ''
kind: trust-center
layout: security
name: Langai Trust Center
name_suffix: Trust Center
overview: Lang.ai maintains a public trust center documenting SOC 2 Type II, HIPAA, and GDPR compliance.
provider_name: Lang.ai
provider_slug: langai
slug: langai-trust-center
source_filename: langai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nprobe_result: >-\n  0-working/probe-security-programs.py returned trust=none because it probes the lang.ai\n  domain only. Lang.ai itself publishes no trust center; the surfaces below belong to\n  Capacity, which acquired Lang.ai, and were verified by hand.\nscope: parent-platform\nurl: https://trust.capacity.com/\nsecurity_page: https://capacity.com/security/\ncertifications:\n- SOC 2 Type II\n- HIPAA\n- GDPR\ncontrols:\n- name: Data encryption\n  detail: AES-256 encryption at rest and TLS 1.2+ for data in transit.\n- name: AI data privacy\n  detail: Customer data is never shared or used to train external models.\n- name: Role-based access control\n  detail: Controls over who has access to data.\nevidence:\n- source: https://capacity.com/security/\n  http_status: 200\n  quote: >-\n    \"Regulatory Compliance — GDPR, HIPAA, SOC 2 Type II certified.\" / \"Data Encryption —\n    AES-256 encryption at rest and TLS 1.2+ for\
  \ data in transit.\"\n- source: https://trust.capacity.com/\n  http_status: 200\n  note: >-\n    Live trust center; the page title is \"Capacity Trust Center\". Content is\n    client-rendered, so certification detail was taken from the security page above.\ncaveat: >-\n  These are Capacity's platform-level attestations following the acquisition, not a\n  Lang.ai-specific audit. No SOC 2 report or certification scope naming the Lang.ai API\n  was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/security/langai-trust-center.yml
summary_line: SOC 2 Type II, HIPAA, GDPR
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Conversation Intelligence
- Customer Support
- Text Classification
- Analytics
- Customer Experience
trust_url: https://trust.capacity.com/
---
