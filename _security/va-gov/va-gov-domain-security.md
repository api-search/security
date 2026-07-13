---
api_specs:
- filename: openapi.json
  format: json
  label: VA Facilities API
  slug: va-facilities-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/facilities/v1/openapi.json
- filename: openapi.json
  format: json
  label: VA Forms API
  slug: va-forms-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/forms/v0/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Claims API
  slug: benefits-claims-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-claims/v2/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Intake API
  slug: benefits-intake-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-intake/v1/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Documents API
  slug: benefits-documents-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-documents/v1/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Reference Data API
  slug: benefits-reference-data-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-reference-data/v1/openapi.json
- filename: openapi.json
  format: json
  label: Appeals Status API
  slug: appeals-status-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/appeals-status/v1/openapi.json
- filename: openapi.json
  format: json
  label: Appealable Issues API
  slug: appealable-issues-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/appealable-issues/v0/openapi.json
- filename: openapi.json
  format: json
  label: Legacy Appeals API
  slug: legacy-appeals-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/legacy-appeals/v0/openapi.json
- filename: metadata
  format: yaml
  label: Patient Health API (FHIR)
  slug: patient-health-api
  spec_type: OpenAPI
  url: https://api.va.gov/services/fhir/v0/r4/metadata
- filename: metadata
  format: yaml
  label: Clinical Health API (FHIR)
  slug: clinical-health-api
  spec_type: OpenAPI
  url: https://api.va.gov/services/fhir/v0/r4/metadata
- filename: openapi.json
  format: json
  label: Community Care Eligibility API
  slug: community-care-eligibility-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/community-care-eligibility/v0/openapi.json
- filename: openapi.json
  format: json
  label: Veteran Verification API
  slug: veteran-verification-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/veteran-verification/v2/openapi.json
- filename: openapi.json
  format: json
  label: Veteran Confirmation API
  slug: veteran-confirmation-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/veteran-confirmation/v1/openapi.json
- filename: openapi.json
  format: json
  label: Address Validation API
  slug: address-validation-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/address-validation/v3/openapi.json
- filename: openapi.json
  format: json
  label: Direct Deposit Management API
  slug: direct-deposit-management-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/direct-deposit-management/v1/openapi.json
- filename: openapi.json
  format: json
  label: VA Letter Generator API
  slug: va-letter-generator-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/va-letter-generator/v1/openapi.json
- filename: openapi.json
  format: json
  label: Loan Review API
  slug: loan-review-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/loan-review/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: va.gov
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: developer.va.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.va.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Va Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VA Lighthouse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: VA Lighthouse
provider_slug: va-gov
slug: va-gov-domain-security
source_filename: va-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.va.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.va.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: va.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/va-gov/refs/heads/main/security/va-gov-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Government
- Veterans Affairs
- Veterans
- Healthcare
- Benefits
- FHIR
- Open Data
- Federal
---
