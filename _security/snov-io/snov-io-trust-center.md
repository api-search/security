---
api_specs:
- filename: snov-io-email-verification-api-openapi.yml
  format: yaml
  label: Snov.io Email Verification API
  slug: snovio-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/snov-io-email-verification-api-openapi.yml
- filename: snov-io-campaigns-api-openapi.yml
  format: yaml
  label: Snov.io Campaigns API
  slug: snovio-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/snov-io-campaigns-api-openapi.yml
- filename: snov-io-email-warm-up-api-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snovio-email-warm-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/snov-io-email-warm-up-api-openapi.yml
- filename: snov-io-webhooks-api-openapi.yml
  format: yaml
  label: Snov.io Webhooks API
  slug: snovio-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/snov-io-webhooks-api-openapi.yml
- filename: snov-io-openapi-generated.yml
  format: yaml
  label: Snov.io API
  slug: snov-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/_ae-authored/snov-io-openapi-generated.yml
certification_count: 3
certifications:
- GDPR
- LOA (Letter of Authorization)
- CCPA / Do Not Sell My Personal Information
description: Snov.io operates a public Security Center page describing its data-protection program. It is a narrative security page rather than a trust portal — there is no document request flow, no subprocessor list, no uptime or incident history, and no named third-party audit report. The only certifications named anywhere are GDPR adherence and an LOA (Letter of Authorization).
kind: trust-center
layout: security
name: Snov.io Trust Center
name_suffix: Trust Center
overview: Snov.io maintains a public trust center documenting GDPR, LOA (Letter of Authorization), and CCPA / Do Not Sell My Personal Information compliance.
provider_name: Snov.io
provider_slug: snov-io
slug: snov-io-trust-center
source_filename: snov-io-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "name: Snov.io Trust Center\nspecificationVersion: '0.1'\ngenerated: '2026-08-13'\nmethod: searched\nsource: https://snov.io/security-center\ndescription: Snov.io operates a public Security Center page describing its data-protection program. It is a narrative\n  security page rather than a trust portal — there is no document request flow, no subprocessor list, no uptime\n  or incident history, and no named third-party audit report. The only certifications named anywhere are GDPR adherence\n  and an LOA (Letter of Authorization).\ntrust_center:\n  url: https://snov.io/security-center\n  http_status: 200\n  type: security-narrative-page\n  document_request_flow: false\n  subprocessor_list: false\n  status_history: false\n  pentest_report: false\ncertifications:\n- GDPR\n- LOA (Letter of Authorization)\n- CCPA / Do Not Sell My Personal Information\nnot_claimed:\n  frameworks:\n  - SOC 2 Type I\n  - SOC 2 Type II\n  - ISO/IEC 27001\n  - ISO/IEC 27701\n  - PCI DSS\n  - HIPAA\n  -\
  \ FedRAMP\n  - CSA STAR\n  note: None of these appear anywhere on snov.io. Snov.io states that \"internal and external audits take place regularly\n    to test access control, risk possibility, information security, and IT infrastructure\" but names no framework,\n    no auditor and no report. For a platform whose entire product is B2B contact data, the absence of a named third-party\n    attestation is the notable finding here.\ncontrols_published:\n- name: Database protections\n  detail: Encrypted passwords, intrusion detection systems, and a VPC with strict firewall settings.\n- name: Integrations security\n  detail: Integrated SaaS services are authorized with OAuth2 and their credentials are not stored.\n- name: Encryption in transit and at rest\n  detail: Data is encrypted both when transmitted over public networks and when stored.\n- name: Data recovery\n  detail: Regular backups with a maximum 24-hour RPO and a maximum 24-hour RTO.\n- name: Internal and external audits\n  detail:\
  \ Regular audits covering access control, risk, information security and IT infrastructure. No framework\n    or auditor named.\nlegal:\n  privacy_policy: https://snov.io/privacy-policy\n  gdpr: https://snov.io/gdpr\n  terms: https://snov.io/terms-and-conditions\n  cookie_policy: https://snov.io/cookie-policy\n  do_not_sell: published in site footer\nvulnerability_disclosure:\n  published: false\n  security_txt: false\n  bug_bounty: false\n  note: Probed 2026-08-13. No /.well-known/security.txt on snov.io or api.snov.io (both HTTP 404), no disclosure\n    or responsible-reporting page, and no HackerOne, Bugcrowd or Intigriti program. There is no published route\n    for a researcher to report a vulnerability other than the general contact form. No VulnerabilityDisclosure or\n    Security pointer is wired in apis.yml as a result.\nx-evidence:\n- fetched: '2026-08-13'\n  url: https://snov.io/security-center\n  http_status: 200\n- fetched: '2026-08-13'\n  url: https://snov.io/gdpr\n  http_status:\
  \ 200\n- fetched: '2026-08-13'\n  url: https://snov.io/privacy-policy\n  http_status: 200\n- fetched: '2026-08-13'\n  url: https://snov.io/.well-known/security.txt\n  http_status: 404\n- fetched: '2026-08-13'\n  url: https://api.snov.io/.well-known/security.txt\n  http_status: 404\ncertification_details:\n- name: GDPR\n  type: regulation\n  claimed: true\n  named_auditor: null\n  report_available: false\n  url: https://snov.io/gdpr\n  evidence: '\"Snov.io fully adheres to GDPR laws and regulations, meaning your personal data is safely stored and\n    processed.\" A dedicated GDPR page is published and returns HTTP 200.'\n- name: LOA (Letter of Authorization)\n  type: authorization\n  claimed: true\n  named_auditor: null\n  report_available: false\n  evidence: '\"LOA (Letter of Authorization) is a permission given to Snov.io to control and manage operations with\n    users'' data.\" Badge text on the page reads \"GDPR compliant • Encrypted • LOA certified\".'\n- name: CCPA / Do Not Sell\
  \ My Personal Information\n  type: regulation\n  claimed: partial\n  evidence: A \"Do Not Sell My Personal Information\" control is published in the site footer, which is a CCPA/CPRA\n    construct. Snov.io does not name CCPA explicitly.\n"
source_yaml_url: https://artifacts.apis.io/snov-io/security/snov-io-trust-center.yml
summary_line: GDPR, LOA (Letter of Authorization), CCPA / Do Not Sell My Personal Information
tags:
- Sales Automation
- Email Finder
- Email Verification
- Lead Generation
- Drip Campaigns
- CRM
- LinkedIn Automation
- Prospect Management
- Data Enrichment
- Cold Email
trust_url: ''
---
