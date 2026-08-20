---
api_specs:
- filename: TzCHBqbH
  format: yaml
  label: Prismic Types API
  slug: types-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/5743666/TzCHBqbH
certifications: []
description: ''
kind: trust-center
layout: security
name: Prismic Trust Center
name_suffix: Trust Center
overview: Prismic maintains a public trust center covering its security and compliance posture.
provider_name: Prismic
provider_slug: prismic
slug: prismic-trust-center
source_filename: prismic-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://prismic.io/legal/security\nurl: https://prismic.io/legal/security\npage_last_updated: '2026-06-11'\nkind: security policy page\ntrust_center: false\ntrust_center_note: >-\n  Prismic does not operate a trust center. trust.prismic.io and\n  security.prismic.io do not resolve to a trust portal; what exists is one static\n  legal page, https://prismic.io/legal/security, with no downloadable evidence,\n  no report request flow and no subprocessor list.\ncertifications: []\ncertifications_correction: >-\n  CORRECTED 2026-08-13. A prior automated pass recorded SOC 2, ISO 27001,\n  ISO 27017, ISO 27018, PCI DSS, GDPR and CSA STAR as Prismic certifications.\n  They are not. Reading the page in full, every one of those names belongs to a\n  THIRD PARTY, and Prismic's own text says so plainly:\n    - ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, PCI-DSS Level 1, SOC 1, SOC 2,\n      SOC 3 and CSA STAR Levels 1-3 are\
  \ listed in the \"Data hosting and storage\"\n      section as AWS's certifications — \"AWS is widely recognized as a global\n      leader in cloud infrastructure, with its data centers and services\n      certified against ... \" Prismic hosts on AWS us-east-1; it does not hold\n      these.\n    - PCI is disclaimed outright: \"All payment instrument processing is\n      outsourced to Stripe. Stripe ... is certified as a PCI Service Provider\n      Level 1.\"\n    - SOC 2 and ISO 27001 also appear in the \"Third-party suppliers\" paragraph,\n      as certifications Prismic REQUIRES OF ITS OWN SUPPLIERS.\n  Prismic names no certification of its own anywhere on the page. Its\n  \"Compliance certifications & policies\" section describes internal auditing,\n  legal watch, annual security training and Stripe's PCI status — no audited\n  attestation. Keyword-matching a security page is how a hosting provider's\n  compliance posture gets credited to its tenant; this file records the\n  distinction\
  \ instead.\nown_certifications: none published\nsupplier_certifications:\n  - {party: AWS, role: infrastructure host (us-east-1), certifications: [ISO/IEC 27001,\n      ISO/IEC 27017, ISO/IEC 27018, PCI-DSS Level 1, SOC 1, SOC 2, SOC 3, CSA STAR\n        Levels 1-3]}\n  - {party: Stripe, role: payment processing, certifications: [PCI Service Provider\n        Level 1]}\n  - {party: Intercom, role: 'sales, marketing and support — processes personal data'}\npublished_practices:\n  - {area: penetration testing, detail: Performed on a yearly basis by external independent\n      contractors specializing in web application cybersecurity, with a remediation\n      plan scheduled by criticality and re-testing of resolved issues.}\n  - {area: vulnerability scanning, detail: Continuous, using industry standards and\n      tools.}\n  - {area: security audits, detail: Periodic internal evaluation of peripheral and\n      in-depth services by external independent contractors.}\n  - {area: secure development\
  \ lifecycle, detail: Code peer review plus a security checklist\n      per release; non-regression testing and approval before production.}\n  - {area: security policies, detail: 'Internal policy set covering access control,\n      physical security, secure development, data protection, privacy and confidentiality;\n      reviewed periodically.'}\n  - {area: security training, detail: Annual security and awareness training for all\n      employees.}\n  - {area: incident response, detail: 'Documented Incident Response Plan with tenant-specific\n      security contacts for Enterprise customers; incident declaration, action tracking,\n      stakeholder communication and post-incident documentation.'}\n  - {area: business continuity, detail: Redundant deployment across three Availability\n      Zones in one AWS region, with backups/snapshots/replication and point-in-time\n      recovery to S3, plus documented runbooks and infrastructure-as-code redeployment.}\n  - {area: audit logging, detail:\
  \ Tooling and processes monitoring account activity\n      across the infrastructure.}\n  - {area: network segregation, detail: 'AWS Network Security Group rules, reviewed\n      and adapted at least annually; virtual firewall between tenants.'}\ndata_protection:\n  gdpr: 'Claimed — \"Prismic fulfils its obligations and maintains transparency about\n    how it processes personal data.\"'\n  dpa:\n    available_online: false\n    note: '\"Prismic is in the process of making a DPA available online\" — in the meantime\n      Enterprise customers must go through their Account Manager.'\n  data_residency: AWS us-east-1 (Northern Virginia, USA) — single region, no choice\n    offered\n  data_portability: Content and metadata exportable through the tenant API endpoint\n  personal_data_scope: 'Limited to the name and email of business users with repository\n    access; more may be processed by Intercom.'\n  contacts:\n    data_privacy: dataprivacy@prismic.io\n    security: security@prismic.io\n\
  sso:\n  supported: true\n  standards: [OAuth2, AD, Okta]\n  tier: Enterprise only, on request\n  mfa: via the customer's own identity provider\nuptime:\n  sla_document: none published\n  sla_availability: Enterprise tier only (\"Support and uptime SLAs\")\n  monitoring: https://status.prismic.io/\nevidence:\n  - {source: 'https://prismic.io/legal/security', http_status: 200, fetched: '2026-08-13',\n     read: full page text, not keyword match}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prismic/refs/heads/main/security/prismic-trust-center.yml
summary_line: trust center published
tags:
- GraphQL
- Headless CMS
- Content Management
- Page Builder
- JAMstack
- Marketing
- Content Delivery
- Developer Tools
- MCP
- Webhook
- Localization
- Digital Asset Management
trust_url: https://prismic.io/legal/security
---
