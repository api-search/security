---
api_specs:
- filename: tabs-external-api-openapi.yml
  format: yaml
  label: Tabs External API
  slug: tabs-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/openapi/tabs-external-api-openapi.yml
- filename: tabs-usage-api-beta-openapi.yml
  format: yaml
  label: Tabs Usage API (Beta)
  slug: tabs-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/openapi/tabs-usage-api-beta-openapi.yml
certifications:
- SOC 2
description: Tabs operates a trust center at trust.tabs.com (hosted on Responsive/RFPIO Profiles; JS-rendered, so the automated keyword probe could not read the body). The tabs.com site footer links to it as "Security" and displays a "SOC2 Compliant" badge in its published site data. An earlier SafeBase trust center at trust.tabs.inc no longer resolves.
kind: trust-center
layout: security
name: Tabs Trust Center
name_suffix: Trust Center
overview: Tabs maintains a public trust center documenting SOC 2 compliance.
provider_name: Tabs
provider_slug: tabs
slug: tabs-trust-center
source_filename: tabs-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nurl: https://trust.tabs.com/\ncertifications: [SOC 2]\ndescription: >-\n  Tabs operates a trust center at trust.tabs.com (hosted on Responsive/RFPIO\n  Profiles; JS-rendered, so the automated keyword probe could not read the\n  body). The tabs.com site footer links to it as \"Security\" and displays a\n  \"SOC2 Compliant\" badge in its published site data. An earlier SafeBase\n  trust center at trust.tabs.inc no longer resolves.\nevidence:\n  - source: https://www.tabs.com/ (site footer data)\n    keywords: [\"SOC2 Compliant\", \"Security -> https://trust.tabs.com/\"]\n  - source: https://trust.tabs.com/\n    note: Live (HTTP 200), titled \"Trust Center\"; content requires JS rendering\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/security/tabs-trust-center.yml
summary_line: SOC 2
tags:
- Billing
- Revenue Automation
- Accounts Receivable
- Revenue Recognition
- Usage-Based Billing
- Invoicing
- Collections
- Fintech
- SaaS
trust_url: https://trust.tabs.com/
---
