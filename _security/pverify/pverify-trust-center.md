---
api_specs:
- filename: pverify-authentication-api-openapi.yml
  format: yaml
  label: pVerify Authentication API
  slug: pverify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-authentication-api-openapi.yml
- filename: pverify-eligibility-api-openapi.yml
  format: yaml
  label: pVerify Eligibility API
  slug: pverify-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-eligibility-api-openapi.yml
- filename: pverify-dental-eligibility-api-openapi.yml
  format: yaml
  label: pVerify Dental Eligibility API
  slug: pverify-dental-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-dental-eligibility-api-openapi.yml
- filename: pverify-insurance-discovery-api-openapi.yml
  format: yaml
  label: pVerify Insurance Discovery API
  slug: pverify-insurance-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-insurance-discovery-api-openapi.yml
- filename: pverify-mbi-lookup-api-openapi.yml
  format: yaml
  label: pVerify MBI Lookup API
  slug: pverify-mbi-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-mbi-lookup-api-openapi.yml
- filename: pverify-patient-demographic-validator-api-openapi.yml
  format: yaml
  label: pVerify Patient Demographic Validator API
  slug: pverify-patient-demographic-validator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-patient-demographic-validator-api-openapi.yml
- filename: pverify-claim-status-api-openapi.yml
  format: yaml
  label: pVerify Claim Status API
  slug: pverify-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-claim-status-api-openapi.yml
- filename: pverify-estimation-api-openapi.yml
  format: yaml
  label: pVerify Patient Cost Estimator API
  slug: pverify-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-estimation-api-openapi.yml
- filename: pverify-payers-api-openapi.yml
  format: yaml
  label: pVerify Payers API
  slug: pverify-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-payers-api-openapi.yml
- filename: pverify-cgx-widget-api-openapi.yml
  format: yaml
  label: pVerify CGX Widget API
  slug: pverify-cgx-widget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-cgx-widget-api-openapi.yml
- filename: pverify-same-or-similar-api-openapi.yml
  format: yaml
  label: pVerify Same or Similar API (discontinued)
  slug: pverify-same-or-similar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-same-or-similar-api-openapi.yml
- filename: pverify-cmn-api-openapi.yml
  format: yaml
  label: pVerify CMN API (discontinued)
  slug: pverify-cmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-cmn-api-openapi.yml
- filename: pverify-snf-api-openapi.yml
  format: yaml
  label: pVerify SNF API (discontinued)
  slug: pverify-snf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-snf-api-openapi.yml
certifications:
- SOC 2 Type II
- HIPAA
description: 'pVerify links its trust center and status dashboard from the footer of its own site (https://pverify.com/), but both are operated under the parent brand: pVerify is a DoseSpot company, and DoseSpot merged with Arrive Health to form Interra Health — which is why a pverify.com link lands on a dosespot.com host. That is the stated corporate relationship, not a third-party page: pVerify''s own homepage and developer page are the referring surface.'
kind: trust-center
layout: security
name: Pverify Trust Center
name_suffix: Trust Center
overview: pVerify maintains a public trust center documenting SOC 2 Type II and HIPAA compliance.
provider_name: pVerify
provider_slug: pverify
slug: pverify-trust-center
source_filename: pverify-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nurl: https://trust.dosespot.com/\ntitle: Interra Health Trust Center\nplatform: Vanta trust report\ndescription: >-\n  pVerify links its trust center and status dashboard from the footer of its own site\n  (https://pverify.com/), but both are operated under the parent brand: pVerify is a DoseSpot\n  company, and DoseSpot merged with Arrive Health to form Interra Health — which is why a\n  pverify.com link lands on a dosespot.com host. That is the stated corporate relationship, not a\n  third-party page: pVerify's own homepage and developer page are the referring surface.\ncertifications:\n- name: SOC 2 Type II\n  source: https://www.pverify.com/pverify-announces-successful-soc2-compliance-examination/\n  basis: pVerify's own published announcement (HTTP 200)\n- name: HIPAA\n  source: https://pverify.com/api-developers/\n  basis: provider-claimed on its own developer page; BAAs offered to customers\nevidence:\n- {source:\
  \ 'https://trust.dosespot.com/', status: 200, keywords: [trust center, interra health], note: 'Vanta-hosted trust report; the certification list renders client-side and the document index sits behind https://app.vanta.com/doc?s=... — the page itself was confirmed live but its cert list is not machine-readable anonymously.'}\n- {source: 'https://pverify.com/', status: 200, note: links trust.dosespot.com and status.dosespot.com from the site footer}\n- {source: 'https://www.pverify.com/pverify-announces-successful-soc2-compliance-examination/', status: 200, note: pVerify's own SOC 2 announcement}\nrelated:\n  status_page: https://status.dosespot.com/posts/dashboard\n  conformance: conformance/pverify-conformance.yml\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/security/pverify-trust-center.yml
summary_line: SOC 2 Type II, HIPAA
tags:
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- 270/271
- 276/277
- Revenue Cycle
- Medicare
- Payers
- Insurance Discovery
- Patient Estimation
- HIPAA
- Dental
trust_url: https://trust.dosespot.com/
---
