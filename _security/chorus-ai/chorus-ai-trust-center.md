---
api_specs:
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus Engagements API
  slug: chorus-engagements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus Recordings & Transcripts API
  slug: chorus-recordings-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus CRM Sync API
  slug: chorus-crm-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
certifications:
- source
- source_status
- verified
- quote
- held
- frameworks
- explicitly_not_held
description: ''
kind: trust-center
layout: security
name: Chorus Ai Trust Center
name_suffix: Trust Center
overview: Chorus.ai maintains a public trust center documenting source, source_status, verified, quote, held, frameworks, and explicitly_not_held compliance.
provider_name: Chorus.ai
provider_slug: chorus-ai
slug: chorus-ai-trust-center
source_filename: chorus-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://trust.zoominfo.com/ + https://www.zoominfo.com/legal/security-overview\nscope_note: >-\n  Chorus.ai operates no trust center of its own — trust.chorus.ai does not resolve. Chorus.ai was\n  acquired by ZoomInfo in 2021 and ships as \"Chorus by ZoomInfo\", so ZoomInfo's trust center is\n  the governing one for the Chorus service. Recorded at the parent level and labelled as such.\ntrust_center:\n  published: true\n  holder: ZoomInfo\n  url: https://trust.zoominfo.com/\n  status: 200\n  platform: Vanta\n  platform_evidence: >-\n    The page is a Vanta-hosted trust center (assets.vanta.com asset host, data-slugid\n    m6iv02iadx6n4t1sbxpk6z, canonical https://trust.zoominfo.com).\n  machine_readable: false\n  machine_readable_note: >-\n    The trust center is a client-rendered single-page app. Its HTML shell is 5.9 KB and contains\n    no certification content, and every path under the host (including /api/*, /graphql and\n\
  \    invented paths) answers HTTP 200 with the same shell — a catch-all. Certifications therefore\n    could NOT be read from the trust center itself; they were taken instead from ZoomInfo's own\n    security page, which serves them as real text.\ncertifications:\n  source: https://www.zoominfo.com/legal/security-overview\n  source_status: 200\n  verified: '2026-08-13'\n  quote: 'ZoomInfo is ISO 27001, ISO 27701, TRUSTe, and SOC 2 Type II certified.'\n  held:\n  - name: SOC 2 Type II\n    body: AICPA\n    scope: security, availability and confidentiality controls around ZoomInfo services\n  - name: ISO/IEC 27001\n    scope: Information Security Management System (ISMS)\n  - name: ISO/IEC 27701\n    scope: Privacy Information Management System\n  - name: TRUSTe\n    scope: enterprise privacy certification\n  frameworks:\n  - name: ISO 31000\n    scope: >-\n      Risk Management Framework the ISMS risk-management program is formally based on. A\n      framework, not a certification.\n  explicitly_not_held:\n\
  \    note: >-\n      ZoomInfo's security page names the following only as certifications it may REQUIRE OF ITS\n      SERVICE PROVIDERS during third-party risk review: \"we carefully review our service\n      providers' security practices, requiring appropriate certifications which may include SOC 2\n      Type II, ISO 27001, PCI DSS, HIPAA, and CSA-STAR\". PCI DSS, HIPAA and CSA-STAR are\n      therefore NOT ZoomInfo or Chorus certifications and are recorded here only to prevent a\n      keyword match from crediting them.\n    items:\n    - PCI DSS\n    - HIPAA\n    - CSA-STAR\nprivacy:\n  policy: https://www.zoominfo.com/legal/privacy-policy\n  status: 200\n  positioning: >-\n    ZoomInfo positions itself as a \"privacy-first company\" dealing exclusively in non-sensitive\n    business-context data.\nsecurity_contact: security@zoominfo.com\nprobed: '2026-08-13'\ncross_links:\n  vulnerability_disclosure: security/chorus-ai-vulnerability-disclosure.yml\n  conformance: conformance/chorus-ai-conformance.yml\n\
  \  domain_security: security/chorus-ai-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/security/chorus-ai-trust-center.yml
summary_line: source, source_status, verified, quote, held, frameworks, explicitly_not_held
tags:
- Sales
- Revenue Intelligence
- Conversation
- Analytics
- ZoomInfo
- Conversation Intelligence
- Sales Enablement
- Call Recording
- Transcription
- Speech Analytics
- CRM
- Coaching
trust_url: ''
---
