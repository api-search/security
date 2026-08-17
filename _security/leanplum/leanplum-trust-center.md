---
api_specs:
- filename: leanplum-api-openapi.json
  format: json
  label: Leanplum API
  slug: leanplum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-api-openapi.json
- filename: leanplum-a-b-tests-api-openapi.yml
  format: yaml
  label: Leanplum A/B Tests API
  slug: leanplum-a-b-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-a-b-tests-api-openapi.yml
- filename: leanplum-content-variables-api-openapi.yml
  format: yaml
  label: Leanplum Content & Variables API
  slug: leanplum-content-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-content-variables-api-openapi.yml
- filename: leanplum-data-export-api-openapi.yml
  format: yaml
  label: Leanplum Data Export API
  slug: leanplum-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-data-export-api-openapi.yml
- filename: leanplum-events-tracking-api-openapi.yml
  format: yaml
  label: Leanplum Events & Tracking API
  slug: leanplum-events-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-events-tracking-api-openapi.yml
- filename: leanplum-messaging-api-openapi.yml
  format: yaml
  label: Leanplum Messaging API
  slug: leanplum-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-messaging-api-openapi.yml
- filename: leanplum-postbacks-batch-api-openapi.yml
  format: yaml
  label: Leanplum Postbacks & Batch API
  slug: leanplum-postbacks-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-postbacks-batch-api-openapi.yml
- filename: leanplum-user-device-attributes-api-openapi.yml
  format: yaml
  label: Leanplum User & Device Attributes API
  slug: leanplum-user-device-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-user-device-attributes-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
- GDPR
- CCPA
- HIPAA
description: 'Leanplum publishes no trust center of its own. Leanplum was acquired by CleverTap in 2022 and its website now 301-redirects to clevertap.com — the operating company''s public surface IS clevertap.com — so the trust surface recorded here is CleverTap''s. This is an inherited-parent record, stated as such: the CleverTap security page does not name Leanplum anywhere, and no Leanplum-scoped attestation was found.'
kind: trust-center
layout: security
name: Leanplum Trust Center
name_suffix: Trust Center
overview: Leanplum maintains a public trust center documenting SOC 2 Type II, ISO 27001, GDPR, CCPA, and HIPAA compliance.
provider_name: Leanplum
provider_slug: leanplum
slug: leanplum-trust-center
source_filename: leanplum-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://clevertap.com/security/\nfetched: '2026-08-13'\ndescription: >-\n  Leanplum publishes no trust center of its own. Leanplum was acquired by CleverTap\n  in 2022 and its website now 301-redirects to clevertap.com — the operating\n  company's public surface IS clevertap.com — so the trust surface recorded here is\n  CleverTap's. This is an inherited-parent record, stated as such: the CleverTap\n  security page does not name Leanplum anywhere, and no Leanplum-scoped attestation\n  was found.\nownership_justification: >-\n  https://www.leanplum.com/ returns 200 after a 301 chain terminating at\n  https://clevertap.com/; https://www.leanplum.com/pricing lands on\n  https://clevertap.com/pricing/ and https://www.leanplum.com/blog/ on\n  https://clevertap.com/blog/. CleverTap is the company that operates the Leanplum\n  brand.\ntrust_center:\n  url: https://clevertap.com/security/\n  status: 200\n  operator: CleverTap\n  leanplum_named_on_page:\
  \ false\nportal:\n  name: CleverTap Trust Portal\n  url: https://trust.clevertap.com/\n  status: 403\n  note: >-\n    Probed 2026-08-13 and returned HTTP 403 to an anonymous client — audit reports,\n    policies and controls are gated. The security page describes it as hosting\n    \"security posture, audit reports, policies and controls\".\ncertifications:\n- name: SOC 2 Type II\n  scope: CleverTap platform\n  evidence_url: https://clevertap.com/security/\n- name: ISO 27001\n  scope: CleverTap platform\n  evidence_url: https://clevertap.com/security/\n- name: GDPR\n  type: regulation compliance claim\n  evidence_url: https://clevertap.com/security/\n- name: CCPA\n  type: regulation compliance claim\n  evidence_url: https://clevertap.com/security/\n- name: HIPAA\n  type: regulation compliance claim\n  evidence_url: https://clevertap.com/security/\nverbatim_claim: >-\n  \"CleverTap currently is compliant with GDPR, CCPA, SOC 2 Type II, ISO 27001, and\n  HIPAA.\"\nplatform_controls:\n- two-factor\
  \ authentication\n- role-based access\n- restricted IP access\n- campaign approval workflow\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No security.txt on any Leanplum host (7 well-known paths x 2 hosts, all 404), no\n    bug bounty program found on HackerOne/Bugcrowd/Intigriti, and no security contact\n    or disclosure policy on the CleverTap security page. probe-security-programs.py\n    returned vdp=none on 2026-08-13, so no vulnerability-disclosure artifact was\n    written and no VulnerabilityDisclosure or Security pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/security/leanplum-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, GDPR, CCPA, HIPAA
tags:
- Mobile Marketing
- Customer Engagement
- Push Notifications
- Messaging
- A/B Testing
- Analytics
- CleverTap
trust_url: ''
---
