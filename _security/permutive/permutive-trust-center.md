---
api_specs:
- filename: permutive-contextual-api-openapi.yml
  format: yaml
  label: Permutive Contextual API
  slug: permutive-contextual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-contextual-api-openapi.yml
- filename: permutive-api-version-1-api-openapi.yml
  format: yaml
  label: Permutive API version 1 API
  slug: permutive-api-version-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-api-version-1-api-openapi.yml
- filename: permutive-v1-api-openapi.yml
  format: yaml
  label: Permutive V1 API
  slug: permutive-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-v1-api-openapi.yml
- filename: permutive-v2-0-api-openapi.yml
  format: yaml
  label: Permutive V2.0 API
  slug: permutive-v2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-v2-0-api-openapi.yml
- filename: permutive-v2-api-openapi.yml
  format: yaml
  label: Permutive V2 API
  slug: permutive-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-v2-api-openapi.yml
certifications:
- SOC 2 Type II
- SOC 3
description: ''
kind: trust-center
layout: security
name: Permutive Trust Center
name_suffix: Trust Center
overview: Permutive maintains a public trust center documenting SOC 2 Type II and SOC 3 compliance.
provider_name: Permutive
provider_slug: permutive
slug: permutive-trust-center
source_filename: permutive-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.permutive.com/\nsource: https://docs.permutive.com/governance/security\nnotes: >-\n  UPGRADE to the 2026-07-20 file, which recorded the Trust Center as live but\n  asserted no certifications because trust.permutive.com is a client-rendered\n  Vanta application that no crawler can read. The certifications are now\n  recorded because Permutive states them itself, in prose, on its own\n  developer-documentation security page — a source that is fetchable and\n  quotable — rather than being inferred from the Trust Center shell.\ncertifications:\n- {name: SOC 2 Type II, status: audited-annually, evidence: 'https://docs.permutive.com/governance/security'}\n- {name: SOC 3, status: published, note: 'SOC 3 reports available publicly', evidence: 'https://docs.permutive.com/governance/security'}\ncompliance_program:\n  attestations_via: https://trust.permutive.com\n  trust_center_contents: [compliance reports, penetration\
  \ testing documentation, security FAQs,\n    subprocessors, live compliance status]\n  privacy_regimes: [GDPR, ePrivacy Directive, CCPA]\n  data_role: >-\n    Permutive operates as a DATA PROCESSOR on behalf of customers (media\n    companies and advertisers) who are the data controllers, governed by a DPA.\nsecurity_posture:\n  encryption_at_rest: AES-256\n  encryption_in_transit: TLS 1.2 or higher\n  key_management: cloud KMS with separation of duties and auditing\n  tenant_isolation: application- and infrastructure-level access controls\n  sso: [SAML, OpenID Connect]\n  mfa: enforced via customer IdP for privileged and administrative access\n  rbac: true\n  just_in_time_privileged_access: true\n  vulnerability_management: continuous scanning across application code, cloud infrastructure and workloads\n  secure_sdlc: automated code analysis and dependency scanning in pipelines\n  penetration_testing: independent third-party, regular cadence\n  bug_bounty: private\nconsent_controls:\n\
  \  mechanisms: [consent-by-token, consent-by-default, opt-out]\n  source: https://docs.permutive.com/governance/consent\n  note: >-\n    Relevant to an advertising-data platform: the SDK can be configured with\n    `consentRequired: true` so no user data is collected until a consent token\n    is supplied. The CCS API has NO server-side consent gate — Permutive\n    documents that the caller is responsible for enforcing consent before\n    sending events.\nevidence:\n- {source: 'https://docs.permutive.com/governance/security', kind: security-practices-page,\n   http_status: 200, keywords: ['SOC 2 Type II', 'SOC 3', 'penetration testing', 'AES-256',\n     'TLS 1.2', 'SAML', 'OpenID Connect'], fetched: '2026-08-13'}\n- {source: 'https://trust.permutive.com/', kind: trust-center, http_status: 200,\n   detail: 'Vanta-hosted; client-rendered, not machine-readable', fetched: '2026-08-13'}\n- {source: 'https://docs.permutive.com/governance/consent', kind: consent-documentation,\n   http_status:\
  \ 200, fetched: '2026-08-13'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/security/permutive-trust-center.yml
summary_line: SOC 2 Type II, SOC 3
tags:
- Company
- Publishing
- Advertising
- AdTech
- MarTech
- Audience
- Data Collaboration
- Data Management Platform
- Contextual
- Identity
- Segmentation
- Agents
trust_url: https://trust.permutive.com/
---
