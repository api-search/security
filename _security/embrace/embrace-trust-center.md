---
certifications: []
description: 'Embrace runs a Vanta-hosted Trust Center at trust.embrace.io, with a Controls section. The page is a single-page app: the shell returns HTTP 200 with the title "Embrace Trust Center" and the keywords "Trust, Security, Compliance, Automation", but the certification list, control list and document requests are all client-rendered and are not reachable by an anonymous machine. No probed endpoint returned structured trust data — every path under trust.embrace.io returns the same HTML shell.'
kind: trust-center
layout: security
name: Embrace Trust Center
name_suffix: Trust Center
overview: Embrace maintains a public trust center covering its security and compliance posture.
provider_name: Embrace
provider_slug: embrace
slug: embrace-trust-center
source_filename: embrace-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nprobe: true\nurl: https://trust.embrace.io/\nsource: https://trust.embrace.io/\nplatform: Vanta\ndescription: >-\n  Embrace runs a Vanta-hosted Trust Center at trust.embrace.io, with a Controls section. The page\n  is a single-page app: the shell returns HTTP 200 with the title \"Embrace Trust Center\" and the\n  keywords \"Trust, Security, Compliance, Automation\", but the certification list, control list and\n  document requests are all client-rendered and are not reachable by an anonymous machine. No\n  probed endpoint returned structured trust data — every path under trust.embrace.io returns the\n  same HTML shell.\ncertifications: []\ncertifications_readable: false\nevidence:\n  - {source: 'https://trust.embrace.io/', status: 200, kind: html, signals: ['title: Embrace Trust Center', 'meta keywords: Trust, Security, Compliance, Automation', 'canonical: https://trust.embrace.io', 'Vanta asset host']}\n  - {source: 'https://trust.embrace.io/controls',\
  \ status: 200, kind: html, note: 'Controls section exists; contents are client-rendered.'}\n  - {source: 'https://trust.embrace.io/api/trust-page', status: 200, kind: html, note: 'Returns the SPA shell, not JSON — no anonymous machine-readable trust API.'}\nrelated:\n  privacy_policy: https://embrace.io/privacy/\n  terms_of_service: https://embrace.io/terms-of-service/\n  data_residency:\n    supported: true\n    regions: [us, eu]\n    hosts: [api-us1.embrace.io, api-eu1.embrace.io]\n    note: Regional data residency is a product feature, documented in the Metrics API pages.\n  privacy_docs:\n    - https://embrace.io/docs/ios/privacy/\nnote: >-\n  No 'Compliance' pointer is emitted in apis.yml. That check reads a published compliance program\n  with named certifications; Embrace's trust center exists but names none that a machine — or a\n  reader without JavaScript — can see. Publishing the certification list as static content, or\n  linking the named frameworks from embrace.io, would\
  \ convert this into a verifiable claim.\nwarning: >-\n  Do NOT confuse this company with embrace.ai, an unrelated firm whose SOC 2 Type II press release\n  surfaces on searches for \"Embrace SOC 2\". That certification belongs to embrace.ai and is not\n  attributed to Embrace (embrace.io) here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embrace/refs/heads/main/security/embrace-trust-center.yml
summary_line: trust center published
tags:
- Company
- Observability
- Monitoring
- Mobile
- Real User Monitoring
- OpenTelemetry
- Metrics
- Crash Reporting
- Application Performance Monitoring
- Developer Tools
- Model Context Protocol
trust_url: https://trust.embrace.io/
---
