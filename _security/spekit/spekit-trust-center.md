---
api_specs:
- filename: spekit-searches-api-openapi.yml
  format: yaml
  label: Spekit Searches API
  slug: spekit-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-searches-api-openapi.yml
- filename: spekit-spek-reactions-api-openapi.yml
  format: yaml
  label: Spekit Spek Reactions API
  slug: spekit-spek-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-spek-reactions-api-openapi.yml
- filename: spekit-spek-views-api-openapi.yml
  format: yaml
  label: Spekit Spek Views API
  slug: spekit-spek-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-spek-views-api-openapi.yml
- filename: spekit-user-activities-api-openapi.yml
  format: yaml
  label: Spekit User Activities API
  slug: spekit-user-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-user-activities-api-openapi.yml
- filename: spekit-users-api-openapi.yml
  format: yaml
  label: Spekit Users API
  slug: spekit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-users-api-openapi.yml
certifications:
- SOC 2
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Spekit Trust Center
name_suffix: Trust Center
overview: Spekit maintains a public trust center documenting SOC 2 and ISO 27001 compliance.
provider_name: Spekit
provider_slug: spekit
slug: spekit-trust-center
source_filename: spekit-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://trust.spekit.com/\nurl: https://trust.spekit.com/\nplatform: Drata (trust.spekit.com is a CNAME to trust.cname.drata.com)\ncertifications:\n- name: SOC 2\n  status: confirmed\n  detail: >-\n    SOC 2 Type II. Independently corroborated outside the trust center — Spekit's own llms.txt\n    states \"SOC 2 Type II\", https://www.spekit.com/security carries the audit announcement\n    (auditor Dansa D'Arata Soucia LLP), and the MCP security FAQ cites a company-wide SOC 2\n    Type II report covering the platform and security controls.\n- name: ISO 27001\n  status: single-probe\n  detail: >-\n    Matched once by probe-security-programs.py in the trust.spekit.com body on 2026-08-14. NOT\n    reproducible on re-probe (see access below), and Spekit does not claim ISO 27001 anywhere on\n    its public marketing, security page or llms.txt — those say SOC 2 Type II and GDPR-aligned\n    practices only. Recorded as\
  \ observed-once, not asserted as a held certification. Re-verify\n    before quoting.\naccess:\n  reproducible: false\n  http_status: 403\n  reason: cloudflare-bot-challenge\n  detail: >-\n    Same-day re-probes of https://trust.spekit.com/ from curl and python-urllib across several\n    user agents all returned HTTP 403 with `cf-mitigated: challenge` and a \"Just a moment...\"\n    interstitial requiring JavaScript and cookies. The trust center is public to a browser but\n    is not machine-readable; a scored catalog cannot re-verify the certification list on demand.\n  checked: '2026-08-14'\nreferenced_from:\n- https://www.spekit.com/security\n- https://www.spekit.com/llms.txt\n- https://help.spekit.com/hc/en-us/articles/53991678945435-Spekit-MCP-Data-Privacy-Security-FAQs\nevidence:\n- source: https://trust.spekit.com/\n  keywords:\n  - soc 2\n  - soc2\n  - iso 27001\n  - trust center\n  note: single successful fetch, 2026-08-14, not reproducible\n- source: https://www.spekit.com/security\n\
  \  http_status: 200\n  keywords: [soc 2, soc 2 type ii]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/security/spekit-trust-center.yml
summary_line: SOC 2, ISO 27001
tags:
- Company
- Software-as-a-Service
- Sales Enablement
- Revenue Enablement
- Digital Adoption
- Knowledge-Management
- MCP
- Artificial Intelligence
- Analytics
- Sales
- Content Management
- Agents
- Authentication
trust_url: https://trust.spekit.com/
---
