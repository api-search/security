---
certifications:
- verified
- verified_note
- claimed_indirect
description: Chainalysis operates a dedicated public Trust Center on the Vanta platform. The page is live and provider-operated, but its contents are rendered client-side, so the specific certification list could not be read anonymously and is NOT asserted here.
kind: trust-center
layout: security
name: Chainalysis Trust Center
name_suffix: Trust Center
overview: Chainalysis maintains a public trust center documenting verified, verified_note, and claimed_indirect compliance.
provider_name: Chainalysis
provider_slug: chainalysis
slug: chainalysis-trust-center
source_filename: chainalysis-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://trust.chainalysis.com/\ndescription: >-\n  Chainalysis operates a dedicated public Trust Center on the Vanta platform. The page is\n  live and provider-operated, but its contents are rendered client-side, so the specific\n  certification list could not be read anonymously and is NOT asserted here.\ntrust_center:\n  present: true\n  url: https://trust.chainalysis.com/\n  http_status: 200\n  platform: Vanta\n  platform_evidence: >-\n    The page bootstraps from assets.vanta.com (signature-manifest.json, index-trust-report\n    bundles) and links document access through app.vanta.com/doc.\n  machine_readable: false\n  machine_readable_note: >-\n    The trust center is a client-rendered single-page app. /api/company, /api/v1/company,\n    /manifest.json and /documents all return HTTP 200 carrying the SPA shell rather than\n    JSON, and api.vanta.com/trust/chainalysis returns 401. No anonymous JSON surface\n    exposes the\
  \ control or certification list.\n  document_access: gated\n  document_access_note: >-\n    Vanta trust centers typically place audit reports behind an NDA / email request flow.\ncertifications:\n  verified: []\n  verified_note: >-\n    NO certification is asserted as verified. Nothing naming SOC 2, ISO 27001, PCI DSS,\n    HIPAA or FedRAMP was recoverable from any anonymously readable Chainalysis surface -\n    not from the trust center (client-rendered), and not from the company's own 675KB\n    llms.txt, which mentions neither SOC 2 nor ISO 27001 anywhere.\n  claimed_indirect:\n    - standard: SOC 2\n      source: https://jobs.ashbyhq.com/chainalysis-careers/da0b9540-9071-4c80-a1ee-a76d46d19c98\n      source_type: Chainalysis careers posting (InfoSec Analyst II, Trust)\n      confidence: low\n      note: >-\n        The role description says the team manages SOC 2 and ISO 27001 evidence collection\n        and control testing. That is a Chainalysis-authored source and is good reason\
  \ to\n        believe the certifications exist, but a job posting is NOT a published attestation\n        and is recorded here at low confidence only.\n    - standard: ISO/IEC 27001\n      source: https://jobs.ashbyhq.com/chainalysis-careers/da0b9540-9071-4c80-a1ee-a76d46d19c98\n      source_type: Chainalysis careers posting (InfoSec Analyst II, Trust)\n      confidence: low\nprivacy_and_data_protection:\n  published: true\n  documents:\n    - name: Privacy Policy\n      url: https://www.chainalysis.com/privacy-policy/\n      status: 200\n    - name: Data Processing Addendum\n      url: https://www.chainalysis.com/data-processing-addendum/\n      status: 200\n    - name: List of Sub-Processors\n      url: https://www.chainalysis.com/sub-processors-list/\n      status: 200\n    - name: EEA and UK Privacy Disclosures\n      url: https://www.chainalysis.com/eea-uk-privacy-disclosures/\n      status: 200\n    - name: California Privacy Disclosures\n      url: https://www.chainalysis.com/california-privacy-disclosures/\n\
  \      status: 200\n    - name: Acceptable Use Policy\n      url: https://www.chainalysis.com/acceptable-use-policy/\n      status: 200\n    - name: Transfer Impact Assessment White Paper\n      url: https://www.chainalysis.com/wp-content/uploads/2023/03/transfer-impact-assessment-white-paper-march-27-2023.pdf\n    - name: Global Code of Business Conduct and Ethics\n      url: https://www.chainalysis.com/wp-content/uploads/2025/09/chainalysis-global-code-of-conduct-09-25-release.pdf\n    - name: Legal Process Guidelines for Law Enforcement\n      url: https://www.chainalysis.com/wp-content/uploads/2026/02/legal-process-guidelines20260220docx.pdf\n  note: >-\n    A published DPA plus a maintained sub-processor list is a substantive, verifiable\n    compliance programme in its own right, independent of the unreadable trust center.\n    This - not the certification list - is what backs the Compliance pointer in apis.yml.\nevidence:\n  - url: https://trust.chainalysis.com/\n    status: 200\n\
  \  - url: https://api.vanta.com/trust/chainalysis\n    status: 401\n  - url: https://www.chainalysis.com/sub-processors-list/\n    status: 200\n  - url: https://www.chainalysis.com/data-processing-addendum/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainalysis/refs/heads/main/security/chainalysis-trust-center.yml
summary_line: verified, verified_note, claimed_indirect
tags:
- Compliance
- AML
- KYT
- Sanctions
- Investigations
- Blockchain Analytics
- Risk
- Crypto
trust_url: ''
---
