---
certifications: []
description: ''
kind: trust-center
layout: security
name: Vendelux Trust Center
name_suffix: Trust Center
overview: Vendelux maintains a public trust center covering its security and compliance posture.
provider_name: Vendelux
provider_slug: vendelux
slug: vendelux-trust-center
source_filename: vendelux-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://vendelux.com/privacy — the Vendelux Privacy Policy (effective 2026-05-04) states that\n  details of Vendelux's security practices are available at the \"Vendelux Trust Center\"\n  (https://trust.vendelux.com/). The same URL is linked three times from the vendelux.com footer.\ntrust_center:\n  url: https://trust.vendelux.com/\n  present: true\n  platform: Drata\n  platform_evidence: >-\n    DNS CNAME trust.vendelux.com -> trust.cname.drata.com. — the hostname is delegated to Drata's\n    hosted Trust Center product, which is what establishes that this is a real, provider-operated\n    compliance surface rather than a marketing page.\n  http_status: 403\n  http_status_note: >-\n    The page could not be read. Cloudflare returned a managed bot challenge (HTTP 403 with the\n    response header `cf-mitigated: challenge` and the \"Just a moment...\" interstitial). Per the\n    pipeline contract a bot challenge is NOT\
  \ a dead pointer: the page demonstrably exists — it is\n    delegated to Drata in DNS and cited by Vendelux's own privacy policy — and only our crawler was\n    turned away. We do not evade challenges.\ncertifications: []\ncertifications_note: >-\n  NOT READ, not absent. The specific certifications Vendelux lists (SOC 2, ISO 27001 or otherwise)\n  are behind the bot challenge above and were not observed, so none are asserted here. Drata Trust\n  Centers conventionally publish a framework list and allow NDA-gated report requests, but that is a\n  property of the product, not an observation about Vendelux, and it is not recorded as one.\nrelated_documents:\n- name: Privacy Policy\n  url: https://vendelux.com/privacy\n  effective: '2026-05-04'\n  status: 200\n- name: Subprocessors\n  url: https://vendelux.com/vendelux-subprocessors/\n  status: unverified\n  note: Cited by the Privacy Policy; not independently probed past the edge challenge.\n- name: Terms of Service\n  url: https://vendelux.com/terms\n\
  \  last_updated: '2024-02-07'\n  status: 200\n- name: Privacy statement for residents of certain states\n  url: https://vendelux.com/privacy-statement-for-residents-of-certain-states\n  status: unverified\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendelux/refs/heads/main/security/vendelux-trust-center.yml
summary_line: trust center published
tags:
- Event Intelligence
- Event Marketing
- B2B Events
- Marketing Intelligence
- Sales Intelligence
- Event Data
- CRM Integration
- Demand Generation
- Field Marketing
- Conference Data
- Company
trust_url: ''
---
