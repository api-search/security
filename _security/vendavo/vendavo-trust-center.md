---
certification_count: 5
certifications:
- ISO/IEC 27001:2022
- SOC 1 Type 2
- SOC 2 Type 2
- CSA STAR Level 1 (CAIQ self-assessment)
- ISO 22301
description: Vendavo publishes a public security posture page at www.vendavo.com/security/ (last updated by Vendavo 11 June 2026) and operates a Trust Center at trustvault.vendavo.com (a Scrut.io tenant, HTTP 200). The certifications below are quoted from the public security page; the Trust Center itself renders client-side and gates its document library behind an access request, so the certification list was taken from the server-rendered security page rather than the Trust Center shell. The automated trust-center probe missed this because Vendavo uses the non-standard `trustvault.` subdomain rather than `trust.<domain>`.
kind: trust-center
layout: security
name: Vendavo Trust Center
name_suffix: Trust Center
overview: Vendavo maintains a public trust center documenting ISO/IEC 27001:2022, SOC 1 Type 2, SOC 2 Type 2, CSA STAR Level 1 (CAIQ self-assessment), and ISO 22301 compliance.
provider_name: Vendavo
provider_slug: vendavo
slug: vendavo-trust-center
source_filename: vendavo-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: false\nsource: https://www.vendavo.com/security/\nurl: https://trustvault.vendavo.com/\ndescription: Vendavo publishes a public security posture page at www.vendavo.com/security/ (last updated by Vendavo 11 June 2026) and operates a Trust Center at trustvault.vendavo.com (a Scrut.io tenant, HTTP 200). The certifications below are quoted from the public security page; the Trust Center itself renders client-side and gates its document library behind an access request, so the certification list was taken from the server-rendered security page rather than the Trust Center shell. The automated trust-center probe missed this because Vendavo uses the non-standard `trustvault.` subdomain rather than `trust.<domain>`.\ntrust_center:\n  url: https://trustvault.vendavo.com/\n  platform: Scrut.io\n  http_status: 200\n  document_access: request-access\n  note: '\"Trust Center – Visit our Trust Center to learn about our security posture and\
  \ request access to documentation\" (www.vendavo.com/security/). The page is a client-rendered Next.js shell; no certification data is present in the served HTML.'\ncertifications:\n- ISO/IEC 27001:2022\n- SOC 1 Type 2\n- SOC 2 Type 2\n- CSA STAR Level 1 (CAIQ self-assessment)\n- ISO 22301\nprivacy_regimes:\n- name: EU GDPR\n  claim: enables customer compliance\n- name: UK GDPR\n  claim: enables customer compliance\n- name: California CPRA\n  claim: enables customer compliance\nsecurity_practices:\n- Independent penetration tests, static and dynamic testing, security design and code reviews.\n- Regular internal and external vulnerability scans; systematic patch management program.\n- Encryption at rest and in transit; customer data segmentation in multi-tenant applications.\n- Fine-grained RBAC/ABAC; SSO integration with customer identity management systems.\n- EDR/XDR with 24x7x365 Security Operations oversight; DDoS protection via firewalls, load balancers, WAF.\n- ISMS governed by a\
  \ Security & Compliance Council chaired by the CISO, meeting bimonthly.\nvulnerability_disclosure:\n  published: false\n  note: No responsible-disclosure or vulnerability-reporting policy, no bug-bounty program and no security contact address are published. /.well-known/security.txt returns 404 on every Vendavo host, and neither the security page, the privacy notice nor the contractor security policy names a security@ address. No `VulnerabilityDisclosure` artifact and no `Security` pointer are emitted — there is nothing to point at.\ndocs:\n- https://www.vendavo.com/security/\n- https://www.vendavo.com/contractor-security-policy/\n- https://cloudsecurityalliance.org/star/registry/vendavo/\nevidence:\n- url: https://www.vendavo.com/security/\n  status: 200\n  keywords:\n  - iso 27001:2022\n  - soc 1 type 2\n  - soc 2 type 2\n  - csa star\n  - caiq\n  - iso 22301\n  - gdpr\n  - cpra\n- url: https://trustvault.vendavo.com/\n  status: 200\n  note: Scrut.io Trust Center; client-rendered shell,\
  \ title \"Trust Vault\"\n- url: https://cloudsecurityalliance.org/star/registry/vendavo/\n  status: 200\n  note: page title \"STAR Registry Entries for Vendavo Inc.\"\n- url: https://www.vendavo.com/.well-known/security.txt\n  status: 404\ncertification_details:\n- name: ISO/IEC 27001:2022\n  status: certified\n  cadence: annual\n  note: '\"Vendavo maintains certification to the international standard to manage information security.\" ISMS is built on ISO 27001.'\n- name: SOC 1 Type 2\n  status: attested\n  cadence: annual\n  availability: on request via Trust Center\n  note: '\"Vendavo conducts annual audits to ensure controls over financial reporting.\"'\n- name: SOC 2 Type 2\n  status: attested\n  cadence: annual\n  availability: on request via Trust Center\n  trust_services_criteria:\n  - Security\n  - Availability\n  - Confidentiality\n  - Processing Integrity\n  note: '\"Vendavo conducts annual audits to ensure control and management of customer data, covering the Security, Availability,\
  \ Confidentiality and Processing Integrity Trust Services Criteria.\"'\n- name: CSA STAR Level 1 (CAIQ self-assessment)\n  status: self-assessed\n  registry: https://cloudsecurityalliance.org/star/registry/vendavo/\n  registry_http_status: 200\n  note: '\"Vendavo has published our completed CSA Consensus Assessments Initiative Questionnaire (CAIQ) self-assessment in the CSA STAR Registry.\"'\n- name: ISO 22301\n  status: aligned\n  note: Not a certification claim — \"our business continuity program is aligned with the international standard ISO 22301.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendavo/refs/heads/main/security/vendavo-trust-center.yml
summary_line: ISO/IEC 27001:2022, SOC 1 Type 2, SOC 2 Type 2, CSA STAR Level 1 (CAIQ self-assessment), ISO 22301
tags:
- Company
- Enterprise
- Pricing
- CPQ
- Quoting
- Rebates
- B2B
- Commercial Optimization
- Margin Optimization
- Artificial Intelligence
trust_url: https://trustvault.vendavo.com/
---
