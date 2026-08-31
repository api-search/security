---
certifications:
- SOC 2 (AICPA SOC)
- ISO/IEC 27001:2022
- PCI DSS
description: 'RainFocus has no dedicated trust-center product page. Its Privacy and Security hub at /privacy-security/ is the equivalent surface: it names the certifications and links every legal and security document. A host at trust.rainfocus.com exists and resolves but sits behind a Cloudflare interstitial ("Just a moment...") that this crawler could not clear, so its contents were not read and nothing is asserted about it.'
kind: trust-center
layout: security
name: Rainfocus Trust Center
name_suffix: Trust Center
overview: RainFocus maintains a public trust center documenting SOC 2 (AICPA SOC), ISO/IEC 27001:2022, and PCI DSS compliance.
provider_name: RainFocus
provider_slug: rainfocus
slug: rainfocus-trust-center
source_filename: rainfocus-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.rainfocus.com/privacy-security/\ndescription: >-\n  RainFocus has no dedicated trust-center product page. Its Privacy and Security hub at\n  /privacy-security/ is the equivalent surface: it names the certifications and links every legal\n  and security document. A host at trust.rainfocus.com exists and resolves but sits behind a\n  Cloudflare interstitial (\"Just a moment...\") that this crawler could not clear, so its contents\n  were not read and nothing is asserted about it.\ntrust_center:\n  url: https://www.rainfocus.com/privacy-security/\n  dedicated_product: false\n  subdomain:\n    host: https://trust.rainfocus.com/\n    status: 403\n    note: Cloudflare managed-challenge interstitial; not confirmed dead, not read.\ncertifications:\n- name: SOC 2 (AICPA SOC)\n  claimed: true\n  detail: Stated as \"AICPA SOC Certified\" on the vulnerability disclosure and privacy/security pages.\n  report_available: unknown\n\
  - name: ISO/IEC 27001:2022\n  claimed: true\n  detail: >-\n    \"RainFocus is ISO/IEC 27001:2022 certified and is audited annually.\" The vulnerability\n    disclosure page carries a typo rendering it as \"ISO/IEC 26001\"; the privacy and security hub\n    states 27001:2022, which is the correct standard for an information security management system.\n  report_available: unknown\n- name: PCI DSS\n  claimed: true\n  detail: Listed as compliant on the privacy and security hub.\n  report_available: unknown\nregulatory_compliance:\n- GDPR\n- CCPA\nsecurity_practices_published:\n- encryption at rest and in transit, with additional layers for sensitive data\n- annual third-party ISO 27001 audit\n- named subprocessor list\n- published data retention policy\ndocuments:\n- name: Privacy Policy\n  url: https://www.rainfocus.com/privacy-policy/\n  status: 200\n- name: Terms of Use\n  url: https://www.rainfocus.com/privacy-security/terms-of-use/\n  status: 200\n- name: API and MCP Tools Terms and\
  \ Conditions\n  url: https://www.rainfocus.com/privacy-security/api-terms-and-conditions/\n  status: 200\n- name: Subprocessors\n  url: https://www.rainfocus.com/privacy-security/subprocessors/\n  status: 200\n- name: Data Retention Policy\n  url: https://www.rainfocus.com/privacy-security/data-retention-policy/\n  status: 200\n- name: Vulnerability Disclosure Program\n  url: https://www.rainfocus.com/privacy-security/vulnerability-disclosure/\n  status: 200\n- name: Base Terms\n  url: https://www.rainfocus.com/legal/base-terms/\n  status: 200\nnot_claimed:\n- HIPAA\n- FedRAMP\n- TX-RAMP\n- StateRAMP\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainfocus/refs/heads/main/security/rainfocus-trust-center.yml
summary_line: SOC 2 (AICPA SOC), ISO/IEC 27001:2022, PCI DSS
tags:
- Company
- Event
- Event Management
- Event Marketing
- Registration
- Conferences
- Webinars
- Marketing Technology
- Attendee Data
- MCP
- Agents
- Enterprise Software
- Software-as-a-Service
trust_url: ''
---
