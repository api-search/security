---
api_specs:
- filename: gloo-api-products-api-openapi.yml
  format: yaml
  label: Gloo API Products API
  slug: gloo-api-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-api-products-api-openapi.yml
- filename: gloo-applications-api-openapi.yml
  format: yaml
  label: Gloo Applications API
  slug: gloo-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-applications-api-openapi.yml
- filename: gloo-me-api-openapi.yml
  format: yaml
  label: Gloo Me API
  slug: gloo-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-me-api-openapi.yml
- filename: gloo-subscriptions-api-openapi.yml
  format: yaml
  label: Gloo Subscriptions API
  slug: gloo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-subscriptions-api-openapi.yml
- filename: gloo-teams-api-openapi.yml
  format: yaml
  label: Gloo Teams API
  slug: gloo-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-teams-api-openapi.yml
- filename: gloo-user-api-openapi.yml
  format: yaml
  label: Gloo User API
  slug: gloo-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-user-api-openapi.yml
- filename: gloo-webhooks-api-openapi.yml
  format: yaml
  label: Gloo Webhooks API
  slug: gloo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-webhooks-api-openapi.yml
- filename: gloo-apis-api-openapi.yml
  format: yaml
  label: Gloo AP Is API
  slug: gloo-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-apis-api-openapi.yml
certification_count: 0
certifications: []
description: 'Solo.io operates a public trust center at https://trust.solo.io/, hosted on Vanta. The page returns HTTP 200 and is linked from https://www.solo.io/security and from the Solo.io site footer. Its substance is rendered entirely client-side, so no certification, audit report or control list could be read from the served HTML on 2026-09-12 — only the canonical title ("Solo Trust Center") and the company description in the meta tags. Certifications are therefore recorded as UNVERIFIED rather than asserted: this pipeline does not claim a certification it could not read.'
kind: trust-center
layout: security
name: Gloo Trust Center
name_suffix: Trust Center
overview: Gloo maintains a public trust center covering its security and compliance posture.
provider_name: Gloo
provider_slug: gloo
slug: gloo-trust-center
source_filename: gloo-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://trust.solo.io/\nprovider: Gloo\nproviderId: gloo\ndescription: >-\n  Solo.io operates a public trust center at https://trust.solo.io/, hosted on Vanta. The page\n  returns HTTP 200 and is linked from https://www.solo.io/security and from the Solo.io site\n  footer. Its substance is rendered entirely client-side, so no certification, audit report or\n  control list could be read from the served HTML on 2026-09-12 — only the canonical title\n  (\"Solo Trust Center\") and the company description in the meta tags. Certifications are\n  therefore recorded as UNVERIFIED rather than asserted: this pipeline does not claim a\n  certification it could not read.\ntrust_center:\n  url: https://trust.solo.io/\n  http_status: 200\n  platform: Vanta\n  platform_evidence: >-\n    Served HTML carries data-signature-manifest-url https://assets.vanta.com/static/... and\n    og:image https://app.vanta.com/doc?s=... — the standard Vanta\
  \ Trust Center shell.\n  machine_readable: false\n  javascript_rendered: true\n  documents_require_request: unknown\ncertifications: []\ncertifications_note: >-\n  No SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP or GDPR attestation could be confirmed from any\n  served document. Neither https://www.solo.io/security nor the trust center HTML names one,\n  and the Vanta SPA catch-all answers HTTP 200 with the same shell for every path, so no API\n  endpoint on that host yields the control list either.\nrelated:\n  - type: SecurityPolicy\n    url: https://www.solo.io/security\n  - type: PrivacyPolicy\n    url: https://legal.solo.io/#privacy-policy\n  - type: DataProcessingAgreement\n    url: https://legal.solo.io/#subscriber-dpa\n  - type: Subprocessors\n    url: https://legal.solo.io/#subprocessors\nevidence:\n  - url: https://trust.solo.io/\n    status: 200\n    fetched: '2026-09-12'\n    note: 6,607-byte HTML shell; body rendered client-side by Vanta.\n  - url: https://trust.solo.io/.well-known/security.txt\n\
  \    status: 200\n    fetched: '2026-09-12'\n    note: FALSE POSITIVE — SPA catch-all returns the identical HTML shell for every path, not a document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/security/gloo-trust-center.yml
summary_line: trust center published
tags:
- API Gateway
- Cloud-Native
- Developer Portal
- Envoy
- Istio
- Kubernetes
- Kubernetes Gateway API
- Open-Source
- Service Mesh
trust_url: ''
---
