---
api_specs:
- filename: experian-address-validation-api-openapi.yml
  format: yaml
  label: Experian Address Validation API
  slug: experian-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-address-validation-api-openapi.yml
- filename: experian-bulk-address-api-openapi.yml
  format: yaml
  label: Experian Bulk Address API
  slug: experian-bulk-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-address-api-openapi.yml
- filename: experian-bulk-email-api-openapi.yml
  format: yaml
  label: Experian Bulk Email API
  slug: experian-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-email-api-openapi.yml
- filename: experian-bulk-phone-api-openapi.yml
  format: yaml
  label: Experian Bulk Phone API
  slug: experian-bulk-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-phone-api-openapi.yml
- filename: experian-email-validation-api-openapi.yml
  format: yaml
  label: Experian Email Validation API
  slug: experian-email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-email-validation-api-openapi.yml
- filename: experian-enrichment-api-openapi.yml
  format: yaml
  label: Experian Enrichment API
  slug: experian-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-enrichment-api-openapi.yml
- filename: experian-identity-append-usa-only-api-openapi.yml
  format: yaml
  label: Experian Identity Append (USA only) API
  slug: experian-identity-append-usa-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-identity-append-usa-only-api-openapi.yml
- filename: experian-phone-validation-api-openapi.yml
  format: yaml
  label: Experian Phone Validation API
  slug: experian-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-phone-validation-api-openapi.yml
- filename: experian-reverse-phone-append-usa-only-api-openapi.yml
  format: yaml
  label: Experian Reverse Phone Append (USA only) API
  slug: experian-reverse-phone-append-usa-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-reverse-phone-append-usa-only-api-openapi.yml
certification_count: 1
certifications:
- ISO/IEC 27001
description: ''
kind: trust-center
layout: security
name: Experian Trust Center
name_suffix: Trust Center
overview: Experian maintains a public trust center documenting ISO/IEC 27001 compliance.
provider_name: Experian
provider_slug: experian
slug: experian-trust-center
source_filename: experian-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://docs.experianaperture.io/more/request-for-information/experian-address-validation,\n  https://docs.experianaperture.io/more/request-for-information/, https://www.experianplc.com/privacy\ntrust_center:\n  published: false\n  url: null\n  note: 'Experian operates no trust center in the modern sense — no trust.experian.com, no\n    self-service portal serving SOC 2 reports, pen-test summaries or a live sub-processor list, and\n    no downloadable evidence behind an NDA click-through. What it publishes instead is a Request for\n    Information (RFI) page per product, which is a structured security questionnaire response: it\n    answers the standard due-diligence questions in prose and names the certifications, but gates the\n    evidence itself. Recorded as published: false because the artifact a buyer or an agent can\n    actually read is an RFI page, not a trust center.'\nrfi_surface:\n  published: true\n  url: https://docs.experianaperture.io/more/request-for-information/\n\
  \  per_product_example: https://docs.experianaperture.io/more/request-for-information/experian-address-validation\n  note: A per-product Request for Information page answering security, data-handling and compliance\n    questions for each Data Quality product.\ncertifications:\n- name: ISO/IEC 27001\n  scope: Experian Data Quality products\n  evidence: 'Stated verbatim on the product RFI page: \"ISO 27001 Certificates available upon\n    request.\"'\n  source: https://docs.experianaperture.io/more/request-for-information/experian-address-validation\n  verified: documented-not-downloadable\n  note: The certificate itself is not published; it is released on request. No certificate number,\n    registrar or scope statement is public.\ncertifications_unverified:\n  note: 'Third-party and Experian marketing sources describe a wider certification estate — ISO\n    27017 and ISO 27018 cloud add-ons, Cyber Essentials, and SOC 2 Type 2 for the Tapad business\n    Experian acquired. None of these\
  \ was found stated on a first-party Experian page reachable in\n    this pass, so they are recorded here as unverified leads rather than as certifications above.\n    EI3PA (Experian Independent Third Party Assessment) is notable in the other direction: it is a\n    standard Experian IMPOSES on its own data recipients rather than one it holds.'\n  leads:\n  - ISO 27017\n  - ISO 27018\n  - Cyber Essentials\n  - SOC 2 Type 2 (Tapad, an Experian company)\ncompliance_documents:\n- name: Privacy statement\n  url: https://www.experianplc.com/privacy\n- name: Developer Portal privacy policy\n  url: https://developer.experian.com/privacy-policy\n- name: Standard terms and conditions and policies (regional EDQ T&Cs, EULAs, fair-usage, cancellation)\n  url: https://docs.experianaperture.io/standard-terms-and-conditions-and-policies\n- name: SaaS Services SLA\n  url: https://docs.experianaperture.io/saas-services-sla\n- name: Global Support policy\n  url: https://docs.experianaperture.io/global-support-policy/\n\
  regulatory_context:\n  note: 'Experian is a consumer reporting agency and its credit products are regulated rather than\n    merely certified — FCRA and GLBA in the United States, the Data Protection Act / UK GDPR and FCA\n    regimes in the United Kingdom. Those obligations are structural to the business and are not a\n    published API-security artifact, so they are recorded as context here and not claimed as\n    certifications.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/security/experian-trust-center.yml
summary_line: ISO/IEC 27001
tags:
- Company
- Credit Bureau
- Credit Reporting
- Identity Verification
- Fraud Prevention
- Data Quality
- Address Validation
- Email Validation
- Phone Validation
- Data Enrichment
- Financial-Services
- Risk Management
trust_url: ''
---
