---
api_specs:
- filename: immutable-activities-api-openapi.yml
  format: yaml
  label: Immutable Activities API
  slug: immutable-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-activities-api-openapi.yml
- filename: immutable-chains-api-openapi.yml
  format: yaml
  label: Immutable Chains API
  slug: immutable-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-chains-api-openapi.yml
- filename: immutable-collections-api-openapi.yml
  format: yaml
  label: Immutable Collections API
  slug: immutable-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-collections-api-openapi.yml
- filename: immutable-crafting-api-openapi.yml
  format: yaml
  label: Immutable Crafting API
  slug: immutable-crafting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-crafting-api-openapi.yml
- filename: immutable-data-api-openapi.yml
  format: yaml
  label: Immutable Data API
  slug: immutable-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-data-api-openapi.yml
- filename: immutable-ingest-api-openapi.yml
  format: yaml
  label: Immutable Ingest API
  slug: immutable-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-ingest-api-openapi.yml
- filename: immutable-metadata-api-openapi.yml
  format: yaml
  label: Immutable Metadata API
  slug: immutable-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-metadata-api-openapi.yml
- filename: immutable-metadata-search-api-openapi.yml
  format: yaml
  label: Immutable Metadata Search API
  slug: immutable-metadata-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-metadata-search-api-openapi.yml
- filename: immutable-nft-owners-api-openapi.yml
  format: yaml
  label: Immutable nft owners API
  slug: immutable-nft-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-nft-owners-api-openapi.yml
- filename: immutable-nfts-api-openapi.yml
  format: yaml
  label: Immutable Nfts API
  slug: immutable-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-nfts-api-openapi.yml
- filename: immutable-orders-api-openapi.yml
  format: yaml
  label: Immutable Orders API
  slug: immutable-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-orders-api-openapi.yml
- filename: immutable-passport-api-openapi.yml
  format: yaml
  label: Immutable Passport API
  slug: immutable-passport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-passport-api-openapi.yml
- filename: immutable-passport-profile-api-openapi.yml
  format: yaml
  label: Immutable passport profile API
  slug: immutable-passport-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-passport-profile-api-openapi.yml
- filename: immutable-pricing-api-openapi.yml
  format: yaml
  label: Immutable Pricing API
  slug: immutable-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-pricing-api-openapi.yml
- filename: immutable-tokens-api-openapi.yml
  format: yaml
  label: Immutable Tokens API
  slug: immutable-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-tokens-api-openapi.yml
- filename: immutable-tracking-consent-api-openapi.yml
  format: yaml
  label: Immutable Tracking Consent API
  slug: immutable-tracking-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-tracking-consent-api-openapi.yml
certifications:
- named
- note
description: ''
kind: trust-center
layout: security
name: Immutable Trust Center
name_suffix: Trust Center
overview: Immutable maintains a public trust center documenting named and note compliance.
provider_name: Immutable
provider_slug: immutable
slug: immutable-trust-center
source_filename: immutable-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://www.immutable.com/trust\ntrust_center:\n  url: https://www.immutable.com/trust\n  http_status: 200\n  hosted: first-party page on immutable.com\n  note: >-\n    Immutable publishes a Trust & Security page, not a hosted trust portal\n    (no Vanta/Drata/SafeBase/Conveyor instance was found). It is narrative rather\n    than evidentiary: it describes a control set but does NOT name a single\n    third-party certification or audit report, and offers no document-request\n    flow. Recorded honestly below — the absence of named certifications is the\n    finding, and it is why conformance/immutable-conformance.yml records\n    soc2/iso27001/pci/hipaa as conforms: false rather than unknown.\ncertifications:\n  named: []\n  note: >-\n    No SOC 2, ISO 27001, ISO 27701, PCI DSS, HIPAA or FedRAMP claim appears\n    anywhere on the Trust page. Searched the rendered text for each term; zero\n    matches. The only compliance regime\
  \ named is the GDPR, as a benchmark the\n    company says it builds against.\nregimes_claimed:\n- name: GDPR\n  claim: >-\n    \"We benchmark against the GDPR and the highest security standards.\" Products\n    (Passport, Audience) are described as built on a privacy-by-design framework,\n    with mapped data flows, vetted sub-processors, a collection statement shown\n    at sign-in, and controller/processor roles defined in commercial agreements.\n  evidence: https://www.immutable.com/trust\n  supporting_api_surface:\n  - operation: deleteAudienceData\n    detail: >-\n      DELETE /v1/audience/data in the Audience API accepts an erasure request for\n      an identity, resolves linked identities via alias mappings, and queues an\n      async erasure event — a machine-callable GDPR right-to-erasure path.\n  - operation: getTrackingConsent / updateTrackingConsent\n    detail: >-\n      GET and PUT /v1/audience/tracking-consent expose per-identity consent state\n      as an API, so consent\
  \ is enforceable at ingestion rather than only in a UI.\ncontrols_published:\n- Enterprise-grade infrastructure on AWS, defence-in-depth, high availability and redundancy\n- Encryption of sensitive data at rest and in transit\n- Tested incident response protocol with regulatory reporting commitments\n- Principle of least privilege with strong authentication for internal data access\n- User-facing processes to manage, export or delete personal data\n- 24/7 security operations centre with automated intrusion detection and threat intelligence\n- Third-party vendor and sub-processor security review\n- Public bug bounty programmes (Bugcrowd, Immunefi) and security@immutable.com\nlegal:\n  privacy_policy: https://www.immutable.com/legal/privacy-policy\n  terms_of_service: https://www.immutable.com/legal/terms-of-service\n  acceptable_use: https://www.immutable.com/legal/acceptable-use\n  collection_statement: https://www.immutable.com/legal/collection-statement\nx-evidence:\n  fetched: '2026-08-23'\n\
  \  url: https://www.immutable.com/trust\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/security/immutable-trust-center.yml
summary_line: named, note
tags:
- Company
- Gaming
- Blockchain
- NFT
- Web3
- Wallets
- Marketplace
- Analytics
- Attribution
- Customer Data Platform
- Authentication
- Developer Platform
trust_url: ''
---
