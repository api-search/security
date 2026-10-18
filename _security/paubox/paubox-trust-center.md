---
api_specs:
- filename: paubox-analytics-api-openapi.yml
  format: yaml
  label: Paubox Analytics API
  slug: paubox-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-analytics-api-openapi.yml
- filename: paubox-campaign-mailings-api-openapi.yml
  format: yaml
  label: Paubox Campaign Mailings API
  slug: paubox-campaign-mailings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-campaign-mailings-api-openapi.yml
- filename: paubox-drip-campaigns-api-openapi.yml
  format: yaml
  label: Paubox Drip Campaigns API
  slug: paubox-drip-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-drip-campaigns-api-openapi.yml
- filename: paubox-dynamic-templates-api-openapi.yml
  format: yaml
  label: Paubox Dynamic Templates API
  slug: paubox-dynamic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-dynamic-templates-api-openapi.yml
- filename: paubox-form-management-api-openapi.yml
  format: yaml
  label: Paubox Form management API
  slug: paubox-form-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-form-management-api-openapi.yml
- filename: paubox-forms-api-openapi.yml
  format: yaml
  label: Paubox Forms API
  slug: paubox-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-forms-api-openapi.yml
- filename: paubox-messages-api-openapi.yml
  format: yaml
  label: Paubox Messages API
  slug: paubox-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-messages-api-openapi.yml
- filename: paubox-submissions-api-openapi.yml
  format: yaml
  label: Paubox Submissions API
  slug: paubox-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-submissions-api-openapi.yml
- filename: paubox-subscribers-api-openapi.yml
  format: yaml
  label: Paubox Subscribers API
  slug: paubox-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-subscribers-api-openapi.yml
- filename: paubox-subscription-lists-api-openapi.yml
  format: yaml
  label: Paubox Subscription Lists API
  slug: paubox-subscription-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-subscription-lists-api-openapi.yml
- filename: paubox-subscriptions-api-openapi.yml
  format: yaml
  label: Paubox Subscriptions API
  slug: paubox-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-subscriptions-api-openapi.yml
- filename: paubox-tracking-links-api-openapi.yml
  format: yaml
  label: Paubox Tracking Links API
  slug: paubox-tracking-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-tracking-links-api-openapi.yml
certification_count: 2
certifications:
- HITRUST
- HIPAA / HITECH business associate
description: 'Paubox publishes a security-information page rather than a dedicated trust center. trust.paubox.com does not resolve (connection failed, no HTTP status). The page is a narrative compliance statement, not a certification portal: there is no document request flow, no downloadable report index and no subprocessor list linked from it.'
kind: trust-center
layout: security
name: Paubox Trust Center
name_suffix: Trust Center
overview: Paubox maintains a public trust center documenting HITRUST and HIPAA / HITECH business associate compliance.
provider_name: Paubox
provider_slug: paubox
slug: paubox-trust-center
source_filename: paubox-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.paubox.com/security\ndescription: 'Paubox publishes a security-information page rather than a dedicated trust center. trust.paubox.com\n  does not resolve (connection failed, no HTTP status). The page is a narrative compliance statement, not a certification\n  portal: there is no document request flow, no downloadable report index and no subprocessor list linked from it.'\nurl: https://www.paubox.com/security\nhttp_status: 200\nfetched: '2026-08-26'\ntrust_center_subdomain_probed: https://trust.paubox.com/\ntrust_center_subdomain_status: <no response> — connection failed, no HTTP status returned\ncertifications:\n- HITRUST\n- HIPAA / HITECH business associate\ncontrols_published:\n- Encryption of PHI in transit and at rest, per HHS guidance on rendering unsecured PHI unusable\n- AWS Key Management Service (KMS) for key management\n- TLS 1.2 and 1.3 only; SSL 2.0/3.0 and TLS 1.0/1.1 unsupported (NSA guidance cited)\n\
  - Two-factor authentication on Paubox accounts\n- U.S.-only data centers, encrypted at rest\n- 99.99% uptime commitment\ngaps:\n- No trust.paubox.com portal.\n- No downloadable audit report or report-request flow.\n- No subprocessor list linked from the security page.\n- No published vulnerability disclosure policy or bug bounty program (see paubox-vulnerability-disclosure).\ncertifications_detail:\n  paubox_own:\n  - name: HITRUST\n    scope: Stated as \"HITRUST certified\" for Paubox Email Suite on the Email API pricing page, and repeated in the\n      description of every first-party SDK repository under github.com/Paubox.\n    source: https://www.paubox.com/pricing/paubox-email-api\n  - name: HIPAA / HITECH business associate\n    scope: Paubox operates as a HIPAA business associate and includes a Business Associate Agreement with all accounts.\n      Third-party audits against HIPAA regulations are claimed on the pricing page.\n    source: https://www.paubox.com/security\n  inherited_from_infrastructure:\n\
  \    note: 'ATTRIBUTION MATTERS HERE. The security page attributes the following to Amazon Web Services, the platform\n      Paubox runs on — not to Paubox. Quoting the page: \"Paubox uses Amazon Web Services (AWS) as its HIPAA compliant\n      cloud platform. As such, the AWS platform provides industry recognized certifications and audits such as ISO\n      27001, FedRAMP, and the Service Organization Control Reports (SOC1, SOC2, and SOC3).\" No Paubox-issued SOC\n      2 report, ISO 27001 certificate or FedRAMP authorization was found on any public Paubox page.'\n    provider: Amazon Web Services\n    items:\n    - ISO 27001\n    - FedRAMP\n    - SOC 1\n    - SOC 2\n    - SOC 3\n    - GDPR DPA\n    - CISPE Code of Conduct\n    source: https://www.paubox.com/security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/security/paubox-trust-center.yml
summary_line: HITRUST, HIPAA / HITECH business associate
tags:
- Email
- HIPAA
- Healthcare
- Compliance
- Transactional Email
- Email Marketing
- Forms
- Security
- Encryption
- Messaging
- A2A
trust_url: https://www.paubox.com/security
---
