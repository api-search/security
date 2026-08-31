---
api_specs:
- filename: validic-devices-api-openapi.yml
  format: yaml
  label: Validic Devices API
  slug: validic-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-devices-api-openapi.yml
- filename: validic-marketplace-connections-api-openapi.yml
  format: yaml
  label: Validic Marketplace & Connections API
  slug: validic-marketplace-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-marketplace-connections-api-openapi.yml
- filename: validic-observations-data-api-openapi.yml
  format: yaml
  label: Validic Observations & Data API
  slug: validic-observations-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-observations-data-api-openapi.yml
- filename: validic-push-service-api-openapi.yml
  format: yaml
  label: Validic Push Service API
  slug: validic-push-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-push-service-api-openapi.yml
- filename: validic-streaming-api-openapi.yml
  format: yaml
  label: Validic Streaming API
  slug: validic-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streaming-api-openapi.yml
- filename: validic-users-api-openapi.yml
  format: yaml
  label: Validic Users API
  slug: validic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-users-api-openapi.yml
- filename: validic-measurements-api-openapi.yml
  format: yaml
  label: Validic Measurements API
  slug: validic-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-measurements-api-openapi.yml
- filename: validic-organizations-api-openapi.yml
  format: yaml
  label: Validic Organizations API
  slug: validic-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-organizations-api-openapi.yml
- filename: validic-streams-api-openapi.yml
  format: yaml
  label: Validic Streams API
  slug: validic-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streams-api-openapi.yml
- filename: validic-streams-token-token-api-openapi.yml
  format: yaml
  label: Validic Streams?token={token} API
  slug: validic-streams-token-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streams-token-token-api-openapi.yml
certifications:
- HITRUST CSF
- ISO/IEC 27001
- HIPAA
description: Validic states real certifications on its own public pages, but it does NOT operate a trust centre - there is no portal at which a prospect can view or request a certificate, a scope statement, an audit date, a pen-test summary or a subprocessor list. The certifications below are first-party ASSERTIONS, recorded as such.
kind: trust-center
layout: security
name: Validic Trust Center
name_suffix: Trust Center
overview: Validic maintains a public trust center documenting HITRUST CSF, ISO/IEC 27001, and HIPAA compliance.
provider_name: Validic
provider_slug: validic
slug: validic-trust-center
source_filename: validic-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: >-\n  https://validic.com/how-we-help/arpa-h-advocate/ +\n  https://dashboard.validic.com/validic-developer-signup.txt\nurl: null\ntrust_center_published: false\ndescription: >-\n  Validic states real certifications on its own public pages, but it does NOT\n  operate a trust centre - there is no portal at which a prospect can view or\n  request a certificate, a scope statement, an audit date, a pen-test summary\n  or a subprocessor list. The certifications below are first-party ASSERTIONS,\n  recorded as such.\ncertifications:\n- name: HITRUST CSF\n  status: certified (asserted)\n  evidence:\n  - source: https://validic.com/how-we-help/arpa-h-advocate/\n    http_status: 200\n    quote: 'Compliance: HIPAA. HITRUST. ISO 27001. FHIR mapping via the Push Service.'\n  - source: https://dashboard.validic.com/validic-developer-signup.txt\n    http_status: 200\n    quote: HITRUST certified - ISO 27001 certified\n  certificate_published:\
  \ false\n  audit_date_published: false\n  assessor_published: false\n- name: ISO/IEC 27001\n  status: certified (asserted)\n  evidence:\n  - source: https://validic.com/how-we-help/arpa-h-advocate/\n    http_status: 200\n  - source: https://dashboard.validic.com/validic-developer-signup.txt\n    http_status: 200\n  certificate_published: false\n  audit_date_published: false\n  assessor_published: false\n- name: HIPAA\n  status: compliant (asserted, and reflected in API design)\n  evidence:\n  - source: https://validic.com/how-we-help/arpa-h-advocate/\n    http_status: 200\n  - source: https://developer.validic.com/docs/inform-rest-api\n    http_status: 200\n    detail: >-\n      HIPAA drives documented API behaviour, not just a claim - the ban on\n      identifying data in `uid`, and the 1-year-over-API / 7-year-retained\n      split on health records.\ncorrections:\n- date: '2026-08-15'\n  removed:\n  - SOC 2\n  reason: >-\n    A previous pass recorded SOC 2 and ISO 27001 for Validic\
  \ from a keyword\n    match on https://trust.validic.com/ and treated that host as a trust\n    centre. Both parts of that were wrong. (1) trust.validic.com is an ATLASSIAN\n    STATUSPAGE, not a trust centre - DNS CNAME\n    trust.validic.com -> qtyl0stcbvvr.stspg-customer.com, page title \"Validic\n    Inform Status\", live component and incident APIs at /api/v2/*. It is now\n    recorded correctly in lifecycle/validic-lifecycle.yml as the status page.\n    (2) The strings \"SOC 2\" and \"ISO 27001\" appear on that page exactly once\n    each, inside an incident notice about Google Health API CASA requirements\n    which advises CUSTOMERS to \"gather existing certifications - SOC 2 or ISO\n    27002 documentation\". That is guidance to Validic's customers about THEIR\n    own audits; it is not a Validic certification claim. No first-party SOC 2\n    assertion exists anywhere on Validic's public surface.\n  kept:\n  - ISO 27001\n  kept_reason: >-\n    ISO 27001 survives the correction,\
  \ but on completely different evidence -\n    Validic asserts it directly on validic.com and in its own\n    provider-published developer guide.\nprobe:\n- url: https://trust.validic.com/\n  status: 200\n  finding: Atlassian Statuspage titled \"Validic Inform Status\" - not a trust centre\n- url: https://validic.com/security/\n  status: 200\n  finding: >-\n    soft-404 - validic.com 200-redirects unknown paths to `/`. Effective URL\n    was https://validic.com/. No security page exists.\n- url: https://validic.com/compliance/\n  status: 200\n  finding: soft-404 to `/`. No compliance page exists.\n- url: https://validic.com/privacy-policy/\n  status: 200\n  finding: real page - the only published policy document found\nsubprocessors_published: false\npen_test_published: false\nsoc2_report_available_on_request: unknown\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/security/validic-trust-center.yml
summary_line: HITRUST CSF, ISO/IEC 27001, HIPAA
tags:
- Health Data
- Digital Health
- Wearables
- Remote Patient Monitoring
- Health IoT
- Interoperability
- HIPAA
trust_url: ''
---
