---
api_specs:
- filename: apiable-companies-api-openapi.yml
  format: yaml
  label: Apiable Companies API
  slug: apiable-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-companies-api-openapi.yml
- filename: apiable-custom-properties-api-openapi.yml
  format: yaml
  label: Apiable Custom Properties API
  slug: apiable-custom-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-custom-properties-api-openapi.yml
- filename: apiable-docs-api-openapi.yml
  format: yaml
  label: Apiable Docs API
  slug: apiable-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-docs-api-openapi.yml
- filename: apiable-files-api-openapi.yml
  format: yaml
  label: Apiable Files API
  slug: apiable-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-files-api-openapi.yml
- filename: apiable-invitations-api-openapi.yml
  format: yaml
  label: Apiable Invitations API
  slug: apiable-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-invitations-api-openapi.yml
- filename: apiable-plans-api-openapi.yml
  format: yaml
  label: Apiable Plans API
  slug: apiable-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-plans-api-openapi.yml
- filename: apiable-products-api-openapi.yml
  format: yaml
  label: Apiable Products API
  slug: apiable-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-products-api-openapi.yml
- filename: apiable-subscriptions-api-openapi.yml
  format: yaml
  label: Apiable Subscriptions API
  slug: apiable-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-subscriptions-api-openapi.yml
- filename: apiable-teams-api-openapi.yml
  format: yaml
  label: Apiable Teams API
  slug: apiable-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-teams-api-openapi.yml
- filename: apiable-users-api-openapi.yml
  format: yaml
  label: Apiable Users API
  slug: apiable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-users-api-openapi.yml
- filename: apiable-webhooks-api-openapi.yml
  format: yaml
  label: Apiable Webhooks API
  slug: apiable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-webhooks-api-openapi.yml
- filename: apiable-server-info-api-openapi.yml
  format: yaml
  label: Apiable Server Info API
  slug: apiable-server-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-server-info-api-openapi.yml
certification_count: 3
certifications:
- AWS Well-Architected Framework Review
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Apiable Trust Center
name_suffix: Trust Center
overview: Apiable maintains a public trust center documenting AWS Well-Architected Framework Review, ISO 27001, and GDPR compliance.
provider_name: Apiable
provider_slug: apiable
slug: apiable-trust-center
source_filename: apiable-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nprobe: true\nsource: https://www.apiable.io/security/\nurl: https://trust.apiable.io/\ntrust_center:\n  url: https://trust.apiable.io/\n  platform: Vanta Trust Center\n  title: Apiable Trust Center\n  http_status: 200\n  probed: '2026-09-02'\nsecurity_page: https://www.apiable.io/security/\ncertifications:\n  - name: AWS Well-Architected Framework Review\n    status: achieved\n    year: 2025\n  - name: ISO 27001\n    status: in-progress\n    target_year: 2026\n  - name: GDPR\n    status: compliance-claimed\n    note: a regulatory regime, not a certification\ncorrection: >-\n  A prior round of this artifact listed \"ISO 27001\" as an achieved certification. Apiable's own\n  security page states \"ISO 27001 in progress (2026)\". Corrected 2026-09-02 to in-progress.\nposture:\n  hosting: AWS eu-central-1 (Frankfurt); additional regions available for enterprise customers\n  tenancy: dedicated single-tenant portal instance with its own\
  \ database per customer\n  proxy: >-\n    Apiable is not in the API request path. Gateway access logs are read retrospectively\n    (CloudWatch Logs, Konnect analytics, Apigee analytics) for usage and billing.\n  encryption_in_transit: TLS 1.2+ enforced on all customer-facing endpoints\n  encryption_at_rest: AES-256 via AWS-managed services (RDS, S3, DynamoDB)\n  secrets: gateway credentials in AWS Secrets Manager behind a dedicated per-customer IAM role\n  audit_log: immutable admin audit log available to customer administrators\n  subprocessors: https://www.apiable.io/terms/subprocessors/\n  disclosure: >-\n    Apiable publishes an \"Honest disclosure\" section stating that adding an Apiable integration\n    grants Apiable admin access to the connected API gateway.\nevidence:\n  - source: https://www.apiable.io/security/\n    http_status: 200\n    keywords: [iso 27001 in progress, gdpr, aws well-architected, tls 1.2, aes-256, single-tenant]\n  - source: https://trust.apiable.io/\n  \
  \  http_status: 200\n    keywords: [apiable trust center, vanta]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/security/apiable-trust-center.yml
summary_line: AWS Well-Architected Framework Review, ISO 27001, GDPR
tags:
- Amazon API Gateway
- API Gateway
- API Monetization
- API Portal
- Developer Experience
- Developer Portal
- Developer Tools
- Kong
- Platform
- Self-Service
trust_url: https://trust.apiable.io/
---
