---
api_specs:
- filename: tradeshift-external-api-openapi.yml
  format: yaml
  label: Tradeshift External API
  slug: tradeshift-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/openapi/tradeshift-external-api-openapi.yml
- filename: tradeshift-mcp-bridge-openapi.yml
  format: yaml
  label: Tradeshift MCP Server
  slug: tradeshift-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/openapi/tradeshift-mcp-bridge-openapi.yml
certifications:
- SOC 1 Type II
- SOC 2 Type II
- ISAE 3402 Type II
- PCI DSS Level 1
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Tradeshift Trust Center
name_suffix: Trust Center
overview: Tradeshift maintains a public trust center documenting SOC 1 Type II, SOC 2 Type II, ISAE 3402 Type II, PCI DSS Level 1, and ISO 27001 compliance.
provider_name: Tradeshift
provider_slug: tradeshift
slug: tradeshift-trust-center
source_filename: tradeshift-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nsource: https://tradeshift.com/security/\nurl: https://tradeshift.com/security/\nkind: security-and-compliance-whitepaper\nnote: >-\n  Tradeshift does not run a hosted trust-center portal (trust.tradeshift.com does not resolve). It publishes a\n  security and compliance whitepaper page instead, which names its third-party audit standards explicitly. Audit\n  reports are described as available to customers on request, not published.\ncertifications:\n  - SOC 1 Type II\n  - SOC 2 Type II\n  - ISAE 3402 Type II\n  - PCI DSS Level 1\n  - ISO 27001\nquote: >-\n  \"Our rigorous and ever-expanding compliance program includes 3rd party audits that enable us to provide our\n  customers reports validating the security of the platform with standards such as SOC 1 Type II, SOC 2 Type II,\n  ISAE 3402 Type II, Payment Card Industry (PCI-DSS) Level 1 and ISO 27001.\"\ntopics_covered:\n  - Governance and risk assessment\n  - Access control\n\
  \  - Secure software development life cycle\n  - Data classification and data security\n  - Physical security (cloud provider certified to ISO 27001 and SOC 1/2)\n  - Configuration and patch management\n  - Vulnerability management and incident response\n  - Monitoring and logging\n  - Data backup and restore\n  - Business continuity and disaster recovery\n  - Awareness and training\n  - Compliance management\nregulatory:\n  - GDPR\n  - e-invoicing compliance across 69 countries\n  - French e-invoicing mandate — registered PDP (Plateforme de Dématérialisation Partenaire)\nprobes:\n  - url: https://trust.tradeshift.com/\n    result: NXDOMAIN\n  - url: https://tradeshift.com/trust/\n    http_status: 404\n  - url: https://tradeshift.com/security/\n    http_status: 200\nevidence:\n  - source: https://tradeshift.com/security/\n    keywords: [soc 1 type ii, soc 2 type ii, isae 3402 type ii, pci-dss level 1, iso 27001, gdpr]\nx-evidence:\n  fetched: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/security/tradeshift-trust-center.yml
summary_line: SOC 1 Type II, SOC 2 Type II, ISAE 3402 Type II, PCI DSS Level 1, ISO 27001
tags:
- e-invoicing
- accounts-payable
- ap-automation
- procure-to-pay
- supply-chain
- b2b-commerce
- invoicing
- ubl
- peppol
- e-invoicing-compliance
- supplier-network
- business-documents
- fintech
- mcp
- agent-native
trust_url: https://tradeshift.com/security/
---
