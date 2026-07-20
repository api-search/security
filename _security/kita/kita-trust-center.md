---
api_specs:
- filename: kita-capture-openapi.yml
  format: yaml
  label: Kita Capture API
  slug: capture
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-capture-openapi.yml
- filename: kita-underwriter-openapi.yml
  format: yaml
  label: Kita AI Underwriter API
  slug: underwriter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-underwriter-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Kita Trust Center
name_suffix: Trust Center
overview: Kita maintains a public trust center documenting SOC 2 Type II and ISO 27001 compliance.
provider_name: Kita
provider_slug: kita
slug: kita-trust-center
source_filename: kita-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.kita.ai/security\nurl: https://www.kita.ai/security\ndedicated_trust_portal: false\nnotes: 'Kita publishes a security and compliance page rather than a hosted trust portal.\n  trust.kita.ai does not resolve. Security questionnaire responses, penetration-test\n  summaries, architecture diagrams, the DPA and Standard Contractual Clauses are stated to be\n  available on request.'\ncertifications:\n- name: SOC 2 Type II\n  status: in-progress\n  detail: Active engagement for an independent audit of security, availability and\n    confidentiality controls. Engagement letter available on request. Not yet certified.\n- name: ISO 27001\n  status: in-progress\n  detail: Active engagement. Engagement letter available on request. Not yet certified.\nencryption:\n  at_rest: AES-256\n  in_transit: TLS 1.3\n  notes: Document data is encrypted before it reaches disk; keys are rotated automatically.\ndata_residency:\n\
  \  model: region-pinned per organization\n  regions:\n  - ap-southeast-1 (Singapore) — default for all organizations unless flagged for MX residency\n  - mx-central-1 (Mexico) — Mexican-residency customers (regulated)\n  active_markets:\n  - United States\n  - Mexico\n  - Singapore\n  - Indonesia\n  cross_region_replication: opt-in only\nlegal:\n  dpa: available on request\n  standard_contractual_clauses: available on request\nsubprocessors:\n  list: named list available on request\n  disclosed_categories:\n  - Vercel (hosting / edge delivery)\n  - Resend (email delivery)\n  - cloud infrastructure and AI/ML inference providers (customer-pinned)\n  - observability and support platforms\npenetration_testing:\n  cadence: annual, third-party, against production\n  between_cycles: continuous internal scanning\nenterprise_controls:\n- SSO/SAML\n- VPC and on-premises deployment options\nevidence:\n- source: https://www.kita.ai/security\n  keywords:\n  - soc 2\n  - iso 27001\n  - aes-256\n  -\
  \ tls 1.3\n  - data residency\n  - subprocessors\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/security/kita-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001
tags:
- Company
- Fintech
- Lending
- Underwriting
- Credit Scoring
- Document Intelligence
- Document Extraction
- Fraud Detection
- Artificial Intelligence
- Computer Vision
- Emerging Markets
- Loan Origination
trust_url: https://www.kita.ai/security
---
