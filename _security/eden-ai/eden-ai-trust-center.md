---
api_specs:
- filename: eden-ai-audio-features-openapi.json
  format: json
  label: Eden AI Audio API
  slug: eden-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-audio-features-openapi.json
- filename: eden-ai-image-features-openapi.json
  format: json
  label: Eden AI Image API
  slug: eden-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-image-features-openapi.json
- filename: eden-ai-ocr-features-openapi.json
  format: json
  label: Eden AI OCR API
  slug: eden-ai-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-ocr-features-openapi.json
- filename: eden-ai-text-features-openapi.json
  format: json
  label: Eden AI Text API
  slug: eden-ai-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-text-features-openapi.json
- filename: eden-ai-translation-features-openapi.json
  format: json
  label: Eden AI Translation API
  slug: eden-ai-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-translation-features-openapi.json
- filename: eden-ai-v3-openapi.json
  format: json
  label: Eden AI API V3
  slug: eden-ai-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-v3-openapi.json
- filename: eden-ai-video-features-openapi.json
  format: json
  label: Eden AI Video API
  slug: eden-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-video-features-openapi.json
- filename: eden-ai-llm-features-openapi.json
  format: json
  label: Eden AI LLM API (v2)
  slug: eden-ai-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-llm-features-openapi.json
- filename: eden-ai-multimodal-features-openapi.json
  format: json
  label: Eden AI Multimodal API
  slug: eden-ai-multimodal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-multimodal-features-openapi.json
- filename: eden-ai-user-management-openapi.json
  format: json
  label: Eden AI User Management API
  slug: eden-ai-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-user-management-openapi.json
- filename: eden-ai-cost-monitoring-openapi.json
  format: json
  label: Eden AI Cost Monitoring API
  slug: eden-ai-cost-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-cost-monitoring-openapi.json
- filename: eden-ai-organization-management-openapi.json
  format: json
  label: Eden AI Organization Management API
  slug: eden-ai-organization-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-organization-management-openapi.json
certification_count: 3
certifications:
- GDPR
- ISO/IEC 27001:2022
- SOC 2 Type 2
description: Eden AI runs a public trust center at trust.edenai.co carrying 3 documents, 248 controls and a 6-entry FAQ, grouped as Business Operations, Cloud Security, Human Resources and Data.
kind: trust-center
layout: security
name: Eden Ai Trust Center
name_suffix: Trust Center
overview: Eden AI maintains a public trust center documenting GDPR, ISO/IEC 27001:2022, and SOC 2 Type 2 compliance.
provider_name: Eden AI
provider_slug: eden-ai
slug: eden-ai-trust-center
source_filename: eden-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nprobe: true\nsource: https://trust.edenai.co/\nurl: https://trust.edenai.co/\nhttp_status: 200\nplatform: Bastion\ndescription: >-\n  Eden AI runs a public trust center at trust.edenai.co carrying 3 documents, 248 controls and a\n  6-entry FAQ, grouped as Business Operations, Cloud Security, Human Resources and Data.\nposture:\n  zero_data_retention_by_default: true\n  training_on_customer_data: false\n  encryption_in_transit: TLS 1.2 minimum\n  encryption_at_rest: AES-256 via AWS KMS\n  hosting: AWS EU (Paris) region\n  audit_logging: continuous monitoring with tamper-evident audit logging\n  penetration_testing: independent third-party testers\n  incident_response: documented process\ncertifications:\n  - name: GDPR\n    status: supported\n    evidence: 'Listed under Compliance on https://trust.edenai.co/; DPA published at https://www.edenai.co/dpa (200)'\n  - name: 'ISO/IEC 27001:2022'\n    status: conflicting\n    evidence: >-\n\
  \      Listed under Compliance on https://trust.edenai.co/, and https://www.edenai.co/security states\n      \"ISO 27001 certified\" — but the trust center's own overview says \"GDPR, SOC 2, and ISO 27001\n      audits are in progress\" (read 2026-09-06).\n  - name: SOC 2 Type 2\n    status: conflicting\n    evidence: >-\n      https://trust.edenai.co/ labels the SOC 2 Type 2 report \"(In progress)\" while\n      https://www.edenai.co/security markets \"SOC 2 certified\".\ndiscrepancy:\n  observed: '2026-09-06'\n  detail: >-\n    Eden AI's marketing security page asserts SOC 2 and ISO 27001 CERTIFICATION; its own trust\n    center says both audits are IN PROGRESS. Recorded rather than resolved — a procurement reader\n    needs to know the two first-party surfaces disagree. An earlier version of this artifact recorded\n    the certifications flat, without the in-progress qualifier.\n  sources:\n    - {url: 'https://trust.edenai.co/', status: 200}\n    - {url: 'https://www.edenai.co/security',\
  \ status: 200}\ndocuments:\n  - {name: Data Processing Agreement, url: 'https://www.edenai.co/dpa', status: 200}\n  - {name: Privacy Policy, url: 'https://www.edenai.co/privacy-policy', status: 200}\n  - {name: Terms & Conditions, url: 'https://www.edenai.co/terms-conditions', status: 200}\nevidence:\n  - source: https://trust.edenai.co/\n    keywords: [soc 2, iso 27001, gdpr, trust center, zero data retention, aes-256, aws kms, penetration testing]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/security/eden-ai-trust-center.yml
summary_line: GDPR, ISO/IEC 27001:2022, SOC 2 Type 2
tags:
- Artificial Intelligence
- AI Gateway
- LLM
- Machine Learning
- OCR
- Translation
- Speech
- Computer Vision
- Model Context Protocol
- Emotion Detection
trust_url: https://trust.edenai.co/
---
