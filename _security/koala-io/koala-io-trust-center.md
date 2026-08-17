---
api_specs:
- filename: koala-io-accounts-api-openapi.yml
  format: yaml
  label: Koala Accounts API
  slug: koala-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-accounts-api-openapi.yml
- filename: koala-io-collection-api-openapi.yml
  format: yaml
  label: Koala Collection API
  slug: koala-io-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-collection-api-openapi.yml
- filename: koala-io-deletion-api-openapi.yml
  format: yaml
  label: Koala Deletion API
  slug: koala-io-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-deletion-api-openapi.yml
- filename: koala-io-sdk-api-openapi.yml
  format: yaml
  label: Koala SDK API
  slug: koala-io-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-sdk-api-openapi.yml
certifications:
- SOC 2 Type II
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Koala Io Trust Center
name_suffix: Trust Center
overview: Koala maintains a public trust center documenting SOC 2 Type II, GDPR, and CCPA compliance.
provider_name: Koala
provider_slug: koala-io
slug: koala-io-trust-center
source_filename: koala-io-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://getkoala.com/security\nurl: https://app.vanta.com/koala/trust/tzb87epi5imm1qbxktj0bn\nurl_status: 200\nurl_note: >-\n  Koala's trust center is hosted on Vanta and linked from https://getkoala.com/security.\n  Upgraded on 2026-08-13 from the previous pass, which recorded only the marketing\n  security page.\ncertifications:\n- name: SOC 2 Type II\n  status: maintained\n  quote: >-\n    \"Koala earned its first SOC 2 compliance certificate about six months after its\n    first line of code was written and maintains SOC 2 Type II.\"\n  evidence: https://getkoala.com/security\n- name: GDPR\n  status: compliant (self-attested)\n  quote: >-\n    \"Koala is compliant with the General Data Protection Regulation (GDPR) and\n    California Consumer Privacy Act (CCPA).\"\n  evidence: https://getkoala.com/security\n- name: CCPA\n  status: compliant (self-attested)\n  evidence: https://getkoala.com/security\nnot_claimed:\n\
  - ISO 27001\n- HIPAA\n- PCI DSS\n- FedRAMP\ncontrols_published:\n- name: Third-party penetration testing\n  cadence: annual\n- name: External code audits\n- name: SSO\n  detail: Google sign-in or magic links\n- name: SAML SSO\n  detail: via Okta, on the Business plan\n  docs: https://getkoala.com/docs/admin-guides/saml-sso\n- name: Password login can be disabled\ndata_processing:\n  dpa: available on request (custom DPA)\n  subprocessor_list_published: false\n  gdpr_erasure_api: https://getkoala.com/docs/developer-guides/gdpr-endpoint\n  gdpr_erasure_api_status: >-\n    Documented at https://app.getkoala.com/api/v1/deletion-requests, but that host\n    returned HTTP 530 (Cloudflare 1016, origin DNS failure) on 2026-08-13 — the\n    erasure channel is currently unreachable.\nevidence:\n- source: https://getkoala.com/security\n  status: 200\n  fetched: '2026-08-13'\n  keywords: [soc 2, soc 2 type ii, gdpr, ccpa, penetration testing, saml, sso, dpa]\n- source: https://app.vanta.com/koala/trust/tzb87epi5imm1qbxktj0bn\n\
  \  status: 200\n  fetched: '2026-08-13'\nlifecycle_warning: >-\n  Koala was acquired by Cursor and shuts down 2026-09-30. Certifications and the trust\n  center are published as of this probe but should not be relied on past that date.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/security/koala-io-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA
tags:
- Buyer Intent
- Visitor Identification
- De-anonymization
- Enrichment
- Go-to-Market
- Sales Intelligence
- B2B
trust_url: https://app.vanta.com/koala/trust/tzb87epi5imm1qbxktj0bn
---
