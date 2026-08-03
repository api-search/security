---
certifications:
- SOC 2
- SOC 3
- CSA STAR Level 1
description: ''
kind: trust-center
layout: security
name: Aidash Trust Center
name_suffix: Trust Center
overview: AiDASH maintains a public trust center documenting SOC 2, SOC 3, and CSA STAR Level 1 compliance.
provider_name: AiDASH
provider_slug: aidash
slug: aidash-trust-center
source_filename: aidash-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nsource: https://security.aidash.com/\nurl: https://security.aidash.com/\nplatform: Sprinto\ntitle: AiDash - Trust Center - Security & Privacy\naccess: 'Public overview; policy documents and the SOC 2 Type 2 report are gated\n  behind a \"Request access\" form.'\ncertifications:\n- SOC 2\n- SOC 3\n- CSA STAR Level 1\ncertification_detail:\n- name: SOC 2 Type 2\n  status: certified\n  detail: 'Reported by AiDASH as achieved with no exceptions for the fifth consecutive\n    year.'\n  evidence: https://www.aidash.com/security-compliance-and-responsible-ai/\n- name: SOC 3\n  status: published\n  detail: Public SOC 3 report, no access request required.\n  evidence: https://www.aidash.com/wp-content/uploads/2026/05/AiDASH-Inc.-SOC-3-2026.pdf\n- name: CSA STAR Level 1 (CAIQ self-assessment)\n  status: self-assessed\n  detail: Listed on the Cloud Security Alliance STAR Registry since 2021-02-09.\n  evidence: https://cloudsecurityalliance.org/star/registry/aidash/\n\
  policies_listed:\n- Information Security Policy\n- Operation Security Policy\n- HR Security Policy\n- Vulnerability Management Policy\n- Vendor Management Policy\n- Risk Assessment & Management Policy\n- 6 further policies (access-gated)\nsecurity_practices:\n  encryption: at rest and in transit for all customers\n  key_management: AWS Key Management Service (KMS) backed by hardware security modules\n  cloud_security_tooling: [AWS KMS, AWS GuardDuty, AWS Inspector]\n  static_analysis: [CodeQL, TruffleHog, SonarQube]\n  penetration_testing: third-party external penetration testing\n  deployment: containerized; no customer-managed production servers\nevidence:\n- source: https://security.aidash.com/\n  http_status: 200\n  keywords: [soc 2, soc2, trust center, vulnerability management policy]\n- source: https://www.aidash.com/security-compliance-and-responsible-ai/\n  http_status: 200\n  keywords: [soc 2 type 2, soc 3, penetration testing, responsible ai]\n- source: https://cloudsecurityalliance.org/star/registry/aidash/\n\
  \  http_status: 200\n  keywords: [csa star level 1, caiq]\nnotes: 'security.aidash.com returns HTTP 403 to some automated user agents; the body\n  captured here was retrieved with an ordinary browser user agent (HTTP 200). No\n  public vulnerability-disclosure contact, security.txt, or bug-bounty program was\n  found — a \"Vulnerability Management Policy\" is listed but access-gated, so no\n  VulnerabilityDisclosure or Security pointer is claimed.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidash/refs/heads/main/security/aidash-trust-center.yml
summary_line: SOC 2, SOC 3, CSA STAR Level 1
tags:
- Company
- Satellite
- Artificial Intelligence
- Geospatial
- Utilities
- Energy
- Vegetation Management
- Wildfire
- Climate Risk
- Asset Management
- Remote Sensing
- Vertical SaaS
trust_url: https://security.aidash.com/
---
