---
api_specs:
- filename: datavant-rest-api-openapi.yml
  format: yaml
  label: Datavant REST API
  slug: datavant-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-rest-api-openapi.yml
certifications:
- FedRAMP Moderate
- SOC 2 Type 2
- HIPAA
- FIPS 140-2
description: ''
kind: trust-center
layout: security
name: Datavant Trust Center
name_suffix: Trust Center
overview: Datavant maintains a public trust center documenting FedRAMP Moderate, SOC 2 Type 2, HIPAA, and FIPS 140-2 compliance.
provider_name: Datavant
provider_slug: datavant
slug: datavant-trust-center
source_filename: datavant-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nurl: https://trust.datavant.com/\nplatform: TrustShare (TrustCloud / Kintent)\nnote: >-\n  trust.datavant.com resolves and returns HTTP 200, but the page is a client-rendered\n  single-page app: the HTML shell contains only a loader, and every content path\n  (/home, /api/v1/company, /trustshare/program-content/*) returns the same shell. The\n  underlying TrustShare content API (backend.trustcloud.ai) answers 401 Unauthorized\n  without a token, so the certification list, policy documents and subprocessor register\n  cannot be read anonymously - most TrustShare tenants gate document download behind an\n  NDA click-through. The certifications recorded below are therefore taken from Datavant's\n  OWN first-party public statements rather than from the trust center itself, and each one\n  carries the URL it was read from. This is a real trust center whose contents are not\n  machine-readable.\ncertifications:\n  - name: FedRAMP\
  \ Moderate\n    status: authorized\n    type: Agency ATO\n    sponsor: National Center for Advancing Translational Sciences (NCATS), National Institutes of Health\n    date: '2022-12'\n    detail: 326 controls in place at FedRAMP Moderate.\n    source: https://www.datavant.com/hipaa-privacy/how-our-security-and-compliance-teams-approached-datavants-fedramp-authorization\n  - name: SOC 2 Type 2\n    status: attested\n    detail: >-\n      Named by Datavant as a pre-existing program at the time of the FedRAMP effort\n      (\"we went from having programs like SOC 2 - Type 2, where we had 50 security\n      controls in place, to FedRAMP Moderate\").\n    source: https://www.datavant.com/hipaa-privacy/how-our-security-and-compliance-teams-approached-datavants-fedramp-authorization\n  - name: HIPAA\n    status: program\n    detail: >-\n      HIPAA Expert Determination de-identification is a productised Datavant capability\n      (Datavant Connect - Privacy), and Datavant maintains a HIPAA privacy\
  \ content hub.\n    source: https://www.datavant.com/hipaa-privacy\n  - name: FIPS 140-2\n    status: referenced\n    detail: Cited as a cryptographic-module requirement met as part of the FedRAMP authorization.\n    source: https://www.datavant.com/hipaa-privacy/how-our-security-and-compliance-teams-approached-datavants-fedramp-authorization\nsecurity_investment:\n  amount_usd_per_year: 40000000\n  quote: '\"invest more than $40 million annually in security and compliance infrastructure\"'\n  source: https://www.datavant.com/about/privacy-compliance\nrelated_pages:\n  - url: https://www.datavant.com/about/privacy-compliance\n    title: Privacy and Compliance\n    http_status: 200\n  - url: https://www.datavant.com/hipaa-privacy\n    title: HIPAA Privacy hub\n    http_status: 200\n  - url: https://www.datavant.com/report-vulnerabilities\n    title: Report Software Vulnerabilities\n    http_status: 200\n  - url: https://www.datavant.com/international-privacy\n    title: International Privacy\n\
  \    http_status: 200\nevidence:\n  - source: https://trust.datavant.com/\n    http_status: 200\n    kind: trust-center\n    keywords: [trustshare, trust center]\n    note: JS-rendered shell; no certification text present in the served HTML.\n    fetched: '2026-08-14'\n  - source: https://backend.trustcloud.ai/trustshare/program-content/datavant\n    http_status: 401\n    kind: trust-center-api\n    note: '{\"error\":\"Unauthorized\",\"debug\":\"Missing authorization token.\"}'\n    fetched: '2026-08-14'\n  - source: https://www.datavant.com/hipaa-privacy/how-our-security-and-compliance-teams-approached-datavants-fedramp-authorization\n    http_status: 200\n    kind: first-party-blog\n    keywords: [fedramp moderate, agency ato, soc 2 type 2, fips 140-2]\n    fetched: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/security/datavant-trust-center.yml
summary_line: FedRAMP Moderate, SOC 2 Type 2, HIPAA, FIPS 140-2
tags:
- Healthcare
- United States
- Interoperability
- Health Data
- De-Identification
- Tokenization
- Real-World Data
- Record Retrieval
- Data Connectivity
- Life Sciences
- HIPAA
- Medical Records
- Release of Information
- Privacy
- Authentication
- Health Information Exchange
trust_url: https://trust.datavant.com/
---
