---
api_specs:
- filename: monetate-engine-api-openapi.yml
  format: yaml
  label: Monetate Engine API
  slug: monetate-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-engine-api-openapi.yml
- filename: monetate-data-api-openapi.yml
  format: yaml
  label: Monetate Data API
  slug: monetate-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-data-api-openapi.yml
- filename: monetate-metadata-api-openapi.yml
  format: yaml
  label: Monetate Metadata API
  slug: monetate-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-metadata-api-openapi.yml
- filename: monetate-auth-api-openapi.yml
  format: yaml
  label: Monetate Auth API
  slug: monetate-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-auth-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Monetate Trust Center
name_suffix: Trust Center
overview: Monetate maintains a public trust center covering its security and compliance posture.
provider_name: Monetate
provider_slug: monetate
slug: monetate-trust-center
source_filename: monetate-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://trust.monetate.com/\nurl: https://trust.monetate.com/\nprovider: SafeBase\npresent: true\ncertifications: []\ncertification_count: 0\nnote: >-\n  A trust center EXISTS and resolves on a Monetate-owned subdomain, but it publishes no completed\n  certification, no attestation, no audit report and no security grade. The page's own copy is the\n  giveaway that it is still a SafeBase default: \"We are working towards compliance certifications\", \"We\n  can provide completed questionnaires upon request\", \"We are currently working with experts to put\n  together our company policies\", and \"We are constantly monitoring the security of our website. We will\n  post our grades from public security rating agencies when they become available.\" No SOC 2, ISO 27001,\n  PCI DSS, HIPAA or FedRAMP is named. No vulnerability disclosure policy or bug bounty is referenced. No\n  subprocessor list or penetration test summary is linked\
  \ from it. Recorded as TrustCenter present with\n  zero certifications — deliberately NOT wired to a `Compliance` pointer, because the check that pointer\n  feeds asks whether the provider publishes a compliance program, and this provider does not yet.\nsections_present:\n- data privacy\n- endpoint security\n- incident response\n- company policies (in progress)\n- security ratings (placeholder)\ndocuments_available_on_request: true\ndocuments_gated_behind: SafeBase access request\nrelated_public_pages:\n- url: https://monetate.com/sub-processor-statement/\n  http_status: 200\n  type: sub-processor statement\n- url: https://monetate.com/website-privacy-policy/\n  http_status: 200\n  type: privacy policy\n  finding: >-\n    References \"the EU-US or Swiss-US Privacy Shield Principles\" as the safeguard standard — a framework\n    invalidated by the CJEU in Schrems II (July 2020) and replaced by the EU-US Data Privacy Framework in\n    2023. The privacy policy has not been updated for that\
  \ change.\nx-evidence:\n- fetched: '2026-08-12'\n  url: https://trust.monetate.com/\n  http_status: 200\n  content_type: text/html\n  finding: SafeBase trust center, JS-rendered, zero named certifications\n- fetched: '2026-08-12'\n  url: https://monetate.com/security/\n  http_status: 404\n- fetched: '2026-08-12'\n  url: https://monetate.com/trust/\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/security/monetate-trust-center.yml
summary_line: trust center published
tags:
- Company
- Personalization
- Experience Optimization
- A/B Testing
- Ecommerce
- Product Recommendations
- Personalized Search
- Marketing
- Customer Data
- Retail
- Decision Engine
trust_url: https://trust.monetate.com/
---
