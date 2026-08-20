---
certifications:
- SOC 2 Type II
- ISO/IEC 27001:2022
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Enboarder Trust Center
name_suffix: Trust Center
overview: Enboarder maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001:2022, GDPR, and CCPA compliance.
provider_name: Enboarder
provider_slug: enboarder
slug: enboarder-trust-center
source_filename: enboarder-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nsource: https://enboarder.com/trust/\nurl: https://enboarder.com/trust/\nnote: >-\n  Enboarder runs no third-party trust portal (trust.enboarder.com does not resolve) and no\n  automated trust-center probe hit. The compliance posture is published across two\n  first-party pages — the Trust page and the Legal Centre security page — which is what\n  this artifact records.\npages:\n- url: https://enboarder.com/trust/\n  http_status: 200\n  role: trust overview\n- url: https://enboarder.com/legal/security/\n  http_status: 200\n  role: security detail (certifications, data residency)\n- url: https://enboarder.com/legal/\n  http_status: 200\n  role: legal centre index\ncertifications:\n- name: SOC 2 Type II\n  authority: AICPA\n  source: https://enboarder.com/legal/security/\n  detail: >-\n    \"SOC 2 Type II Audit is a third-party audit that's part of the American Institute of\n    CPA's (AICPA) Service Organization Control\"\
  \n- name: ISO/IEC 27001:2022\n  authority: ISO/IEC\n  source: https://enboarder.com/legal/security/\n- name: GDPR\n  authority: EU\n  source: https://enboarder.com/trust/\n- name: CCPA\n  authority: State of California\n  source: https://enboarder.com/trust/\ndata_residency:\n  regions:\n  - United States\n  - Europe\n  - Asia-Pacific\n  - Canada\n  detail: >-\n    Dedicated regional storage centres; \"data is subject to the laws and regulations of\n    that area\". Enforced at the API layer through region-scoped base hosts\n    (api.ore / api.fra / api.syd / api.can .e1.enboarder.com).\n  source: https://enboarder.com/legal/security/\nvulnerability_disclosure: security/enboarder-vulnerability-disclosure.yml\ngaps:\n- No downloadable or gated evidence portal (no SOC 2 report request flow published).\n- No sub-processor list published (https://enboarder.com/legal/sub-processors/ returns 404).\n- No penetration-testing cadence published.\n- No status page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enboarder/refs/heads/main/security/enboarder-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001:2022, GDPR, CCPA
tags:
- Company
- Human Resources
- Employee Onboarding
- Employee Experience
- HR Technology
- Workflow-Automation
- SCIM
- Identity Provisioning
- Webhook
- Offboarding
trust_url: https://enboarder.com/trust/
---
