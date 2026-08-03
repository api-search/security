---
api_specs:
- filename: conversica-integrations-api-openapi.yml
  format: yaml
  label: Conversica Integrations API
  slug: integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conversica/refs/heads/main/openapi/conversica-integrations-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Conversica Trust Center
name_suffix: Trust Center
overview: Conversica maintains a public trust center documenting SOC 2 Type II, ISO 27001, and GDPR compliance.
provider_name: Conversica
provider_slug: conversica
slug: conversica-trust-center
source_filename: conversica-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nurl: https://trust.conversica.com/\nplatform: Vanta Trust Center\nplatform_evidence: >-\n  trust.conversica.com resolves via 65a0f6a2b4c7501f8979a89a.cname.vantatrust.com and the\n  page is served as a Vanta trust-report single-page application (assets.vanta.com bundle,\n  slug id 4frf8fa1b2ky3zeyxrzfp).\nsections:\n- url: https://trust.conversica.com/\n  name: Overview\n  http_status: 200\n- url: https://trust.conversica.com/controls\n  name: Controls\n  http_status: 200\n- url: https://trust.conversica.com/resources\n  name: Resources\n  http_status: 200\ncertifications:\n- name: SOC 2 Type II\n  confidence: high\n  evidence: >-\n    Conversica announced completion of a SOC 2 Type II audit performed by A-lign, covering\n    the Trust Services Principles and Criteria for Security, and continues to reference SOC\n    2 on its website.\n  sources:\n  - https://www.globenewswire.com/news-release/2021/01/26/2164248/0/en/Conversica-Announces-SOC-2-Type-II-Certification.html\n\
  \  - https://www.conversica.com/\n- name: ISO 27001\n  confidence: medium\n  evidence: >-\n    An ISO 27001 certificate is listed among the documents on the Conversica trust centre\n    resources page. The document itself sits behind the Vanta access-request gate and was\n    not retrieved, so this is recorded as reported rather than inspected.\n  sources:\n  - https://trust.conversica.com/resources\n- name: GDPR\n  confidence: medium\n  kind: regulatory-program\n  evidence: Conversica's website states enterprise security compliance including GDPR alongside SOC 2.\n  sources:\n  - https://www.conversica.com/\ngated:\n  documents_require_request: true\n  note: >-\n    Vanta trust centres put certificate PDFs and security reports behind an access request\n    (often NDA-gated). The public shell lists what exists; the artefacts themselves were not\n    downloadable anonymously, and the Vanta GraphQL API rejects unsigned requests, so the\n    certification list above is what could be evidenced\
  \ publicly - it is not asserted to be\n    complete.\nrelated:\n  privacy_policy: https://www.conversica.com/legal-info/privacy-policy\n  prohibited_use_policy: https://www.conversica.com/legal-info/prohibited-use-policy\n  responsible_disclosure: https://www.conversica.com/legal-info/responsible-disclosure-policy\n  california_notice: https://www.conversica.com/legal-info/notice-at-collection-of-personal-information-and-privacy-policy-for-california-personnel\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - url: https://trust.conversica.com/\n    http_status: 200\n    content_type: text/html\n  - url: https://trust.conversica.com/controls\n    http_status: 200\n  - url: https://trust.conversica.com/resources\n    http_status: 200\n  - url: https://api.vanta.com/v1/trust-pages/4frf8fa1b2ky3zeyxrzfp\n    http_status: 401\n    note: Vanta public API rejects anonymous reads; trust report GraphQL requires a signed request\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conversica/refs/heads/main/security/conversica-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, GDPR
tags:
- Company
- Artificial Intelligence
- Conversational AI
- AI Agents
- Sales
- Marketing
- Lead Management
- CRM
- Marketing Automation
- Customer Engagement
- Messaging
- SMS
- Email
- Chat
- Automotive
- Higher Education
- Webhooks
trust_url: https://trust.conversica.com/
---
