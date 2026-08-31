---
api_specs:
- filename: starbridge-bridges-api-openapi.yml
  format: yaml
  label: Starbridge Bridges API
  slug: starbridge-bridges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-bridges-api-openapi.yml
- filename: starbridge-buyer-api-openapi.yml
  format: yaml
  label: Starbridge Buyer API
  slug: starbridge-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-buyer-api-openapi.yml
- filename: starbridge-columns-api-openapi.yml
  format: yaml
  label: Starbridge Columns API
  slug: starbridge-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-columns-api-openapi.yml
- filename: starbridge-external-mcp-api-openapi.yml
  format: yaml
  label: Starbridge External MCP API
  slug: starbridge-external-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-external-mcp-api-openapi.yml
- filename: starbridge-signal-api-openapi.yml
  format: yaml
  label: Starbridge Signal API
  slug: starbridge-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-signal-api-openapi.yml
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Starbridge Trust Center
name_suffix: Trust Center
overview: Starbridge maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Starbridge
provider_slug: starbridge
slug: starbridge-trust-center
source_filename: starbridge-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://trust.starbridge.ai/ (HTTP 200) +\n  https://starbridge.ai/blog/starbridge-is-soc-2-type-ii-certified\n# Trust center. probe-security-programs.py did not find this surface (it reported\n# trust=none) because trust.starbridge.ai is not linked from the paths it walks and\n# the page is a JS-rendered Vanta app; it was found by direct subdomain probe.\ntrust_center:\n  url: https://trust.starbridge.ai/\n  http_status: 200\n  platform: Vanta\n  platform_evidence: >-\n    Response HTML is the Vanta trust-report bundle — canonical\n    https://trust.starbridge.ai, assets under assets.vanta.com/static/vite/,\n    og:image https://app.vanta.com/doc?s=..., title \"Starbridge Trust Center\".\n  machine_readable: false\n  machine_readable_note: >-\n    The page renders entirely client-side from a signed Vanta API response; there is\n    no unauthenticated JSON endpoint, so the live control/certification list could not\n \
  \   be read. Certifications below are recorded ONLY from Starbridge's own published\n    announcement, not from the trust center itself.\n  checked: '2026-08-14'\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  scope: security, availability, confidentiality\n  announced: '2026-01-13'\n  auditor: not published\n  report_period: not published\n  evidence: https://starbridge.ai/blog/starbridge-is-soc-2-type-ii-certified\n  method: searched\n  note: >-\n    Starbridge's own blog announces SOC 2 Type II certification, describing\n    \"strong safeguards around security, availability, and confidentiality\" verified\n    over an extended audit period. No auditor, report date or period is named\n    publicly, and the report itself is not offered for download without a request.\nframeworks_not_claimed:\n- ISO 27001\n- HIPAA\n- FedRAMP\n- PCI DSS\n- StateRAMP\n- TX-RAMP\n- GDPR (no dedicated public page found)\n- FERPA (no dedicated public page found)\nnotes: >-\n  Starbridge sells\
  \ into K-12, higher education and government, where StateRAMP /\n  TX-RAMP / FERPA posture is routinely asked for in procurement. None of those is\n  publicly claimed. There is no public link from starbridge.ai to\n  trust.starbridge.ai that this pass could find — /security, /trust and\n  /trust-center all return 404 — so the trust center is effectively unlisted.\nreport_access:\n  self_serve_download: false\n  mechanism: Request through the Vanta trust center (NDA/approval flow) or via support@starbridge.ai\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/security/starbridge-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Artificial Intelligence
- Sales Intelligence
- Go-To-Market
- Public Sector
- Education
- Government
- Procurement
- Buyer Intelligence
- MCP
trust_url: ''
---
