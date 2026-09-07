---
api_specs:
- filename: postman-collection
  format: yaml
  label: Cloudability API v3
  slug: api-v3
  spec_type: Postman
  url: https://github.com/IBM/Apptio-Tools/tree/main/cloudability/postman-collection
certification_count: 7
certifications:
- SOC 2 Type II
- ISO/IEC 27001:2013
- FedRAMP
- Cloud Security Alliance STAR Level One
- EU GDPR
- CCPA
- EU-US Privacy Shield
description: Apptio (IBM) publishes a Trusted Platform page carrying named third-party attestations for the cloud services that host Cloudability, with the attestation documents themselves downloadable as PDFs from the same domain.
kind: trust-center
layout: security
name: Cloudability Trust Center
name_suffix: Trust Center
overview: Cloudability maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001:2013, FedRAMP, Cloud Security Alliance STAR Level One, EU GDPR, CCPA, and EU-US Privacy Shield compliance.
provider_name: Cloudability
provider_slug: cloudability
slug: cloudability-trust-center
source_filename: cloudability-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "specification: API Commons Trust Center\nspecificationVersion: '0.1'\nprovider: Cloudability\nproviderId: cloudability\ngenerated: '2026-09-05'\nmodified: '2026-09-05'\nmethod: searched\nsource: https://www.apptio.com/company/trust/ — fetched 2026-09-05, HTTP 200.\ndescription: >-\n  Apptio (IBM) publishes a Trusted Platform page carrying named third-party\n  attestations for the cloud services that host Cloudability, with the\n  attestation documents themselves downloadable as PDFs from the same domain.\ntrust_center:\n  url: https://www.apptio.com/company/trust/\n  http_status: 200\n  self_serve: false\n  note: >-\n    A static marketing/compliance page with direct PDF links, not a gated trust\n    portal (no Vanta/Drata/SafeBase request flow). The SOC 3 report and the ISO\n    27001 certificate are downloadable without a login; the SOC 2 Type II report\n    itself is not published.\ncertifications:\n  - name: SOC 2 Type II\n    status: attested\n    evidence: https://www.apptio.com/company/trust/\n\
  \    document: https://www.apptio.com/wp-content/uploads/apptio-soc3-report.pdf\n    document_status: 200\n    document_type: application/pdf\n    note: >-\n      The public artifact is the SOC 3 report; the SOC 2 Type II report is\n      referenced on the page but is not publicly downloadable.\n  - name: ISO/IEC 27001:2013\n    status: certified\n    evidence: https://www.apptio.com/company/trust/\n    document: https://www.apptio.com/wp-content/uploads/apptio-inc-iso-27001-certificate.pdf\n    document_status: 200\n    document_type: application/pdf\n  - name: FedRAMP\n    status: authorized\n    evidence: https://www.apptio.com/fedramp/\n    document_status: 200\n    note: >-\n      Applies to the US Government offering; the corresponding API host is\n      api.usgov.cloudability.com, which IBM documents as not supporting\n      Cloudability API keys (apptio-opentoken only).\n  - name: Cloud Security Alliance STAR Level One\n    status: self-assessed\n    evidence: https://www.apptio.com/company/trust/\n\
  \    registry: https://cloudsecurityalliance.org/star/#_registry\n    note: CSA CAIQ / Cloud Controls Matrix response.\n  - name: EU GDPR\n    status: compliance-claimed\n    evidence: https://www.apptio.com/company/data-privacy/\n  - name: CCPA\n    status: compliance-claimed\n    evidence: https://www.apptio.com/company/trust/\n  - name: EU-US Privacy Shield\n    status: legacy\n    evidence: https://www.apptio.com/company/trust/\n    note: >-\n      Still listed on the Apptio trust page although the Privacy Shield framework\n      was invalidated by Schrems II in 2020 and superseded by the EU-US Data\n      Privacy Framework. Recorded verbatim as published; flagged as stale.\nsecurity_contact: infosec@apptio.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudability/refs/heads/main/security/cloudability-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001:2013, FedRAMP, Cloud Security Alliance STAR Level One, EU GDPR, CCPA, EU-US Privacy Shield
tags:
- Cloud Cost Management
- Cost Optimization
- FinOps
- Multi-Cloud
- Recommendations
- Reporting
trust_url: ''
---
