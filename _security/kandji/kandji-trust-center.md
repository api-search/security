---
api_specs:
- filename: kandji-audit-api-openapi.yml
  format: yaml
  label: Iru Audit API
  slug: kandji-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-audit-api-openapi.yml
- filename: kandji-behavioral-detections-api-openapi.yml
  format: yaml
  label: Iru Behavioral Detections API
  slug: kandji-behavioral-detections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-behavioral-detections-api-openapi.yml
- filename: kandji-blueprints-api-openapi.yml
  format: yaml
  label: Iru Blueprints API
  slug: kandji-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-blueprints-api-openapi.yml
- filename: kandji-devices-api-openapi.yml
  format: yaml
  label: Iru Devices API
  slug: kandji-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-devices-api-openapi.yml
- filename: kandji-integrations-api-openapi.yml
  format: yaml
  label: Iru Integrations API
  slug: kandji-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-integrations-api-openapi.yml
- filename: kandji-library-api-openapi.yml
  format: yaml
  label: Iru Library API
  slug: kandji-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-library-api-openapi.yml
- filename: kandji-prism-api-openapi.yml
  format: yaml
  label: Iru Prism API
  slug: kandji-prism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-prism-api-openapi.yml
- filename: kandji-self-service-api-openapi.yml
  format: yaml
  label: Iru Self Service API
  slug: kandji-self-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-self-service-api-openapi.yml
- filename: kandji-settings-api-openapi.yml
  format: yaml
  label: Iru Settings API
  slug: kandji-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-settings-api-openapi.yml
- filename: kandji-tags-api-openapi.yml
  format: yaml
  label: Iru Tags API
  slug: kandji-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-tags-api-openapi.yml
- filename: kandji-threat-details-api-openapi.yml
  format: yaml
  label: Iru Threat Details API
  slug: kandji-threat-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-threat-details-api-openapi.yml
- filename: kandji-upload-to-s3-api-openapi.yml
  format: yaml
  label: Iru Upload To S3 API
  slug: kandji-upload-to-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-upload-to-s3-api-openapi.yml
- filename: kandji-users-api-openapi.yml
  format: yaml
  label: Iru Users API
  slug: kandji-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-users-api-openapi.yml
- filename: kandji-vulnerability-management-api-openapi.yml
  format: yaml
  label: Iru Vulnerability Management API
  slug: kandji-vulnerability-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-vulnerability-management-api-openapi.yml
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
- Device Management
- Mobile Device Management
- apple-management
- Endpoint Security
- endpoint-detection-response
- Vulnerability Management
- Compliance Automation
- Workforce Identity
- IT Operations
- MCP
- agent-native
trust_url: https://trust.iru.com/
---
