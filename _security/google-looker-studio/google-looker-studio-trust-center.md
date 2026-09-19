---
api_specs:
- filename: google-looker-studio-assets-search-api-openapi.yml
  format: yaml
  label: Google Looker Studio Assets:search API
  slug: google-looker-studio-assets-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/openapi/google-looker-studio-assets-search-api-openapi.yml
certification_count: 4
certifications:
- source
- service_row
- evidence
- named
description: ''
kind: trust-center
layout: security
name: Google Looker Studio Trust Center
name_suffix: Trust Center
overview: Google Looker Studio maintains a public trust center documenting source, service_row, evidence, and named compliance.
provider_name: Google Looker Studio
provider_slug: google-looker-studio
slug: google-looker-studio-trust-center
source_filename: google-looker-studio-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  https://cloud.google.com/security/compliance/services-in-scope (HTTP 200, page states\n  \"Last modified: July 16, 2026\"), https://cloud.google.com/trust-center (HTTP 200),\n  https://cloud.google.com/security/compliance/offerings (HTTP 200) and\n  https://docs.cloud.google.com/looker/docs/studio/security-and-compliance (HTTP 200) —\n  all fetched 2026-09-12.\nprovider: Google Looker Studio\nproviderId: google-looker-studio\ntrust_center:\n  url: https://cloud.google.com/trust-center\n  status: 200\n  scope: Google Cloud programme-level, covering Looker Studio as a listed in-scope service.\n  self_serve_document_access: false\n  note: >-\n    There is no Looker-Studio-specific trust portal. Assurance is inherited from Google Cloud's\n    programme. Certification reports (SOC, ISO) are obtained through Google Cloud, not downloaded\n    from a product page.\ncertifications:\n  source: https://cloud.google.com/security/compliance/services-in-scope\n\
  \  service_row: Looker Studio\n  evidence: >-\n    The services-in-scope table marks the \"Looker Studio\" row \"done\" in all four columns. The page\n    header reads: \"The following Services fall within the scope of one or more of: Google's ISO\n    27001 Certification, ISO 27017 Certification, ISO 27018 Certification, PCI DSS Certification,\n    SOC 1 Report, SOC 2 Report and SOC 3 Report and Penetration Testing Report.\"\n  named:\n  - id: iso-27001\n    name: ISO/IEC 27001\n    in_scope: true\n  - id: iso-27017\n    name: ISO/IEC 27017\n    in_scope: true\n  - id: iso-27018\n    name: ISO/IEC 27018\n    in_scope: true\n  - id: soc-1\n    name: SOC 1\n    in_scope: true\n  - id: soc-2\n    name: SOC 2\n    in_scope: true\n  - id: soc-3\n    name: SOC 3\n    in_scope: true\n  - id: pci-dss\n    name: PCI DSS\n    in_scope: true\n  - id: pentest\n    name: Independent penetration testing report\n    in_scope: true\nproduct_security_features:\n  source: https://docs.cloud.google.com/looker/docs/studio/security-and-compliance\n\
  \  tier: Data Studio Pro only\n  features:\n  - name: Customer-managed encryption keys (CMEK)\n    description: Use your own cryptographic keys to protect Data Studio Pro assets.\n  - name: Customer-managed storage\n    description: Store file uploads in your own Cloud Storage bucket and data extracts in your own BigQuery dataset.\n  - name: Data residency\n    description: Keep data physically within a geographical area.\n  note: >-\n    All three shipped together in the 2026-06-11 release notes entry and are explicitly Pro-only.\n    The no-cost tier gets none of them.\nnot_found:\n- FedRAMP status for the Looker Studio row was not asserted — the services-in-scope table this was read from covers ISO / SOC / PCI DSS / penetration testing only, and no FedRAMP row for this service was verified.\n- HIPAA BAA coverage for this service was not verified and is not claimed here.\ncross_links:\n  vulnerability_disclosure: security/google-looker-studio-vulnerability-disclosure.yml\n  domain_security:\
  \ security/google-looker-studio-domain-security.yml\n  conformance: conformance/google-looker-studio-conformance.yml\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/security/google-looker-studio-trust-center.yml
summary_line: source, service_row, evidence, named
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Looker
- Reporting
trust_url: ''
---
