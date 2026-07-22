---
api_specs:
- filename: wayflyer-embedded-finance-openapi-original.json
  format: json
  label: Wayflyer Embedded Finance API
  slug: embedded-finance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-embedded-finance-openapi-original.json
- filename: wayflyer-embedded-finance-sandbox-openapi-original.json
  format: json
  label: Wayflyer Embedded Finance Sandbox API
  slug: embedded-finance-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-embedded-finance-sandbox-openapi-original.json
certifications: []
description: Wayflyer operates a public trust center at trust.wayflyer.com (HTTP 200 at probe time), hosted on Vanta's trust-report platform (page title "Wayflyer Trust Center"; page loads Vanta trust-report assets from assets.vanta.com). The content is JavaScript-rendered, so the automated keyword probe (probe-security-programs.py) could not extract the certification list — named certifications are therefore NOT recorded here rather than guessed. No Compliance rating pointer is emitted until a published certification list is verified.
kind: trust-center
layout: security
name: Wayflyer Trust Center
name_suffix: Trust Center
overview: Wayflyer maintains a public trust center covering its security and compliance posture.
provider_name: Wayflyer
provider_slug: wayflyer
slug: wayflyer-trust-center
source_filename: wayflyer-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nurl: https://trust.wayflyer.com/\nplatform: Vanta Trust Center\ndescription: >-\n  Wayflyer operates a public trust center at trust.wayflyer.com (HTTP 200 at\n  probe time), hosted on Vanta's trust-report platform (page title \"Wayflyer\n  Trust Center\"; page loads Vanta trust-report assets from assets.vanta.com).\n  The content is JavaScript-rendered, so the automated keyword probe\n  (probe-security-programs.py) could not extract the certification list —\n  named certifications are therefore NOT recorded here rather than guessed.\n  No Compliance rating pointer is emitted until a published certification\n  list is verified.\ncertifications: []\ncertifications_note: not extractable from the JS-rendered Vanta app at probe time; none asserted\nevidence:\n  - source: https://trust.wayflyer.com/\n    kind: trust-center\n    detail: 'HTTP 200; <title>Wayflyer Trust Center</title>; Vanta index-trust-report.* assets'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/security/wayflyer-trust-center.yml
summary_line: trust center published
tags:
- Company
- Ecommerce
- Fintech
- Embedded Finance
- Lending
- Revenue-Based Financing
- Financing
trust_url: https://trust.wayflyer.com/
---
