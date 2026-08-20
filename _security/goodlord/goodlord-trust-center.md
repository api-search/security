---
api_specs:
- filename: goodlord-referencing-api-openapi.json
  format: json
  label: Goodlord Referencing API
  slug: goodlord-referencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-referencing-api-openapi.json
- filename: goodlord-referencing-api-sandbox-openapi.json
  format: json
  label: Goodlord Referencing API (Sandbox)
  slug: goodlord-referencing-api-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-referencing-api-sandbox-openapi.json
- filename: goodlord-insurance-app-api-openapi.json
  format: json
  label: Goodlord Insurance App API
  slug: goodlord-insurance-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-insurance-app-api-openapi.json
certifications:
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Goodlord Trust Center
name_suffix: Trust Center
overview: Goodlord maintains a public trust center documenting ISO 27001 and GDPR compliance.
provider_name: Goodlord
provider_slug: goodlord
slug: goodlord-trust-center
source_filename: goodlord-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nprobe: true\nsource: https://trust.goodlord.com/\nurl: https://trust.goodlord.com/\nplatform: Sprinto\ntitle: Goodlord - Trust Center - Security & Privacy\ndiscoverable: false\ndiscoverability_note: >-\n  trust.goodlord.com is not linked from the marketing site navigation, the developer portal or\n  the sitemap (385 URLs, no trust or security entry). It was found by probing the conventional\n  trust.<domain> hostname. It is also fronted by CloudFront with aggressive bot filtering —\n  a default curl User-Agent gets HTTP 403 and only a plausible UA returns the page.\ncertifications:\n- name: ISO 27001\n  version: '2022'\n  status: Compliant\n  evidence: 'published on the trust center Compliances panel as \"ISO 27001 v2022 — Compliant\"'\n  certificate_public: false\n- name: GDPR\n  status: Compliant\n  evidence: published on the trust center Compliances panel\n  certificate_public: false\nnot_claimed: [SOC 2, PCI DSS, HIPAA, FedRAMP,\
  \ CSA STAR, Cyber Essentials, ISO 27017, ISO 27018]\nnot_claimed_note: >-\n  No SOC 2 claim appears anywhere in Goodlord's public surface, and no PCI DSS claim despite\n  Goodlord handling tenant rent and deposit payments (Modulr is named as the payments partner\n  in its client terms). Recorded as absent, not as failed.\nai_posture:\n  published: true\n  human_in_loop: 'Yes'\n  training_on_customer_data: 'No training'\n  data_retention: Contract-based\n  ai_trust_center: published (linked from the trust center as \"View AI Trust Center\")\n  note: >-\n    An explicit AI security posture panel is unusual for a UK PropTech company of this size and\n    is the most forward-looking thing on the page — it states that customer data is not used\n    for model training and that a human stays in the loop.\ncontrols:\n  published: true\n  count: 33\n  displayed: 12\n  categories: [Product security, Data security, Network security, App security, Corporate security]\n  examples:\n  - Service Identification\
  \ and Authentication\n  - Encrypting Data At Rest\n  - Data Backups\n  - Testing for Reliability and Integrity\n  - Limit Network Connections\n  - Anomalous Behavior\n  - Isolation of Information System Components\n  - Conspicuous Link To Privacy Notice\n  - Code of Business Conduct\n  - Roles & Responsibilities\n  - Competency Screening\nresources:\n  published: true\n  count: 43\n  access: gated behind \"Request access\"\n  examples:\n  - Communications & Network Security Policy\n  - Business Continuity Plan\n  - Asset Management Procedure\n  - Business Continuity & Disaster Recovery Policy\n  - Code of Business Conduct Policy\n  - HR Security Procedure\nsubprocessors:\n  published: true\n  count: 40\n  access: partially listed, remainder behind \"Request access\"\n  named:\n  - {name: AWS, category: Cloud Providers}\n  - {name: Supabase, category: IT infrastructure}\n  - {name: Credas, category: Others}\n  - {name: Konfir, category: Others}\n  - {name: Agiito, category: Payment Processing}\n\
  \  - {name: RocketReach, category: Sales}\n  note: >-\n    Credas (identity verification and AML) and Konfir (employment and income verification) are\n    the two that matter for the Referencing API — they are the third parties behind the checks\n    the API orchestrates.\naccess_gate:\n  request_access_required: true\n  what_is_gated: [certificates, full policy library, full subprocessor register]\n  what_is_open: [compliance claims, AI posture, control names, policy names, some subprocessor names]\nregulatory:\n  fca:\n    regulated: true\n    detail: >-\n      Goodlord operates as an Appointed Representative of Goodlord Protect Limited, authorised\n      and regulated by the UK Financial Conduct Authority for insurance distribution activities,\n      Firm Reference Number 836727. A permission for the rent-protection insurance product, not\n      an API or security certification.\nevidence:\n- source: https://trust.goodlord.com/\n  keywords: [iso 27001, trust center, gdpr]\n  observed:\
  \ '2026-07-26'\nrelated:\n  conformance: conformance/goodlord-conformance.yml\n  domain_security: security/goodlord-domain-security.yml\n  privacy_policy: https://www.goodlord.com/privacy-policy\n  terms: https://www.goodlord.com/terms\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/security/goodlord-trust-center.yml
summary_line: ISO 27001, GDPR
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Management
- Rentals
- Lettings
- Tenant Referencing
- Tenancy Management
- Insurance
- Payments
trust_url: https://trust.goodlord.com/
---
