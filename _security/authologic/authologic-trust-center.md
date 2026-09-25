---
api_specs:
- filename: authologic-advanced-api-openapi.yml
  format: yaml
  label: Authologic Advanced API
  slug: authologic-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-advanced-api-openapi.yml
- filename: authologic-affordability-assessment-api-openapi.yml
  format: yaml
  label: Authologic Affordability assessment API
  slug: authologic-affordability-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-affordability-assessment-api-openapi.yml
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-bank-api-openapi.yml
  format: yaml
  label: Authologic Bank API
  slug: authologic-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-bank-api-openapi.yml
- filename: authologic-conversation-api-openapi.yml
  format: yaml
  label: Authologic Conversation API
  slug: authologic-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-conversation-api-openapi.yml
- filename: authologic-database-verification-api-openapi.yml
  format: yaml
  label: Authologic Database Verification API
  slug: authologic-database-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-database-verification-api-openapi.yml
- filename: authologic-enterprise-integration-api-openapi.yml
  format: yaml
  label: Authologic Enterprise Integration API
  slug: authologic-enterprise-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-enterprise-integration-api-openapi.yml
- filename: authologic-metadata-api-openapi.yml
  format: yaml
  label: Authologic Metadata API
  slug: authologic-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-metadata-api-openapi.yml
