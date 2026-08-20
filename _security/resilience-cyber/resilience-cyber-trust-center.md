---
certifications: []
description: ''
kind: trust-center
layout: security
name: Resilience Cyber Trust Center
name_suffix: Trust Center
overview: Resilience maintains a public trust center covering its security and compliance posture.
provider_name: Resilience
provider_slug: resilience-cyber
slug: resilience-cyber-trust-center
source_filename: resilience-cyber-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nprobe: true\nurl: https://trust.cyberresilience.com/\nplatform: Vanta\ntitle: Resilience Trust Center\nstatus: 200\nevidence:\n- source: https://trust.cyberresilience.com/\n  kind: html-head\n  detail: >-\n    <title>Resilience Trust Center</title>, canonical\n    https://trust.cyberresilience.com, keywords \"Trust, Security, Compliance,\n    Automation\", assets served from assets.vanta.com\n    (index-trust-report.*.js/css) — a Vanta trust-report deployment.\ncertifications: []\ncertifications_enumerable: false\nnote: >-\n  The trust center is real and reachable, but the page body is a 4.2 KB\n  single-page-app shell: all content is fetched client-side by an Apollo GraphQL\n  client using Vanta's signed-query mechanism, so no certification list,\n  subprocessor list, control list or document-request surface can be read\n  anonymously with an HTTP client. Certifications are left EMPTY on purpose —\n  naming SOC 2 or ISO 27001 here\
  \ without fetching them would be fabrication.\n  Beware the near-name collision when searching: trust.resilience.care is a\n  different company (National Resilience / Resilience health), not this carrier.\n  Upgrading this artifact requires a rendered fetch of trust.cyberresilience.com.\nrelated:\n  conformance: conformance/resilience-cyber-conformance.yml\n  domain_security: security/resilience-cyber-domain-security.yml\nvulnerability_disclosure:\n  published: false\n  note: >-\n    Probed 2026-07-25: no RFC 9116 security.txt on cyberresilience.com,\n    trust.cyberresilience.com or portal.cyberresilience.com; /security,\n    /responsible-disclosure, /vulnerability-disclosure and /compliance all\n    soft-404 to the WordPress homepage; hackerone.com/cyberresilience and\n    bugcrowd.com/cyberresilience both 404. No public disclosure program or\n    security contact was found for a company whose product is cyber risk.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resilience-cyber/refs/heads/main/security/resilience-cyber-trust-center.yml
summary_line: trust center published
tags:
- Insurance
- United States
- Cyber Insurance
- Property and Casualty
- Insurtech
- Underwriting
- Claims
- Risk Data
- Technology Errors and Omissions
- Brokers
- Specialty Insurance
trust_url: https://trust.cyberresilience.com/
---
