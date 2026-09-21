---
api_specs:
- filename: statable-stats-api-openapi.yml
  format: yaml
  label: Statable Stats API
  slug: statable-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statable-stats-api/refs/heads/main/openapi/statable-stats-api-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Statable Stats Api Trust Center
name_suffix: Trust Center
overview: Statable Stats API maintains a public trust center covering its security and compliance posture.
provider_name: Statable Stats API
provider_slug: statable-stats-api
slug: statable-stats-api-trust-center
source_filename: statable-stats-api-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nprobe: true\nsource: https://statable.com/security\nurl: https://statable.com/security\n# Statable (Key Arg B.V.) holds NO third-party audit certifications of its own.\n# Its published compliance posture is GDPR (EU/Netherlands jurisdiction) plus a DPA\n# and sub-processor disclosure. The SOC 2 / ISO 27001 / PCI DSS names on the security\n# page belong to its SUB-PROCESSORS (NorthC, Bunny, Stripe, Google), not to Statable\n# — recorded separately below so they are not miscredited to the provider.\ncertifications: []\ncompliance:\n  - id: GDPR\n    scope: EU/Netherlands jurisdiction; cookieless, no consent banner in most jurisdictions\n    evidence: https://statable.com/gdpr\n  - id: DPA\n    scope: Data Processing Agreement offered\n    evidence: https://statable.com/dpa\nsub_processor_certifications:\n  - vendor: NorthC Datacenters\n    holds: [ISO/IEC 27001, SOC 2 Type II]\n  - vendor: Bunny (CDN)\n    holds: [SOC 2 Type II, ISO/IEC\
  \ 27001:2022]\n  - vendor: Stripe (billing)\n    holds: [PCI DSS Level 1]\n  - vendor: Google\n    holds: [SOC 2, ISO 27001]\nevidence:\n  - source: https://statable.com/security\n    note: security policy + sub-processor disclosure page (JS-rendered)\n  - source: https://statable.com/services\n    note: sub-processor list\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statable-stats-api/refs/heads/main/security/statable-stats-api-trust-center.yml
summary_line: trust center published
tags:
- Analytics
- Web Analytics
- Cookieless
- Privacy
- GDPR
- OpenAPI
- MCP
- llms-txt
- EU-hosted
trust_url: https://statable.com/security
---
