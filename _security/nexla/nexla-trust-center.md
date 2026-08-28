---
api_specs:
- filename: nexla-rest-api-openapi.yml
  format: yaml
  label: Nexla REST API
  slug: nexla-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/openapi/nexla-rest-api-openapi.yml
- filename: nexla-genai-mcpaas-openapi.json
  format: json
  label: Nexla GenAI API (RAG + MCPaaS)
  slug: nexla-genai-api-rag-mcpaas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/openapi/nexla-genai-mcpaas-openapi.json
certifications:
- SOC 2 Type II
- ISO 27001
- HIPAA
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Nexla Trust Center
name_suffix: Trust Center
overview: Nexla maintains a public trust center documenting SOC 2 Type II, ISO 27001, HIPAA, GDPR, and CCPA compliance.
provider_name: Nexla
provider_slug: nexla
slug: nexla-trust-center
source_filename: nexla-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://nexla.com/data-security/\ntrust_center: false\nnote: >-\n  Nexla does not operate a dedicated trust center portal — trust.nexla.com does not resolve (DNS NXDOMAIN)\n  and no Vanta/Drata/SafeBase/Conveyor portal was found. Certifications are published as prose plus footer\n  badges on the Data Security page. A prior automated probe matched https://nexla.com/connector/trustpilot/\n  — that is a Trustpilot CONNECTOR documentation page, not a Nexla trust center, and has been corrected here.\n  Because there is no trust portal, no `TrustCenter` pointer is emitted in apis.yml; the certifications are\n  wired through the `Compliance` pointer instead.\nurl: https://nexla.com/data-security/\ncertifications:\n- name: SOC 2 Type II\n  evidence: 'Nexla continues to meet the most stringent standards of security with SOC 2 Type II compliance'\n  source: https://nexla.com/data-security/\n- name: ISO 27001\n  evidence: 'ISO badge published\
  \ in the docs.nexla.com and nexla.com footer (/img/badges/ISO.svg)'\n  source: https://docs.nexla.com/\n- name: HIPAA\n  evidence: 'HIPAA compliant badge published in the docs.nexla.com footer (/img/badges/hipaa-compliant.svg)'\n  source: https://docs.nexla.com/\n- name: GDPR\n  evidence: \"Nexla is fully compliant with the European Unions' Global Data Protection Regulation\"\n  source: https://nexla.com/data-security/\n- name: CCPA\n  evidence: 'California Consumer Privacy Act (CCPA) compliance stated'\n  source: https://nexla.com/data-security/\nclaims:\n- 'Encrypt data at rest and in motion for complete end-to-end security'\n- 'Nexla makes no copies of your data as it ingests, processes, and delivers the data'\n- 'data never leaves your environment (private/hybrid cloud and on-premise deployment)'\nevidence:\n- url: https://nexla.com/data-security/\n  status: 200\n- url: https://trust.nexla.com/\n  status: 0\n  note: DNS NXDOMAIN — host does not resolve\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/security/nexla-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, HIPAA, GDPR, CCPA
tags:
- Company
- Data Integration
- Data Engineering
- ETL
- ELT
- Data Products
- Streaming
- Change Data Capture
- Data Governance
- Artificial Intelligence
- Retrieval Augmented Generation
- MCP
- Agent Tools
- Data Pipelines
- Connectors
trust_url: https://nexla.com/data-security/
---
