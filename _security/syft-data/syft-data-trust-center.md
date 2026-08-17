---
api_specs:
- filename: syft-data-export-api-openapi.yml
  format: yaml
  label: Syft Data Export API
  slug: syft-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-export-api-openapi.yml
- filename: syft-data-lookup-api-openapi.yml
  format: yaml
  label: Syft Data Lookup API
  slug: syft-data-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-lookup-api-openapi.yml
- filename: syft-data-events-api-openapi.yml
  format: yaml
  label: Syft Data Event Collection API
  slug: syft-data-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-events-api-openapi.yml
certifications:
- SOC 2 Type I
- SOC 2 Type II
- Penetration Testing
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Syft Data Trust Center
name_suffix: Trust Center
overview: Syft Data maintains a public trust center documenting SOC 2 Type I, SOC 2 Type II, Penetration Testing, and ISO 27001 compliance.
provider_name: Syft Data
provider_slug: syft-data
slug: syft-data-trust-center
source_filename: syft-data-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://trust.syftdata.com (probed) and https://www.syftdata.com/dpa (contractual commitments)\nsummary: >-\n  Syft Data operates a trust center at trust.syftdata.com (\"Trust Vault\"), named\n  in its DPA as both the Security Policy location and the list of Approved\n  Subprocessors. The page returns HTTP 200 but is a JS-rendered Next.js app that\n  serves no readable content to an anonymous client, so the certifications below\n  are read from the DPA's own text rather than from the trust center itself.\ntrust_center:\n  url: https://trust.syftdata.com\n  status: 200\n  readable_anonymously: false\n  platform: unknown (Next.js \"Trust Vault\"; no vendor attribution in the served HTML)\n  checked: '2026-08-13'\n  note: >-\n    Content is rendered client-side; a curl of the page yields only the heading\n    \"Trust Vault\". Document access almost certainly requires a request/NDA flow.\ncertifications:\n  - name: SOC 2 Type I\n\
  \    status: committed\n    evidence: >-\n      DPA Cover Page — \"Provider will maintain annually updated reports or annual\n      certifications of compliance with the following: SOC 2 Type I\".\n    source: https://www.syftdata.com/dpa\n  - name: SOC 2 Type II\n    status: committed\n    evidence: >-\n      DPA Cover Page — same clause names SOC 2 Type II among the annually\n      maintained reports/certifications.\n    source: https://www.syftdata.com/dpa\n  - name: Penetration Testing\n    status: committed\n    evidence: DPA Cover Page lists annual penetration testing alongside the SOC 2 reports.\n    source: https://www.syftdata.com/dpa\n  - name: ISO 27001\n    status: not-claimed\n    evidence: Not named anywhere in the DPA, terms, or public site.\nnote_on_status: >-\n  \"committed\" means the provider contractually undertakes to maintain the report\n  or certification; it is NOT the same as a published, dated attestation. No SOC 2\n  report date, auditor, or certificate number\
  \ is published anywhere public, and\n  the trust center does not expose one anonymously.\ncompliance:\n  - regime: GDPR\n    posture: DPA published with EEA Standard Contractual Clauses and the UK Addendum for international transfers.\n    source: https://www.syftdata.com/dpa\n  - regime: CCPA / CPRA\n    posture: >-\n      Syft Data, Inc. is designated a \"service provider\" under Cal. Civ. Code\n      § 1798.100 et seq; DPA restricts use of personal data to the business purpose.\n    source: https://www.syftdata.com/dpa\n  - regime: Fair Credit Reporting Act\n    posture: DPA disclaims use of the service as a consumer report / for FCRA-regulated purposes.\n    source: https://www.syftdata.com/dpa\n  - regime: IAB TCF v2\n    posture: >-\n      Tracking tag reads and respects the TCF v2 consent string when a TCF-enabled\n      CMP is present; documented opt-out initialization for custom banners.\n    source: https://docs.syftdata.com/implementation/devguide\nsubprocessors:\n  url: https://trust.syftdata.com\n\
  \  published_anonymously: false\n  note: DPA names trust.syftdata.com as the Approved Subprocessors list; not readable without JS/registration.\ndocuments:\n  - name: Data Processing Addendum\n    url: https://www.syftdata.com/dpa\n    last_updated: '2026-05-07'\n  - name: DPA Addendums\n    url: https://www.syftdata.com/dpa/addendums\n  - name: RB2B Addendum\n    url: https://www.syftdata.com/dpa/rb2b-addendum\n  - name: Terms of Service\n    url: https://www.syftdata.com/terms\n  - name: Privacy Policy\n    url: https://www.syftdata.com/privacy.html\nlegal_entity:\n  name: Syft Data, Inc.\n  address: 4101 Dublin Blvd Ste F #3123, Dublin, California 94568, United States\n  officer: Imran Patel, CEO\n  source: https://www.syftdata.com/dpa\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/security/syft-data-trust-center.yml
summary_line: SOC 2 Type I, SOC 2 Type II, Penetration Testing, ISO 27001
tags:
- Company
- Lead Intelligence
- Intent Data
- Website Visitor Identification
- Sales Intelligence
- Go-To-Market
- Analytics
- MCP
trust_url: ''
---
