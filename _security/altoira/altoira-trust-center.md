---
api_specs:
- filename: altoira-handoffs-api-openapi.yml
  format: yaml
  label: AltoIRA Handoffs API
  slug: altoira-handoffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-handoffs-api-openapi.yml
- filename: altoira-investment-api-openapi.yml
  format: yaml
  label: AltoIRA Investment API
  slug: altoira-investment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-investment-api-openapi.yml
- filename: altoira-oauth-api-openapi.yml
  format: yaml
  label: AltoIRA OAUTH API
  slug: altoira-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-oauth-api-openapi.yml
- filename: altoira-offering-api-openapi.yml
  format: yaml
  label: AltoIRA Offering API
  slug: altoira-offering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-offering-api-openapi.yml
- filename: altoira-user-api-openapi.yml
  format: yaml
  label: AltoIRA User API
  slug: altoira-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-user-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Altoira Trust Center
name_suffix: Trust Center
overview: AltoIRA maintains a public trust center covering its security and compliance posture.
provider_name: AltoIRA
provider_slug: altoira
slug: altoira-trust-center
source_filename: altoira-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nprobe: true\nurl: https://trust.altoira.com/\ntitle: Alto Trust Center\nplatform: Vanta\ncertifications: []\ncertifications_readable: false\ndetail: >-\n  Alto publishes a trust center at trust.altoira.com. It is verified live: the\n  host CNAMEs to Vanta (68cc37f32db8854ae217e531.cname.vantatrust.com), returns\n  HTTP 200, and the served HTML carries <title>Alto Trust Center</title>, a\n  canonical link to https://trust.altoira.com, and og:description \"The secure\n  self-directed IRA platform for all your alternatives\". The page body is a\n  client-rendered Vanta single-page application — the 6.6KB HTML shell contains\n  no certification names — and Vanta's backing API (api.vanta.com/v1/trust-pages)\n  returns 401 to an anonymous caller. Requests to trust.altoira.com under any\n  guessed API path return the SPA shell with a 200 (soft-404), which is not\n  evidence of an endpoint.\n  Consequence: API Evangelist can confirm the trust\
  \ center EXISTS but cannot read\n  any named certification (SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP) from it\n  without a browser. No certification is therefore asserted, and no `Compliance`\n  pointer is wired in apis.yml. A grep of altoira.com's homepage, about, FAQ,\n  legal, contact and Alto Trust Company pages found no named certification\n  either.\n  This is a provider-fixable gap: serving the certification list as static HTML\n  or exposing an anonymous JSON view would make Alto's compliance posture\n  machine-readable.\nevidence:\n- source: https://trust.altoira.com/\n  http_status: 200\n  content_type: text/html\n  keywords:\n  - Alto Trust Center\n  - Trust, Security, Compliance, Automation\n  note: JS-rendered Vanta SPA; certification names not present in the served HTML.\n- source: https://api.vanta.com/v1/trust-pages/pgbmbtllndywbuh6bxxjo\n  http_status: 401\n  note: Vanta trust-page data API rejects anonymous requests.\n- source: dig trust.altoira.com\n  result: 68cc37f32db8854ae217e531.cname.vantatrust.com\n\
  x-evidence:\n  fetched: '2026-08-06'\n  url: https://trust.altoira.com/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/security/altoira-trust-center.yml
summary_line: trust center published
tags:
- Company
- Financial Services
- Retirement
- Self-Directed IRA
- Alternative Investments
- Private Markets
- Fintech
- Custody
- Cryptocurrency
- Wealth Management
- Investing
- Capital Raising
trust_url: https://trust.altoira.com/
---
