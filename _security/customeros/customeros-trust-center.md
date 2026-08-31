---
api_specs:
- filename: customeros-graphql-api-openapi.yml
  format: yaml
  label: CustomerOS GraphQL API
  slug: customeros-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-graphql-api-openapi.yml
- filename: customeros-billing-api-api-openapi.yml
  format: yaml
  label: CustomerOS Billing API
  slug: customeros-billing-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-billing-api-api-openapi.yml
- filename: customeros-customerbase-api-api-openapi.yml
  format: yaml
  label: CustomerOS CustomerBASE API
  slug: customeros-customerbase-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-customerbase-api-api-openapi.yml
- filename: customeros-domains-api-openapi.yml
  format: yaml
  label: CustomerOS Domains API
  slug: customeros-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-domains-api-openapi.yml
- filename: customeros-email-verification-api-openapi.yml
  format: yaml
  label: CustomerOS Email Verification API
  slug: customeros-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-email-verification-api-openapi.yml
- filename: customeros-enrichment-api-api-openapi.yml
  format: yaml
  label: CustomerOS Enrichment API
  slug: customeros-enrichment-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-enrichment-api-api-openapi.yml
- filename: customeros-flows-api-openapi.yml
  format: yaml
  label: CustomerOS Flows API
  slug: customeros-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-flows-api-openapi.yml
- filename: customeros-ip-intelligence-api-openapi.yml
  format: yaml
  label: CustomerOS IP Intelligence API
  slug: customeros-ip-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-ip-intelligence-api-openapi.yml
- filename: customeros-mailboxes-api-openapi.yml
  format: yaml
  label: CustomerOS Mailboxes API
  slug: customeros-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-mailboxes-api-openapi.yml
- filename: customeros-outreach-api-openapi.yml
  format: yaml
  label: CustomerOS Outreach API
  slug: customeros-outreach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-outreach-api-openapi.yml
certifications:
- CASA Type 2
description: CustomerOS has no trust center in the usual sense — trust.customeros.ai and security.customeros.ai do not resolve, and customeros.ai/security and /trust return 404. What it does publish is a single Security & Compliance page inside the documentation, which names one real third-party certification and states a GDPR position. That page is the trust surface, so it is recorded as such.
kind: trust-center
layout: security
name: Customeros Trust Center
name_suffix: Trust Center
overview: CustomerOS maintains a public trust center documenting CASA Type 2 compliance.
provider_name: CustomerOS
provider_slug: customeros
slug: customeros-trust-center
source_filename: customeros-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://docs.customeros.ai/security-and-compliance\ndescription: >-\n  CustomerOS has no trust center in the usual sense — trust.customeros.ai and security.customeros.ai\n  do not resolve, and customeros.ai/security and /trust return 404. What it does publish is a single\n  Security & Compliance page inside the documentation, which names one real third-party certification\n  and states a GDPR position. That page is the trust surface, so it is recorded as such.\nurl: https://docs.customeros.ai/security-and-compliance\ndedicated_trust_center: false\ncertifications:\n- name: CASA Type 2\n  issuer: Google — Cloud Application Security Assessment\n  scope: >-\n    Audited because of the depth of the Google integrations; the certification includes code\n    vulnerability scanning.\n  recertification: annual\nregulatory:\n- {regime: GDPR, position: 'Fully compliant; data-removal requests handled in-workspace and company-wide.'}\n\
  - {regime: CCPA, position: 'Compliance asserted in customeros.ai/llms.txt and on the comparison pages.'}\naccess_management:\n- {method: Magic link, note: Email one-time login link. Default.}\n- {method: SSO, providers: [Google, Microsoft], note: 'Recommended; inherits the identity provider''s 2FA/biometrics. Enabled by support request.'}\n- {method: OpenID Connect, note: 'Customer-supplied IdP (Keycloak named as supported). Requires discovery URL, client id and client secret, configured by support.'}\ndata_processing:\n  dpa_url: https://customeros.ai/standard-agreement/dpa\n  statements:\n  - European-based company\n  - All data stored encrypted\n  - Third-party processors vetted for their own data-security policies and listed in the DPA\nnot_claimed: [SOC 2 Type I, SOC 2 Type II, ISO 27001, ISO 27017, ISO 27018, PCI DSS, HIPAA, FedRAMP, CSA STAR]\nevidence:\n- {url: 'https://docs.customeros.ai/security-and-compliance', status: 200, content_type: text/html, keywords: [security, compliance,\
  \ certifications, CASA Type 2, GDPR, encrypted]}\n- {url: 'https://docs.customeros.ai/security-and-compliance.md', status: 200, content_type: text/markdown, note: 'Markdown twin; text quoted above read from this copy.'}\nmisses:\n- {url: 'https://trust.customeros.ai/', status: 0, note: no DNS record}\n- {url: 'https://security.customeros.ai/', status: 0, note: no DNS record}\n- {url: 'https://customeros.ai/trust', status: 404}\n- {url: 'https://customeros.ai/security', status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/security/customeros-trust-center.yml
summary_line: CASA Type 2
tags:
- CRM
- Revenue
- Go-To-Market
- Lead Intelligence
- Visitor Identification
- Attribution
- Email Verification
- Enrichment
- GraphQL
- Open-Source
trust_url: https://docs.customeros.ai/security-and-compliance
---
