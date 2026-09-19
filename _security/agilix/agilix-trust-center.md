---
certification_count: 1
certifications:
- SOC 2
description: 'Agilix does not operate a hosted trust center — trust.agilix.com, security.agilix.com, /trust and /compliance were probed and none exists. What it publishes is a single security page on its own marketing site describing infrastructure controls, encryption, disaster recovery and a completed SOC 2 examination, with the report and the annual penetration-test results available on request rather than openly. For a K-12 vendor handling student data that is a thinner public posture than the sector norm, and the omissions are specific: FERPA is claimed only for BusyBee in the corporate llms.txt and nowhere on the security page, and COPPA, GDPR, ISO 27001 and the state student-data-privacy pledges are not addressed anywhere public.'
kind: trust-center
layout: security
name: Agilix Trust Center
name_suffix: Trust Center
overview: Agilix maintains a public trust center documenting SOC 2 compliance.
provider_name: Agilix
provider_slug: agilix
slug: agilix-trust-center
source_filename: agilix-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://www.agilix.com/security\nname: Agilix Labs security and compliance posture\ndescription: >-\n  Agilix does not operate a hosted trust center — trust.agilix.com, security.agilix.com,\n  /trust and /compliance were probed and none exists. What it publishes is a single security\n  page on its own marketing site describing infrastructure controls, encryption, disaster\n  recovery and a completed SOC 2 examination, with the report and the annual penetration-test\n  results available on request rather than openly. For a K-12 vendor handling student data\n  that is a thinner public posture than the sector norm, and the omissions are specific:\n  FERPA is claimed only for BusyBee in the corporate llms.txt and nowhere on the security\n  page, and COPPA, GDPR, ISO 27001 and the state student-data-privacy pledges are not\n  addressed anywhere public.\ntrust_center_url: null\ntrust_center_probes:\n- url: https://trust.agilix.com\n\
  \  result: NXDOMAIN\n- url: https://security.agilix.com\n  result: NXDOMAIN\n- url: https://www.agilix.com/trust\n  status: 404\n- url: https://www.agilix.com/compliance\n  status: 404\nsecurity_page: https://www.agilix.com/security\nsecurity_page_status: 200\ncertifications:\n- name: SOC 2\n  status: examination completed\n  scope: security, availability, processing integrity, confidentiality, privacy\n  report_public: false\n  request_via: security@agilix.com\n  evidence: https://www.agilix.com/security\n  quote: >-\n    \"Agilix Labs recently completed its SOC 2 examination, which evaluated our controls\n    relevant to security, availability, processing integrity, confidentiality, and privacy.\"\n  note: >-\n    No type (I or II), no audit period and no auditor are named on the public page, and no\n    date is given for \"recently\".\nclaims:\n- name: FERPA\n  scope: BusyBee (the AI teaching assistant)\n  evidence: https://www.agilix.com/llms.txt\n  quote: 'Runs on AWS; FERPA compliant;\
  \ student data is not used to train AI models.'\n  note: >-\n    Stated in the corporate llms.txt, not on the security page. No FERPA statement covering\n    Buzz, TutorKit, Publish Anywhere or Dawn was found.\n- name: WCAG accessibility\n  evidence: https://www.agilix.com/accessibility\n  scope: Buzz and Dawn\nnot_addressed:\n- ISO 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\n- GDPR\n- COPPA\n- Student Privacy Pledge / state student-data-privacy programs\ncontrols_published:\n- area: encryption\n  detail: PKCS #1 SHA-256 with 2048-bit RSA to secure data at rest and in transit.\n- area: identity\n  detail: Google authentication and single sign-on through SAML 2.0.\n- area: disaster recovery\n  detail: Annual testing of recovery processes with multi-location data replication.\n- area: infrastructure\n  detail: >-\n    Runs on AWS; AWS IAM, Shield, KMS, CloudWatch and CloudTrail are named. Agilix is an AWS\n    Public Sector Partner (https://www.agilix.com/partners/aws).\n- area: shared responsibility\n\
  \  detail: >-\n    The API documentation carries a Shared Security Responsibility section splitting security\n    OF Buzz (Agilix) from security IN Buzz (the customer's users, configuration, credentials\n    and data), plus a Tenant Isolation topic describing how multitenancy is enforced.\n  url: https://api.agilixbuzz.com/docs/entry/Concept/SharedResponsibility.md\n- area: audit trail\n  detail: >-\n    The Data Stream emits a full security audit event class — AuthLoginFailed, AuthMFAFailed,\n    AuthAccountLocked/Unlocked, AuthAdminAuthenticated, AuthAdminPasswordChanged,\n    AuthProxyLoginStarted/Failed, AuthPasswordRisk, DomainPermissionsCreated/Changed/Deleted,\n    OAuthClientKeyAdded/Removed — deliverable to the customer's own SIEM.\n  url: https://api.agilixbuzz.com/docs/entry/Concept/DataStream/Overview.md\n- area: password policy\n  detail: >-\n    Per-domain policy covering minimum length, character classes, entropy, breached-password\n    checking, expiry, lockout, stale accounts\
  \ and MFA enforcement, readable through\n    GetEffectivePasswordPolicy.\n  url: https://api.agilixbuzz.com/docs/entry/Schema/PasswordPolicy.md\ncontacts:\n- security@agilix.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilix/refs/heads/main/security/agilix-trust-center.yml
summary_line: SOC 2
tags:
- Company
- Education
- EdTech
- Learning Management System
- K-12
- Online Learning
- Tutoring
- Assessment
- LTI
- SCORM
- Artificial Intelligence
- Event
trust_url: ''
---
