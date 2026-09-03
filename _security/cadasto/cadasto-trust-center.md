---
api_specs:
- filename: cadasto-ehr-api-openapi.json
  format: json
  label: Cadasto EHR API
  slug: cadasto-ehr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-ehr-api-openapi.json
- filename: cadasto-query-api-openapi.json
  format: json
  label: Cadasto Query API (AQL)
  slug: cadasto-query-api-aql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-query-api-openapi.json
- filename: cadasto-definition-api-openapi.json
  format: json
  label: Cadasto Definition API
  slug: cadasto-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-definition-api-openapi.json
- filename: cadasto-demographic-api-openapi.json
  format: json
  label: Cadasto Demographic API
  slug: cadasto-demographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-demographic-api-openapi.json
- filename: cadasto-admin-api-openapi.json
  format: json
  label: Cadasto Admin API
  slug: cadasto-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-admin-api-openapi.json
- filename: cadasto-system-api-openapi.json
  format: json
  label: Cadasto System API
  slug: cadasto-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-system-api-openapi.json
- filename: cadasto-extra-api-openapi.json
  format: json
  label: Cadasto Additional API
  slug: cadasto-additional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-extra-api-openapi.json
- filename: cadasto-smart-on-openehr-openapi.json
  format: json
  label: Cadasto SMART on openEHR
  slug: cadasto-smart-on-openehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-smart-on-openehr-openapi.json
certifications:
- ISO 9001
- ISO/IEC 27001
- NEN 7510
description: Cadasto has NO dedicated trust center, security portal or compliance page. Its published compliance posture consists of three certification badges in the site footer, a privacy and cookie statement, and a security.txt contact. There is no downloadable SOC 2 report, no ISO certificate document, no subprocessor list, no DPA template and no uptime/status page on any anonymously reachable host.
kind: trust-center
layout: security
name: Cadasto Trust Center
name_suffix: Trust Center
overview: Cadasto maintains a public trust center documenting ISO 9001, ISO/IEC 27001, and NEN 7510 compliance.
provider_name: Cadasto
provider_slug: cadasto
slug: cadasto-trust-center
source_filename: cadasto-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  Certification badges published in the site footer of https://www.cadasto.com/ (HTTP 200,\n  fetched 2026-09-02), the openEHR conformance statement at\n  https://www.cadasto.com/wp-content/uploads/2026/06/Cadasto-CDR-openEHR-conformance-statement-June-2026.pdf\n  (HTTP 200), and https://www.cadasto.com/privacy-and-cookie-statement/ (HTTP 200).\ndescription: >-\n  Cadasto has NO dedicated trust center, security portal or compliance page. Its published\n  compliance posture consists of three certification badges in the site footer, a privacy and\n  cookie statement, and a security.txt contact. There is no downloadable SOC 2 report, no ISO\n  certificate document, no subprocessor list, no DPA template and no uptime/status page on any\n  anonymously reachable host.\ntrust_center_url: null\ncertifications:\n- name: ISO 9001\n  domain: Quality management systems\n  status: displayed\n  evidence: Badge image in the footer of\
  \ https://www.cadasto.com/\n  certificate_document: null\n  auditor: not published\n- name: ISO/IEC 27001\n  domain: Information security management systems\n  status: displayed\n  evidence: Badge image in the footer of https://www.cadasto.com/\n  certificate_document: null\n  auditor: not published\n- name: NEN 7510\n  domain: Information security in Dutch healthcare (the NL sector extension of ISO 27001)\n  status: displayed\n  evidence: Badge image in the footer of https://www.cadasto.com/\n  certificate_document: null\n  auditor: not published\nregulatory_context:\n  jurisdiction: Netherlands / European Union\n  regime: healthcare\n  applicable:\n    - GDPR / EU 2016/679 (Cadasto processes patient data on behalf of care providers)\n    - NEN 7510 (mandated information-security norm for Dutch healthcare)\n    - EHDS (European Health Data Space) — not referenced by Cadasto\n  privacy_policy: https://www.cadasto.com/privacy-and-cookie-statement/\n  dpa_published: false\n  subprocessors_published:\
  \ false\ndata_handling_claims:\n  - claim: The FHIR facade does not persist FHIR messages\n    detail: >-\n      \"Because it is a FHIR facade the FHIR messages are not stored\" — openEHR conformance\n      statement, Additional Cadasto CDR Features.\n  - claim: Deletes in the EHR API are logical, not physical\n    detail: >-\n      \"Deletions are logical — the data is marked as deleted but remains in the version history\n      for audit purposes\" — https://docs.cadasto.io/docs/quick-start. Physical deletion requires\n      the separate Admin API.\n  - claim: Credentials are isolated per environment\n    detail: >-\n      \"Credentials for development, acceptation, and production are separate. Treat each set\n      independently.\" — https://docs.cadasto.io/docs/faq.\ngaps:\n  - No trust center or security page exists; the certifications are asserted only by a footer image.\n  - No certificate numbers, issuing bodies or validity dates are published for any of the three certifications.\n\
  \  - No SOC 2, PCI DSS, HIPAA or FedRAMP claim is made (none is expected for a Dutch care-data processor).\n  - No status page, uptime history or SLA document was found on any Cadasto host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/security/cadasto-trust-center.yml
summary_line: ISO 9001, ISO/IEC 27001, NEN 7510
tags:
- Healthcare
- Health IT
- openEHR
- Electronic Health Records
- Clinical Data Repository
- Interoperability
- FHIR
- Vendor Neutral Archive
- Clinical Data
- AQL
- MCP
- Agent Skills
- Netherlands
trust_url: ''
---
