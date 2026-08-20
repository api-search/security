---
certifications: []
description: ''
kind: trust-center
layout: security
name: Cerenovus Trust Center
name_suffix: Trust Center
overview: Cerenovus maintains a public trust center covering its security and compliance posture.
provider_name: Cerenovus
provider_slug: cerenovus
slug: cerenovus-trust-center
source_filename: cerenovus-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nurl: https://www.cerenovus.ai/trust-and-security\ntitle: Trust and Security FAQ\nnote: >-\n  A real, public, prerendered trust page written for IT and security teams. It names\n  certifications but claims none of them yet — Cerenovus states plainly that SOC 2\n  Type II and ISO 27001 are \"in the process of being certified\" and that both take\n  several months. Recorded here as in_progress, NOT as held certifications, and no\n  Compliance pointer is emitted on the strength of a pending audit.\ncertifications: []\ncertifications_in_progress:\n- SOC 2 Type II\n- ISO 27001\ncommitments:\n- claim: Customer data is not used to train models\n  detail: >-\n    Cerenovus states it does not train its own models on customer data and holds\n    zero-data-retention agreements with OpenAI and Anthropic.\n- claim: Deployment isolation\n  detail: >-\n    Default is a single-tenant deployment on a cloud machine run by Cerenovus, with\
  \ the\n    network restricted to customer machines for upload and Cerenovus machines for\n    installation and telemetry. Bring-your-own-cloud and full on-premise deployments are\n    offered where stricter isolation is required.\n- claim: Data minimization and retention\n  detail: >-\n    Connectors are scoped to the sources a customer approves; retention is\n    customer-defined and data is kept only while actively in use.\n- claim: Legal instruments offered in lieu of certification\n  detail: Cerenovus offers to sign NDAs and other agreements while certification is pending.\nevidence:\n- source: https://www.cerenovus.ai/trust-and-security\n  http_status: 200\n  keywords:\n  - trust and security\n  - soc 2 type ii\n  - iso 27001\n  - zero-data-retention\n  - single-tenant\n  fetched: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerenovus/refs/heads/main/security/cerenovus-trust-center.yml
summary_line: trust center published
tags:
- Company
- Artificial Intelligence
- AI Agents
- Enterprise Software
- Decision Intelligence
- Knowledge-Management
- Private Equity
- Due Diligence
- MCP
- Y Combinator
trust_url: https://www.cerenovus.ai/trust-and-security
---
