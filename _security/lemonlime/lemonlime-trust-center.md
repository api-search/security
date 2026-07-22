---
certifications:
- SOC 2
- GDPR
- HIPAA
- PCI DSS
description: 'LemonLime has no trust.<domain> or security.<domain> subdomain (neither resolves); its compliance posture is published on a single /security page. As an early-stage (YC S2026) company its certification story is forward-looking rather than attained: a SOC 2 examination is in progress with Oneleet and the report is not yet issued. HIPAA/PCI are described as deployment-alignment options on the Enterprise plan, not as held certifications. Recorded here exactly as published — no certification is asserted as complete. The mechanical probe flagged "SOC 2" and "GDPR" as keyword hits on this page; this searched capture qualifies those hits with their real status and is kept in preference to the probe''s flat certification list.'
kind: trust-center
layout: security
name: Lemonlime Trust Center
name_suffix: Trust Center
overview: LemonLime maintains a public trust center documenting SOC 2, GDPR, HIPAA, and PCI DSS compliance.
provider_name: LemonLime
provider_slug: lemonlime
slug: lemonlime-trust-center
source_filename: lemonlime-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://lemonlime.ai/security\nurl: https://lemonlime.ai/security\ndescription: >-\n  LemonLime has no trust.<domain> or security.<domain> subdomain (neither resolves);\n  its compliance posture is published on a single /security page. As an early-stage\n  (YC S2026) company its certification story is forward-looking rather than attained:\n  a SOC 2 examination is in progress with Oneleet and the report is not yet issued.\n  HIPAA/PCI are described as deployment-alignment options on the Enterprise plan, not\n  as held certifications. Recorded here exactly as published — no certification is\n  asserted as complete. The mechanical probe flagged \"SOC 2\" and \"GDPR\" as keyword\n  hits on this page; this searched capture qualifies those hits with their real status\n  and is kept in preference to the probe's flat certification list.\ncertifications:\n  - name: SOC 2\n    status: in-progress\n    attained: false\n\
  \    auditor: Oneleet\n    availability: >-\n      To be made available to Customers and prospective Customers under NDA when issued.\n    evidence: >-\n      \"We are completing a SOC 2 examination with the support of Oneleet, and we will\n      make our current report available to Customers and prospective Customers under\n      NDA when it is issued.\"\n  - name: GDPR\n    status: compliance-program\n    attained: true\n    note: >-\n      GDPR handling, subprocessor categories, and retention/deletion commitments are\n      published rather than third-party certified.\n  - name: HIPAA\n    status: deployment-alignment\n    attained: false\n    note: >-\n      Offered as a compliance-aligned deployment protocol on the Enterprise plan\n      (\"security reviews (SOC 2, HIPAA, PCI)\"), not a held certification.\n  - name: PCI DSS\n    status: deployment-alignment\n    attained: false\n    note: >-\n      Offered as a compliance-aligned deployment protocol on the Enterprise plan,\n    \
  \  not a held certification.\nencryption:\n  in_transit: TLS 1.2 or higher\n  at_rest: AES-256\ndata_handling:\n  trains_on_customer_data: false\n  trains_on_customer_data_statement: >-\n    \"LemonLime does not train its models on customer business data — across every\n    plan, in every deployment.\"\n  zero_data_retention: optional\n  zero_data_retention_note: Available on request for the highest-privacy customers.\n  retention: >-\n    \"We retain indexed content only while the relevant integration and account remain\n    active. When you disconnect an integration or close your account, we no longer\n    access the associated source content\" and purge from backups on standard rotation.\nsubprocessors:\n  published: false\n  location: Maintained in the Privacy Policy (https://lemonlime.ai/privacy)\n  categories: [cloud hosting providers, intelligence model providers, operational tooling]\nenterprise_controls:\n  - SSO/SAML (Enterprise plan)\n  - Permission controls and activity history\
  \ (Team plan and above)\n  - Customer security reviews (Enterprise plan)\ndocs:\n  - https://lemonlime.ai/security\n  - https://lemonlime.ai/privacy\nevidence:\n  - source: https://lemonlime.ai/security\n    keywords: [soc 2, oneleet, gdpr, tls 1.2, aes-256, subprocessors, retention]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonlime/refs/heads/main/security/lemonlime-trust-center.yml
summary_line: SOC 2, GDPR, HIPAA, PCI DSS
tags:
- Company
- Artificial Intelligence
- Knowledge Management
- AI Agents
- Workflow Automation
- Model Context Protocol
- Enterprise Software
- SaaS
- Y Combinator
trust_url: https://lemonlime.ai/security
---
