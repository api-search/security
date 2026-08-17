---
api_specs:
- filename: microsoft-linkedin-adaccounts-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdAccounts API
  slug: microsoft-linkedin-adaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adaccounts-api-openapi.yml
- filename: microsoft-linkedin-adaccountusers-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdAccountUsers API
  slug: microsoft-linkedin-adaccountusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adaccountusers-api-openapi.yml
- filename: microsoft-linkedin-adcampaigngroups-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdCampaignGroups API
  slug: microsoft-linkedin-adcampaigngroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adcampaigngroups-api-openapi.yml
- filename: microsoft-linkedin-adcampaigns-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdCampaigns API
  slug: microsoft-linkedin-adcampaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adcampaigns-api-openapi.yml
- filename: microsoft-linkedin-adcreatives-api-openapi.yml
  format: yaml
  label: Microsoft LinkedIn AdCreatives API
  slug: microsoft-linkedin-adcreatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-adcreatives-api-openapi.yml
certifications:
- ISO/IEC 27001
- ISO/IEC 27018
- ISO 22301
- SOC 2 Type II
- PCI DSS
description: LinkedIn runs its own trust and compliance surface at security.linkedin.com, separate from the Microsoft Trust Center, plus a gated SafeBase-powered "Smart Trust Center" where enterprise customers request the actual audit reports.
kind: trust-center
layout: security
name: Microsoft Linkedin Trust Center
name_suffix: Trust Center
overview: Microsoft LinkedIn maintains a public trust center documenting ISO/IEC 27001, ISO/IEC 27018, ISO 22301, SOC 2 Type II, and PCI DSS compliance.
provider_name: Microsoft LinkedIn
provider_slug: microsoft-linkedin
slug: microsoft-linkedin-trust-center
source_filename: microsoft-linkedin-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://security.linkedin.com/trust-and-compliance\ndescription: >-\n  LinkedIn runs its own trust and compliance surface at security.linkedin.com, separate from the\n  Microsoft Trust Center, plus a gated SafeBase-powered \"Smart Trust Center\" where enterprise\n  customers request the actual audit reports.\ntrust_center:\n  public_page:\n    url: https://security.linkedin.com/trust-and-compliance\n    status: 200\n    probed: '2026-08-13'\n  gated_portal:\n    url: https://linkedin.safebase.us/\n    name: LinkedIn Smart Trust Center\n    platform: SafeBase\n    status: 403\n    probed: '2026-08-13'\n    access: account required; reports available to LinkedIn Enterprise customers\n    note: >-\n      Returns 403 to an anonymous probe. The certifications below are read from the public\n      security.linkedin.com page, not from behind the portal.\n  parent_company:\n    name: Microsoft Trust Center\n    url: https://www.microsoft.com/en-us/trust-center\n\
  \    note: LinkedIn maintains its own program; the Microsoft Trust Center is not the source of these claims.\ncertifications:\n  - name: ISO/IEC 27001\n    type: certification\n    scope: Information Security Management System — Learning, Marketing, Sales, Talent Solutions\n  - name: ISO/IEC 27018\n    type: certification\n    scope: PII protection for public cloud processors\n  - name: ISO 22301\n    type: certification\n    scope: Business Continuity Management Systems\n    validity: stated valid through May 2026\n  - name: SOC 2 Type II\n    type: audit report\n    scope: LinkedIn Learning, Marketing, Sales, Talent Solutions and the Glint platform\n    period: 12 months ending 2025-09-30\n    availability: request via the Smart Trust Center (enterprise customers)\n  - name: PCI DSS\n    type: compliance program\n    scope: Payment card processing\nprivacy_programs:\n  - GDPR\n  - CCPA\npolicies:\n  privacy_policy: https://www.linkedin.com/legal/privacy-policy\n  api_terms: https://www.linkedin.com/legal/l/api-terms-of-use\n\
  \  transparency_center: https://security.linkedin.com/trust-and-compliance\nevidence:\n  - url: https://security.linkedin.com/trust-and-compliance\n    status: 200\n    kind: public trust and compliance page naming each certification\n  - url: https://linkedin.safebase.us/\n    status: 403\n    kind: gated trust portal (SafeBase)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/security/microsoft-linkedin-trust-center.yml
summary_line: ISO/IEC 27001, ISO/IEC 27018, ISO 22301, SOC 2 Type II, PCI DSS
tags:
- Marketing
- Microsoft
- Professional Networking
- Recruiting
- Social Network
trust_url: ''
---
