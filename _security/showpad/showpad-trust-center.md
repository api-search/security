---
api_specs:
- filename: showpad-v3-openapi-original.yml
  format: yaml
  label: Showpad Content API
  slug: showpad-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v3-openapi-original.yml
- filename: showpad-v4-openapi-original.yml
  format: yaml
  label: Showpad API v4
  slug: showpad-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v4-openapi-original.yml
- filename: showpad-v3-openapi-original.yml
  format: yaml
  label: Showpad User Management API
  slug: showpad-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v3-openapi-original.yml
certifications:
- SOC 2 Type II
- ISO 27001
- ISO 27701
description: ''
kind: trust-center
layout: security
name: Showpad Trust Center
name_suffix: Trust Center
overview: Showpad maintains a public trust center documenting SOC 2 Type II, ISO 27001, and ISO 27701 compliance.
provider_name: Showpad
provider_slug: showpad
slug: showpad-trust-center
source_filename: showpad-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nurl: https://trust.bigtincan.com/\ndomain_note: >-\n  Showpad's trust center is served on bigtincan.com, not showpad.com. This is a parent-brand\n  case confirmed from Showpad's own site: the \"Visit Trust Center\" button on\n  https://www.showpad.com/security links directly to https://trust.bigtincan.com/, and\n  Showpad's own navigation carries a \"Showpad x Bigtincan\" entry. The trust center names\n  Showpad explicitly as a covered brand alongside Bigtincan.\nsecurity_page: https://www.showpad.com/security\ncertifications:\n  - name: SOC 2 Type II\n    scope: Showpad and Bigtincan\n    source: https://trust.bigtincan.com/\n  - name: ISO 27001\n    scope: Showpad and Bigtincan\n    source: https://trust.bigtincan.com/\n  - name: ISO 27701\n    scope: Showpad\n    source: https://trust.bigtincan.com/\nquote: >-\n  \"Showpad currently maintains ISO27001 and ISO27701 certificates as well as SOC 2 Type II\n  reports. Bigtincan\
  \ currently maintains ISO27001 certificates and SOC 2 Type II Reports.\"\nencryption:\n  at_rest: AES 256\n  in_transit: TLS 1.2 or higher\n  source: https://trust.bigtincan.com/\nprivacy:\n  gdpr_page: https://www.showpad.com/gdpr\n  privacy_principles: https://www.showpad.com/privacy-principles\n  privacy_policy: https://www.showpad.com/privacy-policy\n  data_security_page: https://www.showpad.com/product/data-security-and-privacy\nidentity_controls:\n  sso: SAML 2.0 single sign-on\n  provisioning: SCIM provisioning to sync accounts from an identity provider\n  permissions: Granular permissions down to the file level; read-only licenses\nevidence:\n  - source: https://www.showpad.com/security\n    http_status: 200\n    kind: security-page\n    keywords: [trust center, responsible disclosure, sso, scim]\n  - source: https://trust.bigtincan.com/\n    http_status: 200\n    kind: trust-center\n    keywords: [soc 2, iso 27001, iso 27701, showpad, bigtincan]\nnot_claimed:\n  - HIPAA\n  - PCI\
  \ DSS\n  - FedRAMP\n  - IRAP\n  - CSA STAR\nnot_claimed_note: >-\n  ISAE 3402 Type I appears in older Showpad press releases but is NOT listed on the current\n  trust center, so it is not recorded as a live certification.\nsubdomain_false_positives:\n  - host: trust.showpad.com\n    result: HTTP 200 but redirects to a Showpad tenant login (/login?redirect=...) — a customer\n      instance, not a trust center.\n  - host: security.showpad.com\n    result: HTTP 200 but redirects to a Showpad tenant login — a customer instance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/security/showpad-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, ISO 27701
tags:
- Sales Enablement
- Sales Coaching
- Content Management
- Buyer Engagement
- Sales Analytics
- Training
- CRM Integration
- Digital Sales Rooms
- MCP
- SCIM
trust_url: https://trust.bigtincan.com/
---
