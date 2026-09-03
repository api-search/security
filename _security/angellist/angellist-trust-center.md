---
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Angellist Trust Center
name_suffix: Trust Center
overview: AngelList maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: AngelList
provider_slug: angellist
slug: angellist-trust-center
source_filename: angellist-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nprobe: true\nurl: https://trust-portal.angellist.com/\nlegal_entity: AL Advisors Management Inc.\ntitle: AL Advisors Management Inc. | Trust Center\nplatform: Secureframe\ncertifications:\n- SOC 2 Type II\ncompliance_programs:\n- id: soc2-type2\n  name: SOC 2 Type 2\n  detail: Service Organization Controls (SOC 2) Type II, Trust Services Principles\n  availability: available on request through the trust portal\n- id: gdpr\n  name: GDPR\n  detail: >-\n    Protects the personal data and privacy of EU citizens for transactions\n    occurring within EU member states.\n  availability: linked from the trust portal\nresources:\n- name: SOC 2 Type II report\n  access: request\n- name: Penetration tests\n  access: request\n- name: Privacy Policy\n  access: public\n  url: https://venture.angellist.com/privacy\nmonitored_control_families:\n- Change Management\n- Availability\n- Organizational Management\n- Confidentiality\n- Vulnerability Management\n\
  - Incident Response\n- Risk Assessment\n- Network Security\n- Access Security\n- Physical Security\nnamed_policies:\n- Secure Development Policy\n- Change Management Policy\n- Configuration and Asset Management Policy\n- Business Continuity and Disaster Recovery Policy\n- Acceptable Use Policy\n- Data Classification Policy\n- Data Retention and Disposal Policy\n- Vulnerability and Patch Management Policy\n- Incident Response Plan\n- Vendor Risk Management Policy\n- Risk Assessment and Treatment Policy\n- Network Security Policy\n- Access Control and Termination Policy\nsubprocessors:\n- {name: AWS, purpose: Application hosting and data storage}\n- {name: Cloudflare, purpose: Content Delivery Network}\n- {name: Google Cloud, purpose: Application hosting and data storage}\n- {name: Front, purpose: Customer Management System}\n- {name: Persona, purpose: Identity verification platform for KYC/AML compliance}\n- {name: Alloy, purpose: Identity data orchestration platform and fraud prevention}\n\
  - {name: Plaid, purpose: Digital finance platform used for bank verification}\n- {name: Coinbase, purpose: Cryptocurrency services}\n- {name: Treasury Prime, purpose: Banking-as-a-service platform}\nevidence:\n- source: https://trust-portal.angellist.com/\n  http_status: 200\n  bytes: 230950\n  keywords: [SOC 2, GDPR, trust center, penetration tests, subprocessors, Secureframe]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angellist/refs/heads/main/security/angellist-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Documents
- Funds
- Investing
- Job
- Startups
- Transaction
- Venture Capital
trust_url: https://trust-portal.angellist.com/
---
