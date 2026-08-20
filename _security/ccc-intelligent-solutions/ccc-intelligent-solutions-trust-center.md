---
certifications: []
description: ''
kind: trust-center
layout: security
name: Ccc Intelligent Solutions Trust Center
name_suffix: Trust Center
overview: CCC Intelligent Solutions maintains a public trust center covering its security and compliance posture.
provider_name: CCC Intelligent Solutions
provider_slug: ccc-intelligent-solutions
slug: ccc-intelligent-solutions-trust-center
source_filename: ccc-intelligent-solutions-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nprobe: true\nurl: https://trust.cccis.com/\nstatus: 200\nverified: '2026-07-25'\nplatform: Whistic (public shared security profile, Angular SSR app served on CCC's\n  own trust.cccis.com hostname)\nplatform_evidence: |\n  The page bundle at https://trust.cccis.com/main.4945c477c9ed006e.js references\n  api.whistic.com, graphql.whistic.com, external.whistic.com and the Whistic\n  shared-profile components (lib-whistic-shared-profile-elevate,\n  app-public-profile-elevate). The server-rendered HTML ships only the app shell.\ncertifications: []\ncertifications_note: |\n  No certification badge, framework name or document list is present in the\n  anonymously served HTML - Whistic loads the profile contents client-side and\n  typically gates document access behind an access request/NDA. NOTHING was\n  inferred: the certifications list is deliberately empty rather than populated\n  from marketing claims.\npublished_assurance:\n  source:\
  \ CCC Security Addendum (SA 110425) s7 Audit\n  quote: |\n    \"Customer may request CCC's standard privacy and security questionnaires\n    (SIG), third party reports (SOC2 Type II), and documentation to demonstrate\n    compliance with this Security Addendum.\"\n  frameworks_named_by_ccc:\n  - NIST Cybersecurity Framework v2.0\n  - NIST SP 800-88\n  - SOC 2 Type II (report available to contracted customers on request)\n  - CVSS\n  self_serve_download: false\nrelated:\n  security_policy: security/ccc-intelligent-solutions-security-policy.yml\n  conformance: conformance/ccc-intelligent-solutions-conformance.yml\n  information_security_program: https://www.cccis.com/policy/information-security-program\n  legal_documents: https://docs.cccis.com/insurers/legal\nevidence:\n- source: https://trust.cccis.com/\n  kind: trust-center\n  status: 200\n  keywords: [whistic, trust]\n- source: https://www.cccis.com/policy/information-security-program\n  kind: security-policy-page\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccc-intelligent-solutions/refs/heads/main/security/ccc-intelligent-solutions-trust-center.yml
summary_line: trust center published
tags:
- Insurance
- United States
- Property and Casualty
- Claims
- Auto Physical Damage
- Collision Repair
- Insurtech
- Claims Technology
- CIECA
- Partner Gated
- Authentication
- OpenID Connect
trust_url: https://trust.cccis.com/
---
