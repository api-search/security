---
api_specs:
- filename: emerge-authentication-api-openapi.yml
  format: yaml
  label: Emerge Authentication API
  slug: emerge-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-authentication-api-openapi.yml
- filename: emerge-awards-api-openapi.yml
  format: yaml
  label: Emerge Awards API
  slug: emerge-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-awards-api-openapi.yml
- filename: emerge-network-partners-api-openapi.yml
  format: yaml
  label: Emerge Network Partners API
  slug: emerge-network-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-network-partners-api-openapi.yml
- filename: emerge-opportunities-api-openapi.yml
  format: yaml
  label: Emerge Opportunities API
  slug: emerge-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-opportunities-api-openapi.yml
- filename: emerge-options-api-openapi.yml
  format: yaml
  label: Emerge Options API
  slug: emerge-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-options-api-openapi.yml
- filename: emerge-shipments-api-openapi.yml
  format: yaml
  label: Emerge Shipments API
  slug: emerge-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-shipments-api-openapi.yml
- filename: emerge-tender-api-openapi.yml
  format: yaml
  label: Emerge Tender API
  slug: emerge-tender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-tender-api-openapi.yml
- filename: emerge-tenders-api-openapi.yml
  format: yaml
  label: Emerge Tenders API
  slug: emerge-tenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-tenders-api-openapi.yml
- filename: emerge-webhooks-api-openapi.yml
  format: yaml
  label: Emerge Webhooks API
  slug: emerge-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-webhooks-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Emerge Trust Center
name_suffix: Trust Center
overview: Emerge maintains a public trust center covering its security and compliance posture.
provider_name: Emerge
provider_slug: emerge
slug: emerge-trust-center
source_filename: emerge-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nurl: https://trust.emergemarket.com/\ntitle: EmergeTech Inc Trust Center\nplatform: Vanta\nstatus: 200\ncertifications: []\ncertifications_note: >-\n  The trust center exists and resolves under Emerge's own domain, but its contents are rendered\n  entirely client-side by the Vanta trust-report SPA. Every path under trust.emergemarket.com\n  (including /api/trust-report and /trust-report.json) returns the same HTML shell, so no named\n  certification (SOC 2, ISO 27001, ISO 27017/27018, PCI DSS, HIPAA, FedRAMP, GDPR, CSA STAR) could\n  be read anonymously. Certifications are recorded as an empty list — checked, nothing verifiable —\n  NOT as an assertion that Emerge holds none. No `type: Compliance` pointer is emitted, because that\n  check asserts a published, verifiable compliance program.\ndocument_request:\n  url: https://app.vanta.com/doc?s=REDACTED_VANTA_DOC_TOKEN\n  note: >-\n    The page links a Vanta document share,\
  \ which is the gated path to whatever reports EmergeTech\n    publishes to prospects. The share token is not reproduced here.\n  gated: true\nevidence:\n- source: https://trust.emergemarket.com/\n  status: 200\n  keywords: [trust center, vanta]\n  rendered: client-side\n- source: https://www.emergemarket.com/trust\n  status: 404\n- source: https://security.emergemarket.com/\n  status: 403\n  note: Cloudflare error 1014 — not a served host\nrelated:\n  vulnerability_disclosure: security/emerge-vulnerability-disclosure.yml\n  domain_security: security/emerge-domain-security.yml\n  privacy_policy: https://www.emergemarket.com/legal/privacy-policy\n  terms: https://www.emergemarket.com/legal/terms-and-conditions\n  api_terms: https://www.emergemarket.com/legal/api-terms-of-use\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/security/emerge-trust-center.yml
summary_line: trust center published
tags:
- freight
- Logistics
- Transportation
- Supply Chain
- Procurement
- trucking
- freight-marketplace
- transportation-management
- Shipping
- rate-benchmarking
- Webhook
- b2b-marketplace
trust_url: https://trust.emergemarket.com/
---
