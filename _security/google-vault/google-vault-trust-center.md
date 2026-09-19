---
api_specs:
- filename: google-vault-exports-api-openapi.yml
  format: yaml
  label: Google Vault Exports API
  slug: google-vault-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-exports-api-openapi.yml
- filename: google-vault-heldaccounts-api-openapi.yml
  format: yaml
  label: Google Vault HeldAccounts API
  slug: google-vault-heldaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-heldaccounts-api-openapi.yml
- filename: google-vault-holds-api-openapi.yml
  format: yaml
  label: Google Vault Holds API
  slug: google-vault-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-holds-api-openapi.yml
- filename: google-vault-matters-api-openapi.yml
  format: yaml
  label: Google Vault Matters API
  slug: google-vault-matters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-matters-api-openapi.yml
- filename: google-vault-operations-api-openapi.yml
  format: yaml
  label: Google Vault Operations API
  slug: google-vault-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-operations-api-openapi.yml
- filename: google-vault-saved-queries-api-openapi.yml
  format: yaml
  label: Google Vault Saved Queries API
  slug: google-vault-saved-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-saved-queries-api-openapi.yml
certification_count: 8
certifications:
- FedRAMP
- CJIS
- HIPAA
- US Department of Defense requirements
- ISO/IEC 27001
- ISO/IEC 27017
- ISO/IEC 27018
- SOC 2
description: ''
kind: trust-center
layout: security
name: Google Vault Trust Center
name_suffix: Trust Center
overview: Google Vault maintains a public trust center documenting FedRAMP, CJIS, HIPAA, US Department of Defense requirements, ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, and SOC 2 compliance.
provider_name: Google Vault
provider_slug: google-vault
slug: google-vault-trust-center
source_filename: google-vault-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://workspace.google.com/security/\nreferences:\n  - https://workspace.google.com/security/\n  - https://cloud.google.com/security/compliance/offerings\n  - https://cloud.google.com/security/compliance/compliance-reports-manager\n  - https://safety.google/\nnote: >-\n  Google does not run a single-page trust centre for Vault. Trust material is split across the\n  Google Workspace security page (product-level controls and named regimes), Google Cloud's\n  compliance offerings directory (per-standard certificates), the Compliance Reports Manager\n  (where a customer downloads the actual audit reports), and safety.google (consumer-facing\n  privacy). Every URL below returned HTTP 200 on 2026-09-12. Vault itself is an eDiscovery and\n  legal-hold product, so it is usually the thing a customer buys IN ORDER TO comply — the\n  compliance posture recorded here is Google Workspace's, which is the service boundary the\n  Vault API\
  \ runs inside.\npages:\n  - kind: security-overview\n    url: https://workspace.google.com/security/\n    status: 200\n  - kind: compliance-directory\n    url: https://cloud.google.com/security/compliance/offerings\n    status: 200\n    caveat: The per-standard list is rendered client-side and is not machine-readable.\n  - kind: audit-reports\n    url: https://cloud.google.com/security/compliance/compliance-reports-manager\n    status: 200\n  - kind: privacy\n    url: https://safety.google/\n    status: 200\n  - kind: privacy-policy\n    url: https://policies.google.com/privacy\n    status: 200\ncertifications:\n  - name: FedRAMP\n    named_on: https://workspace.google.com/security/\n    detail_page: https://cloud.google.com/security/compliance/fedramp\n    detail_status: 200\n  - name: CJIS\n    named_on: https://workspace.google.com/security/\n  - name: HIPAA\n    named_on: https://workspace.google.com/security/\n    detail_page: https://cloud.google.com/security/compliance/hipaa-compliance\n\
  \    detail_status: 200\n  - name: US Department of Defense requirements\n    named_on: https://workspace.google.com/security/\n  - name: ISO/IEC 27001\n    named_on: https://cloud.google.com/security/compliance/iso-27001\n    detail_status: 200\n  - name: ISO/IEC 27017\n    named_on: https://cloud.google.com/security/compliance/iso-27017\n    detail_status: 200\n  - name: ISO/IEC 27018\n    named_on: https://cloud.google.com/security/compliance/iso-27018\n    detail_status: 200\n  - name: SOC 2\n    named_on: https://cloud.google.com/security/compliance/soc-2\n    detail_status: 200\ncertifications_note: >-\n  The four ISO/SOC entries are recorded from their own certificate pages on\n  cloud.google.com/security/compliance/, each fetched and confirmed HTTP 200 on 2026-09-12.\n  The Workspace security page names FedRAMP, CJIS, HIPAA, DoD and \"ISO/IEC standards\" in prose\n  without enumerating the ISO numbers, so the numbers come from the certificate pages, not\n  from an inference.\n\
  vulnerability_disclosure: security/google-vault-vulnerability-disclosure.yml\ndomain_security: security/google-vault-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/security/google-vault-trust-center.yml
summary_line: FedRAMP, CJIS, HIPAA, US Department of Defense requirements, ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, SOC 2
tags:
- eDiscovery
- Legal Hold
- Information Governance
- Compliance
- Archiving
- Retention
- Google Workspace
- Audit
trust_url: ''
---
