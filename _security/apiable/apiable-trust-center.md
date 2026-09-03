---
api_specs:
- filename: apiable-platform-api-openapi.json
  format: json
  label: Apiable Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-platform-api-openapi.json
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
- Kong
- Platform
- Self-Service
trust_url: https://trust.apiable.io/
---
