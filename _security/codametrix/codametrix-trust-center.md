---
api_specs:
- filename: codametrix-components-api-openapi.yml
  format: yaml
  label: CodaMetrix Components API
  slug: codametrix-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-components-api-openapi.yml
- filename: codametrix-incidents-api-openapi.yml
  format: yaml
  label: CodaMetrix Incidents API
  slug: codametrix-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-incidents-api-openapi.yml
- filename: codametrix-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: CodaMetrix Scheduled Maintenances API
  slug: codametrix-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-scheduled-maintenances-api-openapi.yml
- filename: codametrix-status-api-openapi.yml
  format: yaml
  label: CodaMetrix Status API
  slug: codametrix-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-status-api-openapi.yml
- filename: codametrix-summary-api-openapi.yml
  format: yaml
  label: CodaMetrix Summary API
  slug: codametrix-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-summary-api-openapi.yml
certifications:
- SOC 2
- SOC 2 Type 2
- ISO 27001
- HIPAA
description: ''
kind: trust-center
layout: security
name: Codametrix Trust Center
name_suffix: Trust Center
overview: CodaMetrix maintains a public trust center documenting SOC 2, SOC 2 Type 2, ISO 27001, and HIPAA compliance.
provider_name: CodaMetrix
provider_slug: codametrix
slug: codametrix-trust-center
source_filename: codametrix-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nurl: https://trust.codametrix.com/\nplatform: Vanta Trust Center\nsummary: >-\n  CodaMetrix operates a Vanta-hosted Trust Center on its own subdomain. The page is a client-rendered\n  single-page app; its document/control data is served over a signed GraphQL request\n  (POST https://trust.codametrix.com/graphql returns 400 \"Missing `signature` or `signedAt`\" anonymously),\n  so the certification list could not be read directly from the trust center. Certifications below are\n  recorded from the sources named in each evidence entry, with confidence stated honestly.\nstatement: >-\n  CodaMetrix delivers secure, AI-powered autonomous medical coding through its flagship CMX CARE platform,\n  grounded in trust and compliance. By prioritizing transparency and implementing rigorous data protection\n  protocols, CMX CARE ensures the utmost care in safeguarding our customer and patient data.\ncertifications:\n- name: SOC 2\n\
  \  auditor: A-LIGN\n  confidence: high\n  evidence: >-\n    SOC 2 and A-LIGN compliance badges rendered in the footer of every www.codametrix.com page\n    (Coda-Compliance-SOC.png, A-Lign.png)\n- name: SOC 2 Type 2\n  confidence: medium\n  evidence: >-\n    Stated in the CodaMetrix CMX CARE Platform vendor listing on AVIA Marketplace\n    (https://marketplace.aviahealth.com/product/79390) — third-party listing, not read from\n    CodaMetrix's own trust center\n- name: ISO 27001\n  confidence: medium\n  evidence: >-\n    Stated in the CodaMetrix CMX CARE Platform vendor listing on AVIA Marketplace\n    (https://marketplace.aviahealth.com/product/79390) — third-party listing, not read from\n    CodaMetrix's own trust center\n- name: HIPAA\n  confidence: medium\n  evidence: >-\n    Stated in the CodaMetrix CMX CARE Platform vendor listing on AVIA Marketplace; consistent with the\n    company's business model (PHI-bearing clinical documentation processed for US health systems)\ninfrastructure:\n\
  - name: AWS\n  evidence: >-\n    AWS compliance badge in the www.codametrix.com footer (Coda-Compliance-AWS.png); CodaMetrix\n    announced joining the AWS Partner Network\n    (https://www.codametrix.com/resources/codametrix-joins-the-aws-partner-network)\ngaps:\n- No /.well-known/security.txt on codametrix.com\n- No published vulnerability disclosure or bug bounty program found\n- No terms of service page found on the public site (privacy policy is published as a PDF)\n- Trust center document/report list is gated behind a signed request; no anonymous machine-readable feed\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - {url: 'https://trust.codametrix.com/', http_status: 200, content_type: text/html}\n  - {url: 'https://trust.codametrix.com/graphql', http_status: 400, note: signed request required}\n  - {url: 'https://www.codametrix.com/our-solution', http_status: 200, note: footer compliance badges}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/security/codametrix-trust-center.yml
summary_line: SOC 2, SOC 2 Type 2, ISO 27001, HIPAA
tags:
- Company
- healthcare
- health-systems
- medical-coding
- autonomous-coding
- revenue-cycle-management
- clinical-documentation
- healthcare-ai
- machine-learning
- natural-language-processing
- ehr-integration
- status
trust_url: https://trust.codametrix.com/
---