certification_count: 3
certifications:
- ISO/IEC 27001
- ISO/IEC 22301
- eIDAS non-qualified trust service provider (EAA issuance)
description: 'Authologic does not run a conventional SaaS trust portal (no trust.authologic.com, no SOC 2 report room, no security.txt). What it publishes instead is an eIDAS trust-service repository: the policy, terms and status-list documents an EU Trust Service Provider is obliged to make public. That is a stronger and more specific disclosure than most vendor trust pages, and it is where the certification claims live.'
kind: trust-center
layout: security
name: Authologic Trust Center
name_suffix: Trust Center
overview: Authologic maintains a public trust center documenting ISO/IEC 27001, ISO/IEC 22301, and eIDAS non-qualified trust service provider (EAA issuance) compliance.
provider_name: Authologic
provider_slug: authologic
slug: authologic-trust-center
source_filename: authologic-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://authologic.com/ (Trust Service document column),\n  https://authologic.com/docs/trust-service/Trust-Service-Policy-for-Non-Qualified-EAA-Issuance.pdf,\n  https://authologic.com/docs/trust-service/TSP-TCs.pdf,\n  https://authologic.com/docs/trust-service/Authologic-Status-List.pdf,\n  https://authologic.com/docs/trust-service/Authologic-EAAP-Example.pdf,\n  https://authologic.com/docs/trust-service/Privacy-Policy.pdf\nspecification: API Commons Trust Center\nspecificationVersion: '0.1'\nprovider: Authologic\nproviderId: authologic\ndescription: >-\n  Authologic does not run a conventional SaaS trust portal (no trust.authologic.com, no SOC 2 report\n  room, no security.txt). What it publishes instead is an eIDAS trust-service repository: the policy,\n  terms and status-list documents an EU Trust Service Provider is obliged to make public. That is a\n  stronger and more specific disclosure than most vendor trust pages,\
  \ and it is where the certification\n  claims live.\ntrust_center:\n  present: true\n  type: eIDAS trust service repository\n  url: https://authologic.com/\n  location: >-\n    Linked from the marketing site footer as the \"Trust Service\" column; documents are served from\n    https://authologic.com/docs/trust-service/. All five were fetched with HTTP 200 on 2026-09-14.\n  availability: >-\n    The Trust Service Policy commits to a public repository on the official website accessible 24/7,\n    subject to reasonable maintenance windows.\n  legal_entity: Authologic Sp. z o.o.\n  contact: contact@authologic.com\ndocuments:\n  - name: Trust Service Policy for the Non-Qualified Electronic Attestation of Attributes Issuance Service\n    url: https://authologic.com/docs/trust-service/Trust-Service-Policy-for-Non-Qualified-EAA-Issuance.pdf\n    version: '1.0'\n    effective: '2026-07-13'\n    status: 200\n    content_type: application/pdf\n    bytes: 427849\n    note: >-\n      The governing\
  \ policy document. Names the eIDAS Regulation, the 2024-2025 Commission Implementing\n      Regulations (2024/2690, 2024/2977, 2024/2979, 2024/2982, 2025/848, 2025/2160), ETSI EN 319 401,\n      ETSI TS 119 471, TS 119 472-1 and TS 119 412-6, GDPR, and the ISO/IEC 27001 + 22301 certification\n      claim.\n  - name: Terms and Conditions for the Provision of the Service of Issuing Electronic Attestations of Attributes\n    url: https://authologic.com/docs/trust-service/TSP-TCs.pdf\n    status: 200\n    content_type: application/pdf\n    bytes: 662217\n  - name: Authologic Status List\n    url: https://authologic.com/docs/trust-service/Authologic-Status-List.pdf\n    status: 200\n    content_type: application/pdf\n    bytes: 58431\n    note: >-\n      The attestation revocation/status list. As of 2026-09-14 its entire content is \"Status list is\n      empty. No attestation has been issued yet.\" — the EAA issuance service is published and operable\n      but has not yet issued an attestation.\n\
  \  - name: Authologic EAAP Example\n    url: https://authologic.com/docs/trust-service/Authologic-EAAP-Example.pdf\n    status: 200\n    content_type: application/pdf\n    bytes: 109759\n  - name: Trust Service Privacy Policy\n    url: https://authologic.com/docs/trust-service/Privacy-Policy.pdf\n    status: 200\n    content_type: application/pdf\ncertifications:\n  - name: ISO/IEC 27001\n    scope: Information security management system covering the trust service\n    status: claimed-certified\n    evidence: >-\n      \"TSP has implemented an information security management system certified against ISO/IEC 27001 and\n      ISO/IEC 22301.\"\n    source: https://authologic.com/docs/trust-service/Trust-Service-Policy-for-Non-Qualified-EAA-Issuance.pdf\n    certificate_published: false\n  - name: ISO/IEC 22301\n    scope: Business continuity management covering the trust service\n    status: claimed-certified\n    evidence: Same statement as ISO/IEC 27001 above.\n    source: https://authologic.com/docs/trust-service/Trust-Service-Policy-for-Non-Qualified-EAA-Issuance.pdf\n\
  \    certificate_published: false\n  - name: eIDAS non-qualified trust service provider (EAA issuance)\n    scope: Electronic Attestation of Attributes issuance under Regulation (EU) No 910/2014 as amended\n    status: self-declared, policy published\n    source: https://authologic.com/docs/trust-service/Trust-Service-Policy-for-Non-Qualified-EAA-Issuance.pdf\nreferenced_standards:\n  - ETSI EN 319 401 v3.1.1\n  - ETSI TS 119 471 v1.1.1\n  - ETSI TS 119 472-1\n  - ETSI TS 119 412-6\n  - EN 50600\n  - ISO/IEC 18013-5 and 18013-7\n  - OpenID for Verifiable Credential Issuance\ngaps:\n  - No SOC 2 report, no HIPAA/PCI attestation, and no certificate PDFs — only the claim in prose.\n  - >-\n    No /.well-known/security.txt on any Authologic host, no published vulnerability-disclosure policy and\n    no bug-bounty program (HackerOne, Bugcrowd and Intigriti all return nothing for this domain).\n  - No public status page and no published SLA.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/security/authologic-trust-center.yml
summary_line: ISO/IEC 27001, ISO/IEC 22301, eIDAS non-qualified trust service provider (EAA issuance)
tags:
- AML
- Digital Identity
- eID
- Identity Verification
- KYB
- KYC
- Liveness Check
trust_url: ''
---
