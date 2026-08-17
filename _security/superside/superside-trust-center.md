---
certifications:
- SOC 2 Type II
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Superside Trust Center
name_suffix: Trust Center
overview: Superside maintains a public trust center documenting SOC 2 Type II, GDPR, and CCPA compliance.
provider_name: Superside
provider_slug: superside
slug: superside-trust-center
source_filename: superside-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://www.superside.com/security\nurl: https://www.superside.com/security\nkind: security-and-compliance-page\nkind_note: >-\n  Superside runs no dedicated trust portal — trust.superside.com and security.superside.com\n  do not resolve (curl exit 6, DNS failure), and /trust and /compliance both 404. The\n  public security posture is published as a single marketing-site page at /security, which\n  names the attestations below and links the bug-bounty policy. Recorded as the trust\n  surface because it carries named, dated certifications, not because it is a portal.\ncertifications:\n- name: SOC 2 Type II\n  status: attested\n  cadence: annual\n  auditor: third-party (not named on the page)\n  monitoring: Drata (continuous control monitoring)\n  evidence_text: >-\n    \"Superside completes a SOC 2 Type II audit annually, performed by a trusted third\n    party, with continuous control monitoring through Drata.\"\
  \n- name: GDPR\n  status: compliance-claimed\n  evidence_text: >-\n    \"Superside complies with applicable data protection and privacy laws, including the\n    GDPR and the CCPA.\"\n- name: CCPA\n  status: compliance-claimed\n  evidence_text: >-\n    \"Superside complies with applicable data protection and privacy laws, including the\n    GDPR and the CCPA.\"\nnot_claimed:\n- ISO 27001\n- HIPAA\n- PCI DSS\n- FedRAMP\n- CSA STAR\nnot_claimed_note: >-\n  Searched the /security page and the legal/privacy surface; none of these appear. Recorded\n  as measured absence, not as a failure.\nprograms:\n- incident response plan\n- bug bounty program\nreport_access:\n  soc2_report: request-only\n  note: >-\n    No self-serve document room (no Drata Trust Center / Vanta / SafeBase instance found);\n    the SOC 2 Type II report is not downloadable from the public page.\nevidence:\n- source: https://www.superside.com/security\n  http_status: 200\n  keywords: [soc 2 type ii, drata, gdpr, ccpa, incident\
  \ response plan, bug bounty]\n- source: https://trust.superside.com/\n  http_status: 000\n  note: DNS does not resolve.\n- source: https://www.superside.com/trust\n  http_status: 404\n- source: https://www.superside.com/compliance\n  http_status: 404\nfetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superside/refs/heads/main/security/superside-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA
tags:
- Company
- Saas
- Creative Services
- Design
- Marketing
- AI
- Creative As A Service
trust_url: https://www.superside.com/security
---
