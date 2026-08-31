---
api_specs:
- filename: blnkfinance-accounts-api-openapi.yml
  format: yaml
  label: Blnk Finance Accounts API
  slug: blnkfinance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-accounts-api-openapi.yml
- filename: blnkfinance-backup-api-openapi.yml
  format: yaml
  label: Blnk Finance Backup API
  slug: blnkfinance-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-backup-api-openapi.yml
- filename: blnkfinance-balance-monitors-api-openapi.yml
  format: yaml
  label: Blnk Finance Balance Monitors API
  slug: blnkfinance-balance-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-balance-monitors-api-openapi.yml
- filename: blnkfinance-balances-api-openapi.yml
  format: yaml
  label: Blnk Finance Balances API
  slug: blnkfinance-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-balances-api-openapi.yml
- filename: blnkfinance-identities-api-openapi.yml
  format: yaml
  label: Blnk Finance Identities API
  slug: blnkfinance-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-identities-api-openapi.yml
- filename: blnkfinance-ledgers-api-openapi.yml
  format: yaml
  label: Blnk Finance Ledgers API
  slug: blnkfinance-ledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-ledgers-api-openapi.yml
- filename: blnkfinance-refund-transaction-api-openapi.yml
  format: yaml
  label: Blnk Finance Refund Transaction API
  slug: blnkfinance-refund-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-refund-transaction-api-openapi.yml
- filename: blnkfinance-transactions-api-openapi.yml
  format: yaml
  label: Blnk Finance Transactions API
  slug: blnkfinance-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-transactions-api-openapi.yml
certifications:
- ISO/IEC 27001
- GDPR
- SOC 2
- PCI DSS
- HIPAA
description: ''
kind: trust-center
layout: security
name: Blnkfinance Trust Center
name_suffix: Trust Center
overview: Blnk Finance maintains a public trust center documenting ISO/IEC 27001, GDPR, SOC 2, PCI DSS, and HIPAA compliance.
provider_name: Blnk Finance
provider_slug: blnkfinance
slug: blnkfinance-trust-center
source_filename: blnkfinance-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://blnkfinance.com/security\nhttp_status: 200\ntrust_center:\n  published: true\n  url: https://blnkfinance.com/security\n  hosted_platform: null\n  note: >-\n    A first-party security page rather than a Vanta/Drata-style trust portal. There is no automated\n    document room; the ISO/IEC 27001 certificate is obtained by emailing sales@blnkfinance.com\n    (\"Request certification\").\ncertifications:\n- name: ISO/IEC 27001\n  status: certified\n  scope: Blnk's ISMS -- access control, incident handling, risk treatment, and the control review cycle\n  evidence_request: 'mailto:sales@blnkfinance.com?subject=Request ISO/IEC 27001 certification'\n  document_available: on request\n- name: GDPR\n  status: compliant\n  scope: Personal data processing; lawful basis, retention and subject-access requests\n  reference: https://blnkfinance.com/legal/privacy\n- name: SOC 2\n  status: not claimed\n- name: PCI DSS\n  status: not claimed\n\
  - name: HIPAA\n  status: not applicable\npractices:\n  compliance:\n  - Written policies for information security, access control, incident response and business continuity, reviewed on a set schedule\n  - Risk assessments tracked to remediation closure\n  - Annual role-based security training for all employees\n  - Background checks on all full-time hires, subject to local regulation\n  - Need-to-know data classification and access\n  infrastructure:\n  - Dedicated production hosts, separate from shared Sandbox capacity\n  - Customer-chosen deployment region\n  - Inbound traffic limited to a customer IP allowlist; Blnk egress IPs publishable for self-hosted firewalls\n  - Encryption at rest (AES-256-GCM for sensitive data including API keys) and TLS 1.2+ in transit\n  - SSO or MFA on critical services; periodic user access reviews\n  availability:\n  - 99.9% uptime SLA on the Production tier\n  - 30-minute SEV-1 response on the Production tier\n  - Auto-backups and multi-region support\
  \ on Production\nlegal:\n  privacy_policy: https://blnkfinance.com/legal/privacy\n  terms_of_service: https://blnkfinance.com/legal/terms\n  open_source_license: https://blnkfinance.com/legal/open-source-license\n  production_sla: https://blnkfinance.com/legal/deploy-sla\n  support_sla: https://blnkfinance.com/legal/support-sla\n  enterprise_license: https://blnkfinance.com/legal/license-sla\ncustomers_note: >-\n  The security page claims Blnk is \"trusted by regulated institutions, public companies, and startups\";\n  named production customers on https://blnkfinance.com/customers include Public Grid, Morna Tech,\n  Yousend and Tecnologia Financiera.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/security/blnkfinance-trust-center.yml
summary_line: ISO/IEC 27001, GDPR, SOC 2, PCI DSS, HIPAA
tags:
- Fintech
- Financial-Services
- Ledger
- double-entry-accounting
- Payments
- Wallets
- Lending
- Banking Infrastructure
- Open-Source
- MCP
- AI Agents
- Developer Tools
trust_url: ''
---
