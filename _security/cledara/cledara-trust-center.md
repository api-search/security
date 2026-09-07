---
api_specs:
- filename: cledara-api-openapi.json
  format: json
  label: Cledara API
  slug: cledara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/openapi/cledara-api-openapi.json
certification_count: 2
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Cledara Trust Center
name_suffix: Trust Center
overview: Cledara maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: Cledara
provider_slug: cledara
slug: cledara-trust-center
source_filename: cledara-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nprobe: true\nsource: https://trust.cledara.com/\nurl: https://trust.cledara.com/\nprovider: Cledara\nproviderId: cledara\nplatform: Vanta\nplatform_evidence: >-\n  trust.cledara.com returns HTTP 200 titled \"Cledara Limited Trust Center\" and loads its\n  bundle from assets.vanta.com; the document request link points at app.vanta.com/doc.\n  Probed 2026-09-05.\nalso_published_at: https://www.cledara.com/security\ncertifications:\n  - name: SOC 2 Type II\n    holder: Cledara\n    quote: >-\n      \"Cledara is SOC 2 Type II certified, the industry-leading standard for security and\n      data protection.\"\n    source: https://www.cledara.com/security\n  - name: GDPR\n    holder: Cledara\n    quote: '\"Cledara is fully compliant with the GDPR legislation.\"'\n    source: https://www.cledara.com/security\nattributed_to_third_parties:\n  - name: 'ISO/IEC 27001:2013'\n    holder: Amazon Web Services (Cledara's hosting provider)\n    quote:\
  \ >-\n      AWS is \"accredited to ISO/IEC 27001:2013, SSAE 16 SOC 1, SOC 2 Type 2, PCI Level 1,\n      FISMA Moderate and SOX.\"\n    source: https://www.cledara.com/security\n    note: >-\n      CORRECTION (2026-09-05): earlier rounds of this artifact listed ISO 27001 and PCI as\n      Cledara certifications. They are AWS's, cited on Cledara's security page as\n      infrastructure assurance. Cledara does not claim ISO 27001 or PCI DSS for itself\n      anywhere we could find.\n  - name: PCI Level 1\n    holder: Amazon Web Services\n    source: https://www.cledara.com/security\nregulatory_authorisations:\n  - authority: UK Financial Conduct Authority\n    entity: Cledara Limited\n    status: EMD Agent\n    reference: '902831'\n    principal: Modulr FS Limited (Electronic Money Institution, FRN 900573)\n    source: https://www.cledara.com/security\n  - authority: De Nederlandsche Bank (DNB)\n    entity: Modulr Finance B.V.\n    status: Electronic Money Institution\n    reference: R182870\n\
  \    source: https://www.cledara.com/security\n  - regime: Electronic Money Regulations 2011 (UK)\n    subject: safeguarding of customer funds\n    source: https://www.cledara.com/security\n  - regime: Financial Supervision Act (Wft) (Netherlands)\n    subject: safeguarding of customer funds\n    source: https://www.cledara.com/security\ncard_scheme_membership:\n  - Mastercard\n  - Visa Europe\nsecurity_practices:\n  - Regular security reviews including active penetration testing\n  - Card tokenization\n  - AWS-hosted infrastructure\ndocuments:\n  request_required: true\n  mechanism: Vanta document request (https://app.vanta.com/doc)\n  note: Individual audit reports are not published anonymously; access is request-gated.\nevidence:\n  - source: https://trust.cledara.com/\n    http_status: 200\n    fetched: '2026-09-05'\n  - source: https://www.cledara.com/security\n    http_status: 200\n    fetched: '2026-09-05'\n    keywords:\n      - soc 2 type ii\n      - gdpr\n      - fca\n      -\
  \ electronic money\nmaintainers:\n  - FN: Kin Lane\n    email: kinlane@gmail.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/security/cledara-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Finance
- SaaS Management
- Software Spending
- Spend Management
- Subscription Management
- Virtual Cards
- Expense Management
- FinOps
- MCP
- Market Data
trust_url: https://trust.cledara.com/
---
