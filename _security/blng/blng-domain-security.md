---
api_specs:
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
- filename: blng-chat-prompts-api-openapi.yml
  format: yaml
  label: Blng Chat Prompts API
  slug: blng-chat-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-chat-prompts-api-openapi.yml
- filename: blng-composite-api-openapi.yml
  format: yaml
  label: Blng Composite API
  slug: blng-composite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-composite-api-openapi.yml
- filename: blng-design-journey-api-openapi.yml
  format: yaml
  label: Blng Design Journey API
  slug: blng-design-journey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-design-journey-api-openapi.yml
- filename: blng-invitation-api-openapi.yml
  format: yaml
  label: Blng Invitation API
  slug: blng-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-invitation-api-openapi.yml
- filename: blng-journeys-api-openapi.yml
  format: yaml
  label: Blng Journeys API
  slug: blng-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-journeys-api-openapi.yml
- filename: blng-organization-api-openapi.yml
  format: yaml
  label: Blng Organization API
  slug: blng-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-organization-api-openapi.yml
- filename: blng-prompts-api-openapi.yml
  format: yaml
  label: Blng Prompts API
  slug: blng-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-prompts-api-openapi.yml
- filename: blng-subscription-api-openapi.yml
  format: yaml
  label: Blng Subscription API
  slug: blng-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-subscription-api-openapi.yml
- filename: blng-user-subscription-api-openapi.yml
  format: yaml
  label: Blng User Subscription API
  slug: blng-user-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-user-subscription-api-openapi.yml
- filename: blng-user-tooltip-api-openapi.yml
  format: yaml
  label: Blng User Tooltip API
  slug: blng-user-tooltip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-user-tooltip-api-openapi.yml
- filename: blng-webhook-api-openapi.yml
  format: yaml
  label: Blng Webhook API
  slug: blng-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-webhook-api-openapi.yml
- filename: blng-workspace-api-openapi.yml
  format: yaml
  label: Blng Workspace API
  slug: blng-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blng.ai
  spf: true
hosts:
- cert_expires: Sep 16 08:46:03 2026 GMT
  host: blng.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: journeys.blng.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: users.blng.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blng, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blng
provider_slug: blng
slug: blng-domain-security
source_filename: blng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blng.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:46:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: journeys.blng.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\n- host: users.blng.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: blng.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/security/blng-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
---
