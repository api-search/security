---
api_specs:
- filename: jotform-folder-api-openapi.yml
  format: yaml
  label: Jotform Folder API
  slug: jotform-folder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-folder-api-openapi.yml
- filename: jotform-form-api-openapi.yml
  format: yaml
  label: Jotform Form API
  slug: jotform-form-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-form-api-openapi.yml
- filename: jotform-label-api-openapi.yml
  format: yaml
  label: Jotform Label API
  slug: jotform-label-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-label-api-openapi.yml
- filename: jotform-report-api-openapi.yml
  format: yaml
  label: Jotform Report API
  slug: jotform-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-report-api-openapi.yml
- filename: jotform-submission-api-openapi.yml
  format: yaml
  label: Jotform Submission API
  slug: jotform-submission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-submission-api-openapi.yml
- filename: jotform-system-api-openapi.yml
  format: yaml
  label: Jotform System API
  slug: jotform-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-system-api-openapi.yml
- filename: jotform-user-api-openapi.yml
  format: yaml
  label: Jotform User API
  slug: jotform-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-user-api-openapi.yml
- filename: jotform-webhook-api-openapi.yml
  format: yaml
  label: Jotform Webhook API
  slug: jotform-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-webhook-api-openapi.yml
certification_count: 8
certifications:
- PCI DSS Service Provider Level 1
- SOC 2 Type II (dedicated Enterprise environment)
- GDPR
- CCPA
- HIPAA (BAA)
- FERPA
- HECVAT
- StateRAMP Security Snapshot
description: ''
kind: trust-center
layout: security
name: Jotform Trust Center
name_suffix: Trust Center
overview: Jotform maintains a public trust center documenting PCI DSS Service Provider Level 1, SOC 2 Type II (dedicated Enterprise environment), GDPR, CCPA, HIPAA (BAA), FERPA, HECVAT, and StateRAMP Security Snapshot compliance.
provider_name: Jotform
provider_slug: jotform
slug: jotform-trust-center
source_filename: jotform-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://www.jotform.com/security/\n- https://www.jotform.com/enterprise/soc-2-compliance/\n- https://www.jotform.com/hipaa/baa/\n- https://www.jotform.com/enterprise/security/\nurl: https://www.jotform.com/security/\nhost: www.jotform.com\nplatform: self-hosted-or-unknown\nplatform_evidence: 'No dedicated trust portal: https://trust.jotform.com/ redirects to the homepage and /trust/\n  -> 404. The /security/ page carries the certification and compliance claims, security practices (encryption, backups,\n  audits, bug bounty) and links to SOC 2, FERPA, HECVAT, data residency and SSO pages.'\ncompany: Jotform\nwebsite: https://www.jotform.com/\ncontact: https://www.jotform.com/vulnerability-disclosure-program/\ncertifications:\n- PCI DSS Service Provider Level 1\n- SOC 2 Type II (dedicated Enterprise environment)\n- GDPR\n- CCPA\n- HIPAA (BAA)\n- FERPA\n- HECVAT\n- StateRAMP Security Snapshot\nframeworks:\n- name: PCI DSS\n\
  \  source: https://www.jotform.com/security/\n- name: SOC 2\n  source: https://www.jotform.com/security/\n- name: GDPR\n  source: https://www.jotform.com/security/\n- name: CCPA\n  source: https://www.jotform.com/security/\n- name: HIPAA\n  source: https://www.jotform.com/security/\n- name: FERPA\n  source: https://www.jotform.com/security/\n- name: HECVAT\n  source: https://www.jotform.com/security/\n- name: StateRAMP\n  source: https://www.jotform.com/security/\nsubprocessors:\n- name: Amazon Web Services\n  purpose: Data storage -- Cloud Service Provider (IaaS/PaaS)\n  url: https://www.jotform.com/subprocessors/\n- name: Deepgram\n  purpose: AI voice technology -- AI / Voice Processing\n  url: https://www.jotform.com/subprocessors/\n- name: ElevenLabs\n  purpose: AI voice technology -- AI / Voice Processing\n  url: https://www.jotform.com/subprocessors/\n- name: Google LLC / Google Cloud EMEA Limited / Google Australia Pty Ltd / Google Cloud Canada Corporation\n  purpose: Data storage,\
  \ AI, Google Workspace, Google Analytics -- Cloud Service Provider (IaaS/PaaS), Productivity\n    Suite, AI Platform, Analytics Tracking\n  url: https://www.jotform.com/subprocessors/\ndpa: https://www.jotform.com/dpa/\ninfrastructure_note: Our primary platform is Google Cloud, which complies with SSAE16 / ISAE 3402 Type II, SOC 1,\n  SOC 2, SOC 3, ISO 27001, ISO 27017 (Cloud Security), ISO 27018 (Cloud Privacy), and PCI DSS v3.2. (These are the\n  hosting provider's certifications, quoted as Jotform states them, not Jotform's own.)\nsecurity_practices:\n- 256 Bit SSL\n- Encrypted Forms (RSA 2048 at the user's computer)\n- Two-factor Authentication (2FA)\n- Single Sign-On (SSO, Enterprise)\n- EU Servers / local data residency\n- Backups (30 days in the cloud environment)\n- ASV scans for PCI, periodic penetration tests, bug bounty program\ncertification_evidence:\n- name: PCI DSS Service Provider Level 1\n  status: claimed\n  evidence: Jotform is PCI DSS Service Provider Level 1 compliant,\
  \ the highest security attainment you can have\n    as a business that collects payments from and integrates with credit cards.\n  source: https://www.jotform.com/security/\n- name: SOC 2 Type II (dedicated Enterprise environment)\n  status: claimed\n  evidence: Jotform Enterprise now offers a dedicated SOC 2 Type II-compliant environment that customers can purchase\n    access to.\n  source: https://www.jotform.com/enterprise/soc-2-compliance/\n- name: GDPR\n  status: claimed\n  evidence: Jotform is compliant with the European Union's General Data Protection Regulation (GDPR), which governs\n    businesses that collect personally-identifiable information from or on EU citizens.\n  source: https://www.jotform.com/security/\n- name: CCPA\n  status: claimed\n  evidence: Jotform is compliant with the California Consumer Privacy Act (CCPA), which, among other things, prohibits\n    the selling of personal information of California residents without their consent.\n  source: https://www.jotform.com/security/\n\
  - name: HIPAA (BAA)\n  status: offered\n  evidence: We offer a Business Associate Agreement (BAA) for HIPAA customers who operate in the USA and who have\n    enabled HIPAA compliance features in their account.\n  source: https://www.jotform.com/hipaa/baa/\n- name: FERPA\n  status: claimed\n  evidence: FERPA Compliance (listed; detail at https://www.jotform.com/enterprise/ferpa/)\n  source: https://www.jotform.com/security/\n- name: HECVAT\n  status: completed\n  evidence: Jotform has used the Higher Education Community Vendor Assessment Toolkit\n  source: https://www.jotform.com/security/\n- name: StateRAMP Security Snapshot\n  status: in-program\n  evidence: Jotform is currently in the security snapshot Program of StateRAMP.\n  source: https://www.jotform.com/security/\nsubprocessors_url: https://www.jotform.com/subprocessors/\nsubprocessor_count: null\nsubprocessor_note: the first four rows of the subprocessor table are listed; the page carries more rows and no last-updated\n  date\n"
source_yaml_url: https://artifacts.apis.io/jotform/security/jotform-trust-center.yml
summary_line: PCI DSS Service Provider Level 1, SOC 2 Type II (dedicated Enterprise environment), GDPR, CCPA, HIPAA (BAA), FERPA, HECVAT, StateRAMP Security Snapshot
tags:
- Forms
- Surveys
- No-Code
- Data Collection
- Workflows
- HIPAA
- EU
- MCP
- E-Signature
- Webhook
- Online Payments
trust_url: https://www.jotform.com/security/
---
