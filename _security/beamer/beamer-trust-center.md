---
certification_count: 2
certifications:
- SOC 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Beamer Trust Center
name_suffix: Trust Center
overview: Beamer maintains a public trust center documenting SOC 2 and GDPR compliance.
provider_name: Beamer
provider_slug: beamer
slug: beamer-trust-center
source_filename: beamer-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nprobe: true\nsource: https://www.getbeamer.com/security\nurl: https://trust.userflow.com/\nlegacy_url: https://trust.getbeamer.com/\nredirect_note: >-\n  trust.getbeamer.com 301s to trust.userflow.com — a Vanta-hosted trust center titled \"Userflow Trust\n  Center\". Beamer and Userflow now operate as one company, and the trust surface has been consolidated\n  on the Userflow domain; Beamer's own footer and navigation still link to it as Beamer's Trust Center.\ntrust_center_platform: Vanta\ncertifications:\n  - SOC 2\n  - GDPR\nsecurity_practices:\n  source: https://www.getbeamer.com/security\n  encryption_in_transit: 'TLS, 2,048-bit keys or better'\n  encryption_at_rest: 'AES-256 with integrity'\n  backups: 'Customer data is always backed up'\n  uptime_claim: 'over 99.9%'\n  penetration_testing: 'Third party network, application and physical security tests conducted regularly'\n  gdpr: 'GDPR compliant, Data Processing Agreements in\
  \ place'\n  data_ownership: 'Account and data belong to the customer and are not sold; deletion on request'\nrelated:\n  vulnerability_disclosure: security/beamer-vulnerability-disclosure.yml\n  privacy_endpoint: 'DELETE /privacy — the API surface for GDPR erasure'\nevidence:\n  - source: https://www.getbeamer.com/security\n    http_status: 200\n  - source: https://www.getbeamer.com/bug-bounty-program\n    http_status: 200\n  - source: https://trust.getbeamer.com/\n    http_status: 301\n    redirects_to: https://trust.userflow.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beamer/refs/heads/main/security/beamer-trust-center.yml
summary_line: SOC 2, GDPR
tags:
- Changelog
- Deprecation
- Notification
- Product Updates
- User Engagement
- Webhook
- NPS
- Feedback
trust_url: https://trust.userflow.com/
---
