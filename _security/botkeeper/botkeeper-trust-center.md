---
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Botkeeper Trust Center
name_suffix: Trust Center
overview: Botkeeper maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Botkeeper
provider_slug: botkeeper
slug: botkeeper-trust-center
source_filename: botkeeper-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://trust.botkeeper.com/\nname: Botkeeper Trust Center\ntrust_center:\n  published: true\n  url: https://trust.botkeeper.com/\n  platform: first-party page on botkeeper.com infrastructure (not Vanta/Drata/SafeBase)\n  linked_from:\n    - https://www.botkeeper.com/ (footer, \"Security Protocols\")\n    - https://www.botkeeper.com/legal\n\ncertifications:\n  - name: SOC 2 Type 2\n    status: maintained\n    evidence: >-\n      \"Botkeeper Maintains SOC 2 Type 2 Accreditation\" — annually renewed, with\n      continuous control testing.\n    url: https://trust.botkeeper.com/\n    report_available: not stated on the public page\n  # No ISO 27001, PCI DSS, HIPAA, FedRAMP, CSA STAR or GDPR certification is\n  # claimed anywhere on the trust center. Absence recorded deliberately.\n\ncontrol_families_published:\n  - name: App Security\n    controls: [penetration testing, code review, secure development lifecycle]\n  - name: Data\
  \ Security\n    controls: [encryption at rest, SSL/TLS in transit, daily backups]\n  - name: Infrastructure Security\n    controls: [cloud storage restrictions, SSO, automatic patching]\n  - name: Network Security\n    controls: [malware detection, access controls]\n  - name: Organization Security\n    controls: [incident response plan, disaster recovery, security awareness training]\n  - name: Product Security\n    controls: [multi-factor authentication, database monitoring, session locks]\n\npractices:\n  penetration_testing: annual\n  data_residency: AWS data centers in the United States\n  ip_ownership: Botkeeper states it owns its intellectual property\n\ngaps:\n  - No subprocessor list published\n  - No downloadable report / document request flow (SOC 2 report availability not stated)\n  - No DPA linked from the trust center or the legal page\n  - No RFC 9116 security.txt pointing at the trust center or the VDP\n\nrelated:\n  vulnerability_disclosure: security/botkeeper-vulnerability-disclosure.yml\n\
  \  privacy_policy: https://www.botkeeper.com/legal#privacy\n  terms: https://www.botkeeper.com/legal\n\nx-evidence:\n  fetched: '2026-08-08'\n  probes:\n    - url: https://trust.botkeeper.com/\n      status: 200\n      content_type: text/html\n    - url: https://www.botkeeper.com/legal\n      status: 200\n      content_type: text/html; charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botkeeper/refs/heads/main/security/botkeeper-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Company
- Accounting
- Bookkeeping
- Financial Services
- Artificial Intelligence
- Automation
- SaaS
- Banking Data
- Practice Management
- Small Business
trust_url: ''
---
