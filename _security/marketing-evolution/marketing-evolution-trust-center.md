---
certifications:
- ISO/IEC 27001:2022
- ISO/IEC 42001:2023
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Marketing Evolution Trust Center
name_suffix: Trust Center
overview: Marketing Evolution maintains a public trust center documenting ISO/IEC 27001:2022, ISO/IEC 42001:2023, and SOC 2 Type 2 compliance.
provider_name: Marketing Evolution
provider_slug: marketing-evolution
slug: marketing-evolution-trust-center
source_filename: marketing-evolution-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.marketingevolution.com/\nurl: https://trust.marketingevolution.com/\nplatform: SafeBase (by Drata)\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://trust.marketingevolution.com/\n  http_status: 200\n  content_type: text/html\n  parsed_from: __NEXT_DATA__ props.pageProps.orgInfo.sp.products.default.raw.spData\n  control_items_published: 175\n\n# IMPORTANT — read `status` on every row before treating this as a certification claim.\n# The trust center names three frameworks, but the provider's own explanation on each\n# one says it is NOT currently held: the ISO 27001 certificate LAPSED and is in\n# recertification, and both ISO 42001 and SOC 2 Type 2 are planned, not audited.\n# This artifact records that distinction verbatim so the catalog does not credit\n# Marketing Evolution with certifications it says it does not hold.\ncertifications_held: 0\ncertifications_in_progress: 3\n\ncertifications:\n\
  - name: ISO/IEC 27001:2022\n  status: in_progress\n  held: false\n  auditor: A-LIGN\n  provider_statement: >-\n    Marketing Evolution previously held ISO27001 certification. While our certification\n    lapsed during a period of organizational restructuring, our information security\n    management system and security controls have remained in place and continue to\n    operate. We are actively engaged with A-LIGN to achieve ISO27001:2022 recertification.\n  source: https://trust.marketingevolution.com/?itemName=reports&itemUid=5c93ca3e-519a-4260-a50a-a9de78294538\n- name: ISO/IEC 42001:2023\n  status: in_progress\n  held: false\n  auditor: null\n  provider_statement: >-\n    Marketing Evolution plans to pursue ISO/IEC 42001 certification as part of our\n    expanding AI governance program. Our AI management system includes documented\n    governance, risk management, and development practices, with certification planned\n    as part of our broader compliance roadmap.\n  source: https://trust.marketingevolution.com/?itemName=reports&itemUid=14594ab4-5ef0-41fb-a53c-aa408ff72971\n\
  - name: SOC 2 Type 2\n  status: in_progress\n  held: false\n  auditor: A-LIGN\n  provider_statement: >-\n    Marketing Evolution plans to undergo a SOC 2 Type II audit following completion of\n    our ISO/IEC 27001 recertification. Our security program and control environment are\n    designed to support SOC 2 requirements, and the audit is included as part of our\n    ongoing compliance roadmap.\n  source: https://trust.marketingevolution.com/?itemName=reports&itemUid=fa950d02-cbb3-4010-b917-7137a7c2a982\n\n# Published control areas (SafeBase cards) that carry provider-authored explanations.\ncontrol_areas:\n- Overview\n- Compliance\n- Documents\n- Reports\n- Product Security\n- Data Security\n- Data Privacy\n- Customer Data\n- App Security\n- Access Control\n- Network Security\n- Endpoint Security\n- Infrastructure\n- Corporate Security\n- Incident Response\n- Risk Management\n- Risk Profile\n- Asset Management\n- BC/DR\n- Change Management\n- Continuous Monitoring\n- Training\n- Policies\n\
  - Legal\n- Subprocessors\n- AI\n- ESG\n\n# Security-assurance items published on the trust center. These are control\n# ASSERTIONS with provider explanations, not attested reports.\nsecurity_assurance:\n- item: Application Penetration Testing\n  maturity: full\n  provider_statement: >-\n    Marketing Evolution proactively identifies vulnerabilities in its applications and\n    systems through various methods, including security assessments. This is part of a\n    comprehensive vulnerability management policy designed to reduce security risks and\n    protect information assets.\n- item: Penetration Testing\n  maturity: null\n  provider_statement: >-\n    Marketing Evolution has a defined policy for vulnerability management across the\n    organization, which includes monitoring, cataloging, and assigning risk ratings to\n    vulnerabilities to prioritize remediation efforts.\n- item: Code Analysis\n  maturity: full\n  provider_statement: >-\n    Marketing Evolution identifies vulnerabilities\
  \ using a combination of methods, which\n    may include automated tools, development and deployment workflows, security\n    assessments, third-party advisories, and other sources of security-relevant\n    information. All AI-generated code must follow secure coding practices, licensing\n    rules, and regulatory requirements, with developers clearly documenting when AI\n    assistance was used.\n- item: Responsible Disclosure\n  maturity: null\n  provider_statement: >-\n    Marketing Evolution actively addresses responsible disclosure through established\n    processes, including bug bounties, to proactively identify and remediate security\n    flaws.\n\n# Why no VulnerabilityDisclosure / Security pointer is emitted from this artifact:\n# the trust center ASSERTS a responsible-disclosure process (and mentions bug bounties)\n# but publishes no reporting channel — no security.txt on any host (all 404, see\n# well-known/marketing-evolution-well-known.yml), no security@ address anywhere\
  \ on the\n# site or trust center, no named bug-bounty program page (HackerOne/Bugcrowd/Intigriti\n# all miss). A researcher reading this cannot report a vulnerability, so the claim is\n# recorded here rather than promoted to a disclosure pointer.\nresponsible_disclosure:\n  asserted: true\n  reporting_channel_published: false\n  security_txt: false\n  security_contact: null\n  bounty_program_url: null\n\n# Why no Compliance pointer is emitted: `compliance_published` credits a published\n# certification/compliance posture. Marketing Evolution publishes a compliance ROADMAP\n# with zero currently-held certifications. Flip this to a Compliance pointer on a later\n# pass once A-LIGN completes the ISO/IEC 27001:2022 recertification.\ncompliance_pointer_emitted: false\n\nnotes: >-\n  Full SafeBase trust center with 175 published control items, an AI-governance (AIMS)\n  section, and a vendor-management program. Substantially more security transparency\n  than the company publishes about its\
  \ API surface, which has no public documentation\n  at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketing-evolution/refs/heads/main/security/marketing-evolution-trust-center.yml
summary_line: ISO/IEC 27001:2022, ISO/IEC 42001:2023, SOC 2 Type 2
tags:
- Company
- Marketing
- Analytics
- Marketing Measurement
- Attribution
- Media Planning
- Artificial Intelligence
- MarTech
- Marketing Mix Modeling
- Marketing Intelligence
- Advertising
trust_url: https://trust.marketingevolution.com/
---
