---
api_specs:
- filename: snov-io-authentication-api-openapi.yml
  format: yaml
  label: Snov.io Authentication API
  slug: snov-io-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-authentication-api-openapi.yml
- filename: snov-io-campaigns-api-openapi.yml
  format: yaml
  label: Snov.io Campaigns API
  slug: snov-io-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-campaigns-api-openapi.yml
- filename: snov-io-crm-pipeline-api-openapi.yml
  format: yaml
  label: Snov.io CRM Pipeline API
  slug: snov-io-crm-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-crm-pipeline-api-openapi.yml
- filename: snov-io-domain-search-api-openapi.yml
  format: yaml
  label: Snov.io Domain Search API
  slug: snov-io-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-domain-search-api-openapi.yml
- filename: snov-io-email-accounts-api-openapi.yml
  format: yaml
  label: Snov.io Email Accounts API
  slug: snov-io-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-accounts-api-openapi.yml
- filename: snov-io-email-finder-api-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snov-io-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-finder-api-openapi.yml
- filename: snov-io-email-verification-api-openapi.yml
  format: yaml
  label: Snov.io Email Verification API
  slug: snov-io-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-verification-api-openapi.yml
- filename: snov-io-email-warm-up-api-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snov-io-email-warm-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-warm-up-api-openapi.yml
- filename: snov-io-prospects-api-openapi.yml
  format: yaml
  label: Snov.io Prospects API
  slug: snov-io-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-prospects-api-openapi.yml
- filename: snov-io-user-api-openapi.yml
  format: yaml
  label: Snov.io User API
  slug: snov-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-user-api-openapi.yml
- filename: snov-io-webhooks-api-openapi.yml
  format: yaml
  label: Snov.io Webhooks API
  slug: snov-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-webhooks-api-openapi.yml
certifications:
- GDPR
- LOA (Letter of Authorization)
- CCPA / Do Not Sell My Personal Information
description: Snov.io operates a public Security Center page describing its data-protection program. It is a narrative security page rather than a trust portal — there is no document request flow, no subprocessor list, no uptime or incident history, and no named third-party audit report. The only certifications named anywhere are GDPR adherence and an LOA (Letter of Authorization).
kind: trust-center
layout: security
name: Snov Io Trust Center
name_suffix: Trust Center
overview: Snov.io maintains a public trust center documenting GDPR, LOA (Letter of Authorization), and CCPA / Do Not Sell My Personal Information compliance.
provider_name: Snov.io
provider_slug: snov-io
slug: snov-io-trust-center
source_filename: snov-io-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "name: Snov.io Trust Center\nspecificationVersion: '0.1'\ngenerated: '2026-08-13'\nmethod: searched\nsource: https://snov.io/security-center\ndescription: >-\n  Snov.io operates a public Security Center page describing its data-protection program. It is a\n  narrative security page rather than a trust portal — there is no document request flow, no\n  subprocessor list, no uptime or incident history, and no named third-party audit report. The\n  only certifications named anywhere are GDPR adherence and an LOA (Letter of Authorization).\n\ntrust_center:\n  url: https://snov.io/security-center\n  http_status: 200\n  type: security-narrative-page\n  document_request_flow: false\n  subprocessor_list: false\n  status_history: false\n  pentest_report: false\n\ncertifications:\n  - name: GDPR\n    type: regulation\n    claimed: true\n    named_auditor: null\n    report_available: false\n    url: https://snov.io/gdpr\n    evidence: >-\n      \"Snov.io fully adheres to GDPR laws and regulations,\
  \ meaning your personal data is safely\n      stored and processed.\" A dedicated GDPR page is published and returns HTTP 200.\n  - name: LOA (Letter of Authorization)\n    type: authorization\n    claimed: true\n    named_auditor: null\n    report_available: false\n    evidence: >-\n      \"LOA (Letter of Authorization) is a permission given to Snov.io to control and manage\n      operations with users' data.\" Badge text on the page reads \"GDPR compliant • Encrypted •\n      LOA certified\".\n  - name: CCPA / Do Not Sell My Personal Information\n    type: regulation\n    claimed: partial\n    evidence: >-\n      A \"Do Not Sell My Personal Information\" control is published in the site footer, which is\n      a CCPA/CPRA construct. Snov.io does not name CCPA explicitly.\n\nnot_claimed:\n  frameworks:\n    - SOC 2 Type I\n    - SOC 2 Type II\n    - ISO/IEC 27001\n    - ISO/IEC 27701\n    - PCI DSS\n    - HIPAA\n    - FedRAMP\n    - CSA STAR\n  note: >-\n    None of these appear anywhere\
  \ on snov.io. Snov.io states that \"internal and external audits\n    take place regularly to test access control, risk possibility, information security, and IT\n    infrastructure\" but names no framework, no auditor and no report. For a platform whose\n    entire product is B2B contact data, the absence of a named third-party attestation is the\n    notable finding here.\n\ncontrols_published:\n  - name: Database protections\n    detail: >-\n      Encrypted passwords, intrusion detection systems, and a VPC with strict firewall settings.\n  - name: Integrations security\n    detail: >-\n      Integrated SaaS services are authorized with OAuth2 and their credentials are not stored.\n  - name: Encryption in transit and at rest\n    detail: Data is encrypted both when transmitted over public networks and when stored.\n  - name: Data recovery\n    detail: Regular backups with a maximum 24-hour RPO and a maximum 24-hour RTO.\n  - name: Internal and external audits\n    detail: >-\n      Regular\
  \ audits covering access control, risk, information security and IT infrastructure.\n      No framework or auditor named.\n\nlegal:\n  privacy_policy: https://snov.io/privacy-policy\n  gdpr: https://snov.io/gdpr\n  terms: https://snov.io/terms-and-conditions\n  cookie_policy: https://snov.io/cookie-policy\n  do_not_sell: published in site footer\n\nvulnerability_disclosure:\n  published: false\n  security_txt: false\n  bug_bounty: false\n  note: >-\n    Probed 2026-08-13. No /.well-known/security.txt on snov.io or api.snov.io (both HTTP 404),\n    no disclosure or responsible-reporting page, and no HackerOne, Bugcrowd or Intigriti\n    program. There is no published route for a researcher to report a vulnerability other than\n    the general contact form. No VulnerabilityDisclosure or Security pointer is wired in\n    apis.yml as a result.\n\nx-evidence:\n  - fetched: '2026-08-13'\n    url: https://snov.io/security-center\n    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://snov.io/gdpr\n\
  \    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://snov.io/privacy-policy\n    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://snov.io/.well-known/security.txt\n    http_status: 404\n  - fetched: '2026-08-13'\n    url: https://api.snov.io/.well-known/security.txt\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/security/snov-io-trust-center.yml
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
