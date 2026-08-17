---
api_specs:
- filename: sequel-analytics-api-openapi.yml
  format: yaml
  label: Sequel Analytics API
  slug: sequel-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-analytics-api-openapi.yml
- filename: sequel-client-api-openapi.yml
  format: yaml
  label: Sequel Client API
  slug: sequel-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-client-api-openapi.yml
- filename: sequel-company-api-openapi.yml
  format: yaml
  label: Sequel company API
  slug: sequel-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-api-openapi.yml
- filename: sequel-company-theme-api-openapi.yml
  format: yaml
  label: Sequel company theme API
  slug: sequel-company-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-api-openapi.yml
- filename: sequel-company-theme-fonts-api-openapi.yml
  format: yaml
  label: Sequel company theme fonts API
  slug: sequel-company-theme-fonts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-fonts-api-openapi.yml
- filename: sequel-company-theme-overrides-api-openapi.yml
  format: yaml
  label: Sequel company theme overrides API
  slug: sequel-company-theme-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-overrides-api-openapi.yml
- filename: sequel-event-api-openapi.yml
  format: yaml
  label: Sequel event API
  slug: sequel-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-api-openapi.yml
- filename: sequel-event-theme-api-openapi.yml
  format: yaml
  label: Sequel event theme API
  slug: sequel-event-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-theme-api-openapi.yml
- filename: sequel-event-theme-overrides-api-openapi.yml
  format: yaml
  label: Sequel event theme overrides API
  slug: sequel-event-theme-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-theme-overrides-api-openapi.yml
- filename: sequel-media-api-openapi.yml
  format: yaml
  label: Sequel Media API
  slug: sequel-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-media-api-openapi.yml
- filename: sequel-networking-api-openapi.yml
  format: yaml
  label: Sequel networking API
  slug: sequel-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-networking-api-openapi.yml
- filename: sequel-platform-api-openapi.yml
  format: yaml
  label: Sequel platform API
  slug: sequel-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-platform-api-openapi.yml
certifications: []
description: Sequel runs a hosted Trust Center at trust.sequel.io, built on Vanta's trust-report product. https://sequel.io/security redirects to it, and the marketing navigation carries a "Security — Enterprise-grade, built in" entry pointing at the same surface.
kind: trust-center
layout: security
name: Sequel Trust Center
name_suffix: Trust Center
overview: Sequel maintains a public trust center covering its security and compliance posture.
provider_name: Sequel
provider_slug: sequel
slug: sequel-trust-center
source_filename: sequel-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nurl: https://trust.sequel.io/\nvendor: Vanta\ndescription: >-\n  Sequel runs a hosted Trust Center at trust.sequel.io, built on Vanta's trust-report\n  product. https://sequel.io/security redirects to it, and the marketing navigation\n  carries a \"Security — Enterprise-grade, built in\" entry pointing at the same surface.\nevidence:\n- source: https://trust.sequel.io/\n  http_status: 200\n  content_type: text/html\n  signals:\n  - 'og:title = \"Sequel.io Trust Center\"'\n  - 'meta keywords = \"Trust, Security, Compliance, Automation\"'\n  - assets served from assets.vanta.com (Vanta trust-report bundle)\n  - 'og:image = https://app.vanta.com/doc?s=hskpdnb3qr74wzs085wtz5'\n- source: https://sequel.io/security\n  http_status: 200\n  note: 302/redirect chain resolves to https://trust.sequel.io/\ncertifications: []\ncertifications_status: not-machine-readable\ncertifications_note: >-\n  NOT an assertion that Sequel holds no\
  \ certifications — it is a statement about what\n  is anonymously readable. The Vanta trust report renders entirely client-side: the\n  served HTML contains only the page title and description, and the Vanta trust-report\n  API (api.vanta.com/v1/trust-report/<slug>) answers 401 Unauthorized without a token.\n  No named certification (SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP) appears in any\n  anonymously-fetchable document on sequel.io, docs.introvoke.com or help.sequel.io.\n  Confirming the certification list requires either a JS-rendering client or the\n  document-request flow Vanta trust centers gate behind an email.\nprobes_that_missed:\n- url: https://api.vanta.com/v1/trust-report/hskpdnb3qr74wzs085wtz5\n  status: 401\n- url: https://sequel.io/trust\n  status: 404\n- url: https://sequel.io/.well-known/security.txt\n  status: 404\nrelated:\n  vulnerability_disclosure: >-\n    No public vulnerability-disclosure policy, bug-bounty program or security.txt was\n    found — see the probes\
  \ recorded in well-known/sequel-well-known.yml. No\n    VulnerabilityDisclosure or Security artifact is emitted for that reason.\n  enterprise_controls: >-\n    The Enterprise plan advertises \"Custom contract and security review\" and \"Enhanced\n    security with IP proxy\" (plans/sequel-plans-pricing.yml), which indicates a\n    security-review process exists for enterprise buyers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/security/sequel-trust-center.yml
summary_line: trust center published
tags:
- Company
- Webinars
- Virtual Events
- Live Streaming
- Video
- Networking
- Marketing
- Events
- Webhooks
trust_url: https://trust.sequel.io/
---
