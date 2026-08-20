---
certifications:
- SOC 2 Type II
- CASA Tier 3
description: ''
kind: trust-center
layout: security
name: 11X Trust Center
name_suffix: Trust Center
overview: 11x maintains a public trust center documenting SOC 2 Type II and CASA Tier 3 compliance.
provider_name: 11x
provider_slug: 11x
slug: 11x-trust-center
source_filename: 11x-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: true\nsource: https://trust.11x.ai/\nurl: https://trust.11x.ai/\nplatform: SafeBase\nplatform_note: trust.11x.ai is a CNAME to x-1.portals.safebase.io\nsecondary_source: https://www.11x.ai/security\ncertifications:\n- id: soc2-type-2\n  name: SOC 2 Type II\n  detail: >-\n    Annual audit covering System Security, Availability, Processing Integrity, Confidentiality\n    and Privacy.\n  source: https://www.11x.ai/security\n- id: casa-tier-3\n  name: CASA Tier 3\n  detail: >-\n    Covers Identity & Access Management, Data Security, Infrastructure & Virtualisation Security,\n    Application & Interface Security, and Incident Management.\n  source: https://www.11x.ai/security\nregulatory_alignment:\n- id: gdpr\n  claimed: true\n  detail: Data retention protocols and data processing agreements offered to EU customers.\n- id: ccpa\n  claimed: true\npolicies_published:\n- Acceptable Use\n- Business Continuity / Disaster Recovery\n-\
  \ Change Management\n- Code of Conduct\n- Data Classification, Protection and Retention\n- Incident Response\n- Information Security\n- Network Security\ncontrols_listed:\n- Asset Management\n- Business continuity and disaster recovery\n- Capacity and performance planning\ninfrastructure:\n  hosting: AWS\n  encryption_in_transit: TLS\n  encryption_at_rest: AES-256 (AWS RDS)\n  resilience: clustered database configurations, dynamic scaling, containerized deployments\n  monitoring: centralized infrastructure change tracking and security event logging\nnot_claimed:\n- ISO 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\nevidence:\n- source: https://trust.11x.ai/\n  http_status: 200\n  keywords: [soc 2, casa tier 3, trust center, security]\n- source: https://www.11x.ai/security\n  http_status: 200\n  keywords: [soc 2 type ii, casa tier 3, gdpr, ccpa, aes-256, aws]\nx-evidence:\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/11x/refs/heads/main/security/11x-trust-center.yml
summary_line: SOC 2 Type II, CASA Tier 3
tags:
- Company
- Artificial Intelligence
- AI Agents
- Sales
- Sales Automation
- Lead Generation
- Conversational AI
- Voice
- CRM
- Go-To-Market
trust_url: https://trust.11x.ai/
---
