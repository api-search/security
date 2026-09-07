---
api_specs:
- filename: acall-public-api-openapi.yml
  format: yaml
  label: Acall Public API
  slug: acall-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acall/refs/heads/main/openapi/acall-public-api-openapi.yml
certification_count: 1
certifications:
- ISO/IEC 27001 (ISMS)
description: ''
kind: trust-center
layout: security
name: Acall Trust Center
name_suffix: Trust Center
overview: Acall maintains a public trust center documenting ISO/IEC 27001 (ISMS) compliance.
provider_name: Acall
provider_slug: acall
slug: acall-trust-center
source_filename: acall-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nprobe: true\nurl: https://www.workstyleos.com/security/\nnote: >-\n  Acall has no trust portal in the modern sense (no trust.acall.* host, no document-request workflow, no\n  subprocessor list, no SOC 2 report). What it does publish is a security-posture page plus a formal\n  information-security policy and a named ISO/IEC 27001 registration, which is a real, verifiable published\n  compliance program.\ncertifications:\n- name: ISO/IEC 27001 (ISMS)\n  also_registered_as: JIS Q 27001\n  certificate_number: ISA IS 0170\n  scope_url: https://www.acall.inc/about/details\n  source: https://www.workstyleos.com/security/\n  verified: '2026-09-06'\n  note: >-\n    Stated on the security page as 「ISO 27001（ISMS）」の認証を取得しています and carried in the site footer\n    as 認証番号: ISA IS 0170. The registration summary is linked from the company-details page.\nnot_found:\n- SOC 2\n- PCI DSS\n- HIPAA\n- FedRAMP\n- ISO 27017\n- ISO 27018\n- CSA STAR\n- Privacy\
  \ Mark (Pマーク)\npolicies:\n- name: 情報セキュリティ方針 (Information Security Policy)\n  url: https://www.workstyleos.com/security_policy/\n  established: '2022-01-07'\n  revised: '2023-08-01'\n  signed_by: 代表取締役 長沼斉寿\n- name: セキュリティへの取り組み (Security measures)\n  url: https://www.workstyleos.com/security/\ncontrols_published:\n- encryption of stored confidential data at rest\n- TLS/SSL for all traffic to Acall\n- source IP address restriction for Acall Portal access\n- single sign-on (Microsoft Entra ID / Azure AD and others) as a paid option\n- documented risk assessment, internal audit, and incident-response process (per the security policy)\nincident_transparency:\n  status_page: https://status.acall.inc/\n  incident_reports: https://www.workstyleos.com/sctl/\nevidence:\n- source: https://www.workstyleos.com/security/\n  status: 200\n  keywords: [iso 27001, isms, 暗号化, ip アドレス制限, sso]\n- source: https://www.workstyleos.com/security_policy/\n  status: 200\n  keywords: [情報セキュリティ方針, リスクアセスメント, 情報セキュリティマネジメントシステム]\n\
  - source: https://www.acall.inc/about/details\n  status: 200\n  keywords: [ISO/IEC27001, JISQ27001, 認証登録概要]\nvulnerability_disclosure:\n  found: false\n  note: >-\n    No security.txt on any Acall host, no /security/responsible-disclosure or vulnerability-disclosure page,\n    no bug-bounty program on HackerOne, Bugcrowd or Intigriti, and no security@ contact published. The only\n    security.txt reachable under an Acall hostname is Atlassian's, served by the Statuspage vendor at\n    status.acall.inc — see well-known/acall-well-known.yml. No Security or VulnerabilityDisclosure pointer\n    is emitted.\npointer_emitted: false\npointer_note: >-\n  No TrustCenter pointer is wired into apis.yml — Acall publishes a security-posture page and a named\n  ISO/IEC 27001 registration, but no trust portal. The published certification is carried instead by the\n  Compliance pointer at https://www.workstyleos.com/security/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acall/refs/heads/main/security/acall-trust-center.yml
summary_line: ISO/IEC 27001 (ISMS)
tags:
- Workplace Management
- Visitor Management
- Meeting Room Booking
- Desk Booking
- Hybrid Work
- Access Control
- Facilities
- Smart Office
- Japan
- SaaS
trust_url: https://www.workstyleos.com/security/
---
