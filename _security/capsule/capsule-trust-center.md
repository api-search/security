---
api_specs:
- filename: capsule-opportunities-api-openapi.yml
  format: yaml
  label: Capsule Opportunities API
  slug: capsule-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-opportunities-api-openapi.yml
- filename: capsule-parties-api-openapi.yml
  format: yaml
  label: Capsule Parties API
  slug: capsule-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-parties-api-openapi.yml
- filename: capsule-projects-api-openapi.yml
  format: yaml
  label: Capsule Projects API
  slug: capsule-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-projects-api-openapi.yml
- filename: capsule-tasks-api-openapi.yml
  format: yaml
  label: Capsule Tasks API
  slug: capsule-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-tasks-api-openapi.yml
certification_count: 3
certifications:
- ISO 27001
- PCI-DSS
- SOC (report)
description: Capsule's public security and compliance page. There is no dedicated trust portal - trust.capsulecrm.com was probed on 2026-09-05 and answers with the Capsule app's "The account you were looking for doesn't exist." shell, which is a false 200, not a trust center.
kind: trust-center
layout: security
name: Capsule Trust Center
name_suffix: Trust Center
overview: Capsule maintains a public trust center documenting ISO 27001, PCI-DSS, and SOC (report) compliance.
provider_name: Capsule
provider_slug: capsule
slug: capsule-trust-center
source_filename: capsule-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://capsulecrm.com/security/\ndescription: >-\n  Capsule's public security and compliance page. There is no dedicated trust\n  portal - trust.capsulecrm.com was probed on 2026-09-05 and answers with the\n  Capsule app's \"The account you were looking for doesn't exist.\" shell, which\n  is a false 200, not a trust center.\nurl: https://capsulecrm.com/security/\nstatus: 200\ndedicated_trust_portal: false\nprobed:\n- {url: 'https://trust.capsulecrm.com/', status: 200, verdict: 'soft-404 / application shell, not a trust center'}\n- {url: 'https://capsulecrm.com/security/', status: 200, verdict: live security + compliance page}\n- {url: 'https://capsulecrm.com/gdpr/', status: 200, verdict: live GDPR page}\ncertifications:\n- name: ISO 27001\n  scope: infrastructure\n  holder: Amazon Web Services\n  self_certified: false\n  note: >-\n    Capsule cites ISO 27001 as a property of the AWS data centres it runs on,\n    NOT as a\
  \ certification held by Capsule/Zestia. Recorded with that\n    distinction because the two are routinely conflated.\n- name: PCI-DSS\n  scope: payment collection\n  holder: Capsule\n  note: Cited for the handling of subscription payment collection.\n- name: SOC (report)\n  scope: infrastructure\n  holder: Amazon Web Services\n  note: >-\n    The page refers to SOC reports being available; it does not state that\n    Capsule itself holds a SOC 2 Type II attestation. No report or audit\n    period is published.\ncompliance_programs:\n- {name: GDPR, url: 'https://capsulecrm.com/gdpr/', status: 200}\nsecurity_practices:\n- Encryption in transit with current recommended cipher suites and protocols\n- Customer data encrypted at rest\n- Hosted on AWS with real-time replication across multiple locations\n- Continuous backups for disaster recovery\n- Regular third-party penetration testing\nuptime_claim: '99.99%'\ngaps:\n- No downloadable audit report, certificate or attestation letter.\n- No\
  \ security questionnaire package or NDA-gated document room.\n- No sub-processor list linked from the security page.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/security/capsule-trust-center.yml
summary_line: ISO 27001, PCI-DSS, SOC (report)
tags:
- Contact Management
- CRM
- Custom Fields
- Opportunities
- Pipelines
- Project Management
- REST
- Sales
- Task
- Webhook
trust_url: https://capsulecrm.com/security/
---
