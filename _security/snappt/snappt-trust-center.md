---
api_specs:
- filename: snappt-account-api-openapi.yml
  format: yaml
  label: Snappt Account API
  slug: snappt-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-account-api-openapi.yml
- filename: snappt-applicant-sessions-api-openapi.yml
  format: yaml
  label: Snappt Applicant Sessions API
  slug: snappt-applicant-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-applicant-sessions-api-openapi.yml
- filename: snappt-applicants-api-openapi.yml
  format: yaml
  label: Snappt Applicants API
  slug: snappt-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-applicants-api-openapi.yml
- filename: snappt-id-verification-api-openapi.yml
  format: yaml
  label: Snappt ID Verification API
  slug: snappt-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-id-verification-api-openapi.yml
- filename: snappt-internal-idv-api-openapi.yml
  format: yaml
  label: Snappt Internal IDV API
  slug: snappt-internal-idv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-internal-idv-api-openapi.yml
- filename: snappt-properties-api-openapi.yml
  format: yaml
  label: Snappt Properties API
  slug: snappt-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-properties-api-openapi.yml
- filename: snappt-webhooks-api-openapi.yml
  format: yaml
  label: Snappt Webhooks API
  slug: snappt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-webhooks-api-openapi.yml
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Snappt Trust Center
name_suffix: Trust Center
overview: Snappt maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Snappt
provider_slug: snappt
slug: snappt-trust-center
source_filename: snappt-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: true\nurl: https://trust.snappt.com/\ntitle: SNAPPT Trust Center\nplatform: Vanta\nnote: >-\n  0-working/probe-security-programs.py recorded no hit because the Vanta trust report is rendered\n  client-side — the served HTML carries no compliance keywords for the keyword gate to match. The\n  page is real: it returns HTTP 200 with <title>SNAPPT Trust Center</title>, a\n  content-location of https://assets.vanta.com/static/index-trust-report...html and a\n  Vanta-scoped Content-Security-Policy. Certification artifacts on it are gated behind a Vanta\n  document-access request (https://app.vanta.com/doc?s=...), so the named certification below is\n  taken from Snappt's own public security page rather than from the gated trust center.\ncertifications:\n- SOC 2 Type II\nregulatory_claims:\n- FCRA\n- Fair Housing Act\nsecurity_page: https://snappt.com/security/\nsecurity_practices:\n- Encryption of all data in motion and at rest\n\
  - Mandatory security and compliance training for employees handling sensitive information\n- AWS-hosted infrastructure with built-in security and redundancy\ndocument_access:\n  gated: true\n  mechanism: Vanta document request\n  example: https://app.vanta.com/doc?s=695pfvmm32o3enw49nqwc\nevidence:\n- {source: 'https://trust.snappt.com/', http_status: 200, signal: 'title \"SNAPPT Trust Center\"; content-location assets.vanta.com index-trust-report'}\n- {source: 'https://snappt.com/security/', http_status: 200, signal: 'SOC 2 Type II Compliance, FCRA Compliance, Fair Housing Act'}\ngaps:\n- No /.well-known/security.txt on any Snappt host (snappt.com returns 404; the host returns real 404s).\n- No published vulnerability disclosure or responsible-disclosure policy, and no bug bounty program found on HackerOne, Bugcrowd or Intigriti.\n- 'No security@ contact published; the only published contact is partnersupport@snappt.com (API support).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/security/snappt-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- fraud-detection
- document-verification
- Identity Verification
- income-verification
- property-management
- multifamily
- real-estate
- proptech
- tenant-screening
- rental-applications
- Webhook
trust_url: https://trust.snappt.com/
---
