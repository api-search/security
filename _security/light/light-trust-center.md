---
api_specs:
- filename: light-openapi-original.json
  format: json
  label: Light API
  slug: light-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/openapi/light-openapi-original.json
certifications:
- SOC 2 Type II
- SOC 1 Type II
- SOX / Sarbanes-Oxley compliance
description: ''
kind: trust-center
layout: security
name: Light Trust Center
name_suffix: Trust Center
overview: Light maintains a public trust center documenting SOC 2 Type II, SOC 1 Type II, and SOX / Sarbanes-Oxley compliance compliance.
provider_name: Light
provider_slug: light
slug: light-trust-center
source_filename: light-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://light.inc/security\nurl: https://light.inc/security\ncorrected: '2026-07-19'\ncorrection_note: >-\n  The automated probe keyword-matched \"ISO 27001\" and \"HIPAA\" on the security page and\n  recorded them as Light certifications. Reading the surrounding sentences shows both are\n  claims about Light's INFRASTRUCTURE PROVIDERS (cloud data centers / the AWS deployment),\n  not certifications held by Light. They have been moved to vendor_scoped_claims. SOC 1 Type\n  II and SOX were missed by the probe and have been added.\n\ntrust_center:\n  dedicated_trust_center: false\n  notes: >-\n    The site footer carries a \"Trust Center\" item, but its href is \"#\" — an unimplemented\n    placeholder, not a link to a trust portal. Light's published trust surface is the\n    /security page plus the dedicated /soc-2, /soc-1 and /sox-compliance pages.\n\ncertifications:\n- name: SOC 2 Type II\n  url: https://light.inc/soc-2\n\
  \  evidence: >-\n    \"Light is SOC 2 Type II compliant, meaning that the way we process and store client data is\n    secure and protected, based on standards set by the AICPA.\"\n- name: SOC 1 Type II\n  url: https://light.inc/soc-1\n  evidence: Listed as \"SOC 1, Type 2\" in the site compliance footer.\n- name: SOX / Sarbanes-Oxley compliance\n  url: https://light.inc/sox-compliance\n  evidence: Dedicated \"Sarbanes-Oxley Act & SOX compliance\" page.\n\nregulatory:\n- name: GDPR\n  url: https://light.inc/gdpr\n- name: CCPA\n  evidence: '\"Compliant with GDPR (& CCPA)\"'\n- name: DPA\n  url: https://light.inc/dpa\n\nvendor_scoped_claims:\n- standard: ISO 27001\n  scope: cloud providers\n  evidence: >-\n    \"we ... only work with cloud providers whose data centers are SOC 2 and ISO 27001 certified\"\n- standard: ISO (unspecified)\n  scope: Light servers\n  evidence: '\"All Light servers are ISO-certified.\" — standard and certification body not named.'\n- standard: HIPAA\n  scope: AWS\
  \ deployment\n  evidence: '\"Our own core backend application is located in our HIPAA-compliant AWS deployment.\"'\n- standard: PCI\n  scope: AWS Secrets Manager\n  evidence: >-\n    \"The secrets we store with enterprise-grade AWS Secrets Manager which is both PCI and SOC 2\n    compliant.\"\n\nsecurity_practices:\n- Encryption in transit and at rest.\n- Multi-factor authentication; 2FA and secure password generators used internally.\n- Data residency in the European Union.\n- Minimal OAuth scopes requested from connected systems.\n- Backups replicated to different locations.\n\nevidence:\n- source: https://light.inc/security\n  keywords: [soc 2, soc 1, sox, gdpr, ccpa, encryption, mfa]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/security/light-trust-center.yml
summary_line: SOC 2 Type II, SOC 1 Type II, SOX / Sarbanes-Oxley compliance
tags:
- Accounting
- Finance
- ERP
- Accounts Payable
- Accounts Receivable
- General Ledger
- Spend Management
- Invoicing
- Corporate Cards
- Expense Management
- Financial Operations
- Agents
- Company
trust_url: https://light.inc/security
---
