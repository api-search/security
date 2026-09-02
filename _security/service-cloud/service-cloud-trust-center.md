---
api_specs:
- filename: service-cloud-bot-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Bot API
  slug: service-cloud-bot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-bot-api-openapi.yml
- filename: service-cloud-health-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Health API
  slug: service-cloud-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-health-api-openapi.yml
- filename: service-cloud-versions-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Versions API
  slug: service-cloud-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-versions-api-openapi.yml
certifications:
- note
- observed
- unverified_in_this_pass
- unverified_note
description: ''
kind: trust-center
layout: security
name: Service Cloud Trust Center
name_suffix: Trust Center
overview: Salesforce Service Cloud APIs maintains a public trust center documenting note, observed, unverified_in_this_pass, and unverified_note compliance.
provider_name: Salesforce Service Cloud APIs
provider_slug: service-cloud
slug: service-cloud-trust-center
source_filename: service-cloud-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://trust.salesforce.com/, https://compliance.salesforce.com/,\n  https://security.salesforce.com/ and https://api.status.salesforce.com/v1/instances/status/preview\n  (all probed 2026-08-27)\ntrust_center:\n  published: true\n  url: https://trust.salesforce.com/\n  http_status: 200\n  title: Salesforce Trust\n  note: >-\n    Salesforce runs three separate public surfaces rather than one trust portal: Trust (live\n    availability and security status), Compliance (the certification document library) and\n    Security (programme and product-security guidance).\nsurfaces:\n  - name: Salesforce Trust\n    url: https://trust.salesforce.com/\n    http_status: 200\n    covers: [availability, incident history, maintenance, security advisories]\n  - name: Salesforce Compliance Site\n    url: https://compliance.salesforce.com/\n    http_status: 200\n    covers: [certifications, attestations, audit reports]\n    document_library:\
  \ https://compliance.salesforce.com/en/documents\n    library_size: >-\n      The document index reports \"Showing 1 to 10 of 505 entries\" — a 505-document library, gated\n      only by the site's client-side rendering, not by a login.\n  - name: Salesforce Security\n    url: https://security.salesforce.com/\n    http_status: 200\n    covers: [security programme, product security, customer guidance]\n  - name: Salesforce Status\n    url: https://status.salesforce.com/\n    api: https://api.status.salesforce.com/v1/instances/status/preview\n    http_status: 200\n    api_http_status: 200\n    covers: [per-instance live status, release version, maintenance windows]\ncertifications:\n  note: >-\n    Only certifications actually observed on the compliance site during this pass are listed.\n    The site renders its document index client-side, so this is a floor, not the full roster —\n    the library holds 505 documents. Nothing here is inferred from Salesforce's reputation.\n  observed:\n\
  \    - {name: IRAP, source: 'https://compliance.salesforce.com/en/documents'}\n    - {name: PCI DSS, source: 'https://compliance.salesforce.com/en/documents'}\n    - {name: ACSC Essential 8, source: 'https://compliance.salesforce.com/en/documents'}\n    - {name: ENS, source: 'https://compliance.salesforce.com/ (page text)'}\n  unverified_in_this_pass:\n    - SOC 1 / SOC 2 / SOC 3\n    - ISO 27001 / 27017 / 27018 / 27701\n    - HIPAA\n    - FedRAMP\n  unverified_note: >-\n    Widely reported for Salesforce but NOT read off the compliance site in this pass because the\n    document index is JS-rendered and only the first page resolved. Left unclaimed on purpose.\nprivacy:\n  url: https://www.salesforce.com/company/privacy/\n  http_status: 200\nlegal:\n  url: https://www.salesforce.com/company/legal/agreements/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/security/service-cloud-trust-center.yml
summary_line: note, observed, unverified_in_this_pass, unverified_note
tags:
- Cloud
- CRM
- Customer Service
- Enterprise
- Salesforce
- Support
trust_url: ''
---
