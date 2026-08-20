---
api_specs:
- filename: blng-journey-api-openapi.yml
  format: yaml
  label: BLNG Journey API
  slug: blng-journey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-journey-api-openapi.yml
- filename: blng-user-api-openapi.yml
  format: yaml
  label: BLNG User API
  slug: blng-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-user-api-openapi.yml
- filename: blng-billing-api-openapi.yml
  format: yaml
  label: BLNG Billing API
  slug: blng-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-billing-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Blng Trust Center
name_suffix: Trust Center
overview: Blng maintains a public trust center covering its security and compliance posture.
provider_name: Blng
provider_slug: blng
slug: blng-trust-center
source_filename: blng-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://trust.blng.ai/\npresent: true\nplatform: Vanta Trust Center\nplatform_evidence: >-\n  trust.blng.ai is a CNAME to 69d5a4d9eef946c721025951.cname.vantatrust.com, and the served page loads\n  its bundle from assets.vanta.com (index-trust-report.vite-*.js).\nurl: https://trust.blng.ai/\nhttp_status: 200\ntitle: blng.ai Trust Center\ncertifications: []\ncertifications_readable: false\nnote: >-\n  The trust center exists and answers 200, but every certification, control and policy on it is rendered\n  client-side by the Vanta React bundle. A non-JS client receives only the page shell, the title\n  \"blng.ai Trust Center\" and a meta description that repeats BLNG's mission statement — no SOC 2, ISO\n  27001, PCI, HIPAA or FedRAMP string appears anywhere in the served HTML. Vanta retired its public\n  GraphQL API (api.vanta.com/graphql returns HTTP 410 pointing at the REST API) and the REST trust-center\n  endpoint requires\
  \ authorization (HTTP 401), so there is no anonymous machine path to the certification\n  list. Recorded as present with certifications unknown rather than guessed. NO `Compliance` pointer is\n  wired in apis.yml — that check requires a named, published certification.\ndocument_access: >-\n  Vanta trust centers typically gate report downloads behind an NDA/email request form; whether BLNG's\n  does could not be determined without executing the page.\nrelated:\n  privacy_policy: https://blng.ai/privacy-policy\n  california_notices: https://blng.ai/privacy-policy#california-notices\n  privacy_choices: https://blng.ai/your-privacy-choices\n  terms: https://blng.ai/terms\n  data_controls_doc: https://docs.blng.ai/account-management/data-controls/\n  account_security_doc: https://docs.blng.ai/account-management/security/\nx-evidence:\n- url: https://trust.blng.ai/\n  http_status: 200\n  content_type: text/html\n  bytes: 4953\n  fetched: '2026-08-13'\n- url: https://api.vanta.com/graphql\n \
  \ http_status: 410\n  fetched: '2026-08-13'\n  finding: GraphQL API retired in favor of the Vanta REST API\n- url: https://api.vanta.com/v1/trust-centers/69d5a4d9eef946c721025951\n  http_status: 401\n  fetched: '2026-08-13'\n  finding: authorization required; no anonymous read of the certification list\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/security/blng-trust-center.yml
summary_line: trust center published
tags:
- Company
- Jewelry
- Generative AI
- Design
- Creative Tools
- Rendering
- Marketing
- Retail
- 3D Models
- Image-Generation
- Workspaces
- Billing
- OpenAPI
- AWS Cognito
trust_url: https://trust.blng.ai/
---
