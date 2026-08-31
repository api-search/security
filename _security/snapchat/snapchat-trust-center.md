---
api_specs:
- filename: snapchat-conversion-events-api-openapi.yml
  format: yaml
  label: Snapchat Conversion Events API
  slug: snapchat-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-conversion-events-api-openapi.yml
- filename: snapchat-oauth-api-openapi.yml
  format: yaml
  label: Snapchat OAuth API
  slug: snapchat-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-oauth-api-openapi.yml
- filename: snapchat-user-profile-api-openapi.yml
  format: yaml
  label: Snapchat User Profile API
  slug: snapchat-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-user-profile-api-openapi.yml
certifications: []
description: 'Snap Inc. publishes a trust / assurance profile at trust.snap.com covering application security, infrastructure, data protection, access control, incident response and business resiliency. What it does NOT publish is a certification: the profile''s own certificationSelections list is empty, and every attached document — including the Information Security Policy, the Security Incident Response Policy, the Resiliency and Crisis Management Policy, the Pentest Report summary, and the CAIQ and SIG Lite questionnaires — is marked isPublic false, i.e. released only on request. Recording this as an assurance surface, NOT as published compliance.'
kind: trust-center
layout: security
name: Snapchat Trust Center
name_suffix: Trust Center
overview: Snapchat maintains a public trust center covering its security and compliance posture.
provider_name: Snapchat
provider_slug: snapchat
slug: snapchat-trust-center
source_filename: snapchat-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://trust.snap.com\nprovider: Snapchat\nproviderId: snapchat\nhas_trust_center: true\nurl: https://trust.snap.com\nplatform: SecurityPal (Customer Assurance Profile)\nprofile_id: 3bb1e6c4-15a1-4476-8769-2c672d7e4de8\npublished: '2026-07-28'\nlast_updated: '2026-07-28'\nhttp_status: 200\ndescription: >-\n  Snap Inc. publishes a trust / assurance profile at trust.snap.com covering application security,\n  infrastructure, data protection, access control, incident response and business resiliency. What\n  it does NOT publish is a certification: the profile's own certificationSelections list is empty,\n  and every attached document — including the Information Security Policy, the Security Incident\n  Response Policy, the Resiliency and Crisis Management Policy, the Pentest Report summary, and the\n  CAIQ and SIG Lite questionnaires — is marked isPublic false, i.e. released only on request.\n  Recording this as an assurance surface,\
  \ NOT as published compliance.\ncertifications: []\ncertifications_note: >-\n  No SOC 2, SOC 1, ISO 27001, ISO 27701, PCI DSS, HIPAA, FedRAMP or CSA STAR attestation is named\n  anywhere on the profile, and the platform's certificationSelections array is literally empty.\n  Absence of a named certification here is a measurement, not an inference.\ndocuments:\n- title: Information Security Policy\n  public: false\n- title: Security Incident Response Policy\n  public: false\n- title: Resiliency and Crisis Management Policy\n  public: false\n- title: Pentest Report\n  description: Summary of Pentest Report\n  public: false\n- title: CAIQ\n  public: false\n  note: Cloud Security Alliance Consensus Assessments Initiative Questionnaire, request-gated.\n- title: SIG Lite\n  public: false\n  note: Shared Assessments Standardized Information Gathering questionnaire, request-gated.\n- title: Conversions API (CAPI) FAQs\n  public: false\n- title: Snap Pixel FAQs\n  public: false\n- title: Snap Audience\
  \ Match (SAM) FAQs\n  public: false\ncontrols_published:\n  application_security:\n  - Code Analysis\n  - Software Development Lifecycle\n  - Separate Production Environment\n  - Vulnerability Scanning\n  - Vulnerability and Patch Management\n  infrastructure:\n  - AWS\n  - GCP\n  - Virtual Private Cloud\n  - Firewall\n  - Web Application Firewall\n  - Anti-DDoS\n  - IDS/IPS\n  - Traffic Filtering\n  - Endpoint Detection and Response\n  data_protection:\n  - Encryption-at-rest\n  - Encryption-in-transit\n  - Disk Encryption\n  - Backups Enabled\n  - Data Erasure\n  - Data Breach Notifications\n  access_control:\n  - Multi-Factor Authentication\n  - Role-Based Access Control\n  - SSO Support\n  - Access Reviews\n  - Credential Management\n  - Password Security\n  resiliency:\n  - BC/DR\n  - Recovery Point Objective\n  - Recovery Time Objective\n  - Business Resiliency and Crisis Management Program\n  - Incident Response\n  - Incident Response Plan\n  organizational:\n  - HR Security\n \
  \ - Employee Training\n  - Employee Privacy Training\n  - Physical Security\n  - Cyber Insurance\n  - Asset Management Practices\n  - Audit Logging\n  - Logging\n  - Subprocessors\nrelated:\n  privacy_policy: https://snap.com/en-US/privacy/privacy-policy\n  transparency: https://snap.com/en-US/privacy/transparency\n  terms: https://snap.com/en-US/terms\n  developer_terms: https://www.snap.com/en-US/terms/developer\n  business_services_terms: https://www.snap.com/en-US/terms/business-services\n  business_tools_terms: https://www.snap.com/en-US/terms/snap-business-tools\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://trust.snap.com\n    http_status: 200\n  - url: https://snap.com/en-US/privacy/transparency\n    http_status: 200\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/security/snapchat-trust-center.yml
summary_line: trust center published
tags:
- Advertising
- AR
- Augmented Reality
- Marketing
- Messaging
- Social-Media
trust_url: https://trust.snap.com
---
