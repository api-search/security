---
api_specs:
- filename: bindbee-candidates-api-openapi.yml
  format: yaml
  label: Bindbee Candidates API
  slug: bindbee-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-candidates-api-openapi.yml
- filename: bindbee-departments-api-openapi.yml
  format: yaml
  label: Bindbee Departments API
  slug: bindbee-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-departments-api-openapi.yml
- filename: bindbee-employees-api-openapi.yml
  format: yaml
  label: Bindbee Employees API
  slug: bindbee-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-employees-api-openapi.yml
- filename: bindbee-jobs-api-openapi.yml
  format: yaml
  label: Bindbee Jobs API
  slug: bindbee-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-jobs-api-openapi.yml
- filename: bindbee-time-off-api-openapi.yml
  format: yaml
  label: Bindbee Time Off API
  slug: bindbee-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-time-off-api-openapi.yml
- filename: bindbee-unified-api-openapi.json
  format: json
  label: Bindbee Unified API
  slug: bindbee-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-unified-api-openapi.json
certification_count: 4
certifications:
- SOC 2 Type II
- ISO 27001
- HIPAA
- GDPR
description: ''
kind: trust-center
layout: security
name: Bindbee Trust Center
name_suffix: Trust Center
overview: Bindbee maintains a public trust center documenting SOC 2 Type II, ISO 27001, HIPAA, and GDPR compliance.
provider_name: Bindbee
provider_slug: bindbee
slug: bindbee-trust-center
source_filename: bindbee-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://trust.bindbee.dev/ and https://bindbee.dev/pricing\nprovider: Bindbee\nproviderId: bindbee\ntrust_center:\n  url: https://trust.bindbee.dev/\n  http_status: 200\n  checked: '2026-09-04'\n  title: Trust Vault\n  hosted: true\n  readable: false\n  note: >-\n    Bindbee runs a dedicated trust portal on its own subdomain. The page is a Next.js application\n    that renders its content entirely client-side (the server response carries only the shell and a\n    sites/[slug] route keyed on \"trust.bindbee.dev\"), so no certification, report or subprocessor\n    list could be read from it by a crawler. The certifications below are therefore sourced from\n    the server-rendered pricing page, not from the trust center itself.\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  source: https://bindbee.dev/pricing\n- name: ISO 27001\n  status: claimed\n  source: https://bindbee.dev/pricing\n- name: HIPAA\n  status:\
  \ claimed\n  detail: Business Associate Agreements offered.\n  source: https://bindbee.dev/pricing\n- name: GDPR\n  status: claimed\n  source: https://bindbee.dev/pricing\npolicies:\n  privacy: https://www.bindbee.dev/policies/privacy-policy\n  terms: https://www.bindbee.dev/policies/terms-of-use\n  index: https://bindbee.dev/policies\nsecurity_program:\n  vulnerability_disclosure: not published\n  security_txt: absent — /.well-known/security.txt returns 404 on all five Bindbee hosts\n  bug_bounty: none found on HackerOne, Bugcrowd or Intigriti\n  security_contact: >-\n    No dedicated security address is published. support@bindbee.dev is the only contact stated in\n    the documentation.\n  note: >-\n    A company holding SOC 2 Type II and claiming ISO 27001 has a vulnerability-management process\n    by definition; what is missing is a public front door to it. Publishing an RFC 9116\n    security.txt naming a Contact and a Policy URL is the smallest possible fix and would make the\n\
  \    existing program discoverable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/security/bindbee-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, HIPAA, GDPR
tags:
- ATS
- HR Integration
- HRIS
- Workforce
- Unified API
- Payroll
- LMS
- Employee Data
- Integrations
trust_url: ''
---
