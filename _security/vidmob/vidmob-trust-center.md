---
api_specs:
- filename: vidmob-media-api-openapi.yml
  format: yaml
  label: VidMob Media API
  slug: vidmob-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-media-api-openapi.yml
- filename: vidmob-organization-api-openapi.yml
  format: yaml
  label: VidMob Organization API
  slug: vidmob-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-organization-api-openapi.yml
- filename: vidmob-scoring-api-openapi.yml
  format: yaml
  label: VidMob Scoring API
  slug: vidmob-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-scoring-api-openapi.yml
- filename: vidmob-workspaces-api-openapi.yml
  format: yaml
  label: VidMob Workspaces API
  slug: vidmob-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-workspaces-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Vidmob Trust Center
name_suffix: Trust Center
overview: VidMob maintains a public trust center covering its security and compliance posture.
provider_name: VidMob
provider_slug: vidmob
slug: vidmob-trust-center
source_filename: vidmob-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nprobe: true\nurl: https://trust.vidmob.com/\nplatform: Vanta\ntitle: Vidmob Trust Center\nslug_id: fji5cwrwf92zqikpc6ob2u\ncertifications: []\ncertifications_readable: false\ndetail: >-\n  trust.vidmob.com resolves and returns HTTP 200 with a canonical link to https://trust.vidmob.com, the page title\n  \"Vidmob Trust Center\", and the Vanta trust-report bundle\n  (https://assets.vanta.com/static/index-trust-report.*.js). The trust center is therefore genuinely published on\n  Vidmob's own subdomain. Its CONTENT — the certification list, controls and document requests — is rendered entirely\n  client-side from an authenticated Vanta API (api.vanta.com trust-report paths all return 401 anonymously), so no\n  named certification could be verified. Nothing is asserted here that was not observed: certifications is\n  deliberately empty rather than populated from marketing copy. Consequently no `Compliance` pointer is wired in\n  apis.yml\
  \ — a trust center that exists is not the same as a certification that was verified.\n  0-working/probe-security-programs.py reports trust=none for the same reason: its keyword check reads the served\n  HTML, which carries no compliance keywords.\nrelated:\n  mcp_security_overview: https://help.vidmob.com/en/articles/15461399-vidmob-mcp-security-compliance-overview\n  note: >-\n    Vidmob does publish a detailed, plainly-written security and access-control overview for its MCP integration aimed\n    at vendor security reviews — covering authentication, tenancy isolation, input validation, rate limiting, audit\n    logging and transport security, with each control tagged implemented / rolling out / planned. It names no\n    third-party certification.\nevidence:\n  - source: https://trust.vidmob.com/\n    http_status: 200\n    signals: [canonical trust.vidmob.com, 'title: Vidmob Trust Center', vanta trust-report bundle]\n  - source: https://api.vanta.com/v1/trust-report/fji5cwrwf92zqikpc6ob2u\n\
  \    http_status: 401\n    signals: [anonymous read of the trust report is gated]\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://trust.vidmob.com/\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/security/vidmob-trust-center.yml
summary_line: trust center published
tags:
- Creative Intelligence
- creative-data
- Advertising
- Marketing
- Media Measurement
- Video
- Computer-Vision
- Creative Analytics
- AdTech
- MCP
- agent-native
- MarTech
trust_url: https://trust.vidmob.com/
---
