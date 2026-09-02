---
api_specs:
- filename: videoamp-admeasurements-api-openapi.yml
  format: yaml
  label: VideoAmp Ad Measurements API
  slug: videoamp-admeasurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-admeasurements-api-openapi.yml
- filename: videoamp-audiences-api-openapi.yml
  format: yaml
  label: VideoAmp Audiences API
  slug: videoamp-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-audiences-api-openapi.yml
- filename: videoamp-campaigns-api-openapi.yml
  format: yaml
  label: VideoAmp Campaigns API
  slug: videoamp-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-campaigns-api-openapi.yml
- filename: videoamp-consents-api-openapi.yml
  format: yaml
  label: VideoAmp Consents API
  slug: videoamp-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-consents-api-openapi.yml
- filename: videoamp-content-api-openapi.yml
  format: yaml
  label: VideoAmp Content API
  slug: videoamp-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-content-api-openapi.yml
- filename: videoamp-currency-of-record-api-openapi.yml
  format: yaml
  label: VideoAmp Currency Of Record API
  slug: videoamp-currency-of-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-currency-of-record-api-openapi.yml
- filename: videoamp-datastreams-api-openapi.yml
  format: yaml
  label: VideoAmp Data Streams API
  slug: videoamp-datastreams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-datastreams-api-openapi.yml
- filename: videoamp-datastreamtypes-api-openapi.yml
  format: yaml
  label: VideoAmp Data Stream Types API
  slug: videoamp-datastreamtypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-datastreamtypes-api-openapi.yml
- filename: videoamp-inventories-api-openapi.yml
  format: yaml
  label: VideoAmp Inventories API
  slug: videoamp-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-inventories-api-openapi.yml
- filename: videoamp-library-api-openapi.yml
  format: yaml
  label: VideoAmp Library API
  slug: videoamp-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-library-api-openapi.yml
- filename: videoamp-me-api-openapi.yml
  format: yaml
  label: VideoAmp Me API
  slug: videoamp-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-me-api-openapi.yml
- filename: videoamp-plans-api-openapi.yml
  format: yaml
  label: VideoAmp Plans API
  slug: videoamp-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-plans-api-openapi.yml
- filename: videoamp-reports-api-openapi.yml
  format: yaml
  label: VideoAmp Reports API
  slug: videoamp-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-reports-api-openapi.yml
- filename: videoamp-shares-api-openapi.yml
  format: yaml
  label: VideoAmp Shares API
  slug: videoamp-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-shares-api-openapi.yml
certifications: []
description: VideoAmp operates a Vanta-hosted trust center at trust.videoamp.com. The host resolves and returns HTTP 200, and the served document is a Vanta trust report shell (data-signature-manifest-url on assets.vanta.com, meta keywords "Trust, Security, Compliance, Automation", slug id kc0vaj770r912yhumz0k2). The page body is rendered entirely client-side, so the certification list, subprocessor list and document library could not be read anonymously.
kind: trust-center
layout: security
name: Videoamp Trust Center
name_suffix: Trust Center
overview: VideoAmp maintains a public trust center covering its security and compliance posture.
provider_name: VideoAmp
provider_slug: videoamp
slug: videoamp-trust-center
source_filename: videoamp-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nprobe: true\nurl: https://trust.videoamp.com/\nplatform: Vanta\ndescription: >-\n  VideoAmp operates a Vanta-hosted trust center at trust.videoamp.com. The host resolves and returns\n  HTTP 200, and the served document is a Vanta trust report shell (data-signature-manifest-url on\n  assets.vanta.com, meta keywords \"Trust, Security, Compliance, Automation\", slug id\n  kc0vaj770r912yhumz0k2). The page body is rendered entirely client-side, so the certification list,\n  subprocessor list and document library could not be read anonymously.\ncertifications: []\ncertifications_note: >-\n  NOT verified. The 3.5 KB HTML shell served to an anonymous fetch contains no certification names.\n  Reading the actual compliance posture requires a JavaScript-rendering client or a Vanta access\n  request. Do not assert SOC 2 / ISO 27001 / HIPAA / PCI for VideoAmp on the basis of this artifact.\ndocuments_gated: true\nevidence:\n  - source: https://trust.videoamp.com/\n\
  \    http_status: 200\n    content_type: text/html\n    keywords: [trust, security, compliance]\n    platform_markers:\n      - assets.vanta.com/static/index-trust-report.css\n      - data-signature-manifest-url=https://assets.vanta.com/static/signature-manifest...\n      - data-slugid=kc0vaj770r912yhumz0k2\n  - source: https://trust.videoamp.com/.well-known/security.txt\n    http_status: 200\n    content_type: text/html\n    valid: false\n    note: SPA catch-all returns the same HTML shell for every path — not a real security.txt.\nrelated:\n  vulnerability_disclosure: security/videoamp-vulnerability-disclosure.yml\nx-evidence:\n  fetched: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/security/videoamp-trust-center.yml
summary_line: trust center published
tags:
- Media Measurement
- Advertising
- AdTech
- tv-currency
- Audience Measurement
- Media Planning
- Streaming
- Attribution
- Data Collaboration
- MCP
- agent-native
trust_url: https://trust.videoamp.com/
---
