---
api_specs:
- filename: kandji-endpoint-management-openapi.json
  format: json
  label: Iru Endpoint Management API
  slug: iru-endpoint-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-endpoint-management-openapi.json
- filename: kandji-upload-to-s3-openapi.json
  format: json
  label: Iru Library Item Upload API
  slug: iru-library-item-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-upload-to-s3-openapi.json
certifications:
- SOC 2 Type II
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Kandji Trust Center
name_suffix: Trust Center
overview: Iru maintains a public trust center documenting SOC 2 Type II and ISO 27001 compliance.
provider_name: Iru
provider_slug: kandji
slug: kandji-trust-center
source_filename: kandji-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nsource: https://www.iru.com/security\nurl: https://trust.iru.com/\nalternate_urls:\n- https://www.iru.com/security\n- https://trust.kandji.io/\ncertifications:\n- SOC 2 Type II\n- ISO 27001\ncompliance_artifacts:\n- {name: Data Processing Addendum, url: 'https://www.iru.com/legal/data-processing-addendum'}\n- {name: Sub-processor list, url: 'https://www.iru.com/legal/service-providers'}\n- {name: Platform Services Agreement, url: 'https://www.iru.com/legal/terms'}\n- {name: Privacy Policy, url: 'https://www.iru.com/legal/privacy'}\n- {name: Privacy Rights Request Form, url: 'https://www.iru.com/legal/privacy-rights-request'}\n- {name: Artificial Intelligence Acceptable Use Policy, url: 'https://www.iru.com/legal/ai-use-policy'}\n- {name: Accessibility Statement, url: 'https://www.iru.com/legal/accessibility'}\nsecurity_program:\n  external_pentest: minimum 2x per year, qualified third-party firm\n  vulnerability_scanning:\
  \ monthly third-party scans + daily internal scans\n  vulnerability_disclosure: security/kandji-vulnerability-disclosure.yml\nnotes: >-\n  Two trust surfaces exist and they are different things. https://www.iru.com/security is Iru's own\n  security-practices page and is where the SOC 2 Type II and ISO 27001 claims and the pentest\n  cadence are stated in plain HTML. https://trust.iru.com/ (and trust.kandji.io, which resolves to\n  the same app) returned HTTP 200 but renders client-side — an unauthenticated fetch on 2026-08-01\n  saw only a \"Loading...\" shell, so no certification list could be read from it and none is asserted\n  from that host. Iru also SELLS a Trust Center product\n  (https://www.iru.com/products/compliance/trust-center); trust.iru.com is plausibly Iru dogfooding\n  it, but that is not asserted here as fact.\nevidence:\n- source: https://www.iru.com/security\n  keywords:\n  - soc 2\n  - trust center\nx-evidence:\n- {fetched: '2026-08-01', url: 'https://www.iru.com/security',\
  \ http_status: 200, keywords: [soc 2 type ii, iso 27001, penetration test, vulnerability disclosure program]}\n- {fetched: '2026-08-01', url: 'https://trust.iru.com/', http_status: 200, note: 'JS-rendered; body was a Loading shell — no certifications readable'}\n- {fetched: '2026-08-01', url: 'https://trust.kandji.io/', http_status: 200, note: same app as trust.iru.com}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/security/kandji-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001
tags:
- Company
- device-management
- mobile-device-management
- apple-management
- endpoint-security
- endpoint-detection-response
- vulnerability-management
- compliance-automation
- workforce-identity
- it-operations
- mcp
- agent-native
trust_url: https://trust.iru.com/
---
