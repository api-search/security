---
certifications:
- ISO 27001:2022
- SOC 2
- Cyber Essentials
- PCI DSS SAQ A
description: ''
kind: trust-center
layout: security
name: Instanda Trust Center
name_suffix: Trust Center
overview: INSTANDA maintains a public trust center documenting ISO 27001:2022, SOC 2, Cyber Essentials, and PCI DSS SAQ A compliance.
provider_name: INSTANDA
provider_slug: instanda
slug: instanda-trust-center
source_filename: instanda-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nprobe: true\nurl: https://app.trustero.com/trust/instanda\nhosted_by: Trustero (third-party trust-centre platform)\nfirst_party_security_page: https://instanda.com/platform-security\nhttp_status: 200\nmachine_readable: false\nnote: >-\n  The Trustero trust centre is linked from the instanda.com footer and returns\n  HTTP 200, but it is a client-rendered React application - the served HTML is an\n  empty shell with the title \"Trustero\" and no certification text, so its contents\n  cannot be harvested without executing JavaScript. The certifications recorded\n  below are therefore taken from INSTANDA's own first-party security page at\n  instanda.com/platform-security, not scraped from Trustero.\ncertifications:\n- ISO 27001:2022\n- SOC 2\n- Cyber Essentials\n- PCI DSS SAQ A\ncontrols_published:\n  encryption_at_rest: AES-256 (Azure full disk encryption)\n  encryption_in_transit: AES-256 SSL certificates\n  siem: true\n  dlp: true\n\
  \  waf: machine-learning web application firewall\n  firewall: next-generation firewall with SSL VPN, deep-packet inspection, intrusion detection/prevention\n  ssdlc: >-\n    \"Our Secure Software Development Lifecycle (SSDLC) includes secure code\n    reviews, vulnerability assessments, full penetration testing, and threat\n    modeling.\"\n  hosting: Microsoft Azure\n  data_residency: client data stored in required geographies to meet regional regulations\ngaps:\n  security_contact_published: false\n  vulnerability_disclosure_policy: false\n  security_txt: false\n  subprocessor_list_public: false\n  audit_reports_downloadable: false\n  note: >-\n    No security@ address, no responsible-disclosure or bug-bounty page, and no\n    RFC 9116 security.txt was found on any INSTANDA host. Named certifications\n    are claimed but no report or certificate is publicly downloadable.\nevidence:\n- source: https://instanda.com/platform-security\n  status: 200\n  kind: first-party-security-page\n\
  \  keywords: [iso 27001:2022, soc 2, cyber essentials, pci dss saq a, ssdlc, penetration testing, siem, dlp, waf]\n- source: https://app.trustero.com/trust/instanda\n  status: 200\n  kind: hosted-trust-center\n  keywords: []\n  note: JavaScript-rendered shell; no keywords extractable from served HTML.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instanda/refs/heads/main/security/instanda-trust-center.yml
summary_line: ISO 27001:2022, SOC 2, Cyber Essentials, PCI DSS SAQ A
tags:
- Insurance
- United Kingdom
- Insurtech
- Policy Administration
- Underwriting
- Claims
- Property and Casualty
- Life Insurance
- Health Insurance
- Digital Distribution
- No-Code
- Core Systems
- MGA
- Brokers
- Webhook
- Microsoft Azure
- Embedded Insurance
trust_url: https://app.trustero.com/trust/instanda
---
