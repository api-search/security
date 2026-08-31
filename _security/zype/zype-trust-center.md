---
api_specs:
- filename: zype-platform.json
  format: json
  label: Zype Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-platform.json
- filename: zype-playout-scheduler.json
  format: json
  label: Zype Playout Scheduler API
  slug: playout-scheduler
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-playout-scheduler.json
- filename: zype-monetization.json
  format: json
  label: Zype Monetization API
  slug: monetization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-monetization.json
- filename: zype-consumers.json
  format: json
  label: Zype Consumers API
  slug: consumers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-consumers.json
- filename: zype-live-3.json
  format: json
  label: Zype Live API (V3)
  slug: live-3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-live-3.json
- filename: zype-zobjects.json
  format: json
  label: Zype Zobjects API
  slug: zobjects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-zobjects.json
- filename: zype-analytics-v3.json
  format: json
  label: Zype Analytics API (V3)
  slug: analytics-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-analytics-v3.json
- filename: zype-analytics.json
  format: json
  label: Zype Analytics API (V2)
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-analytics.json
- filename: zype-content-regions.json
  format: json
  label: Zype Custom Regions API
  slug: content-regions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-regions.json
- filename: zype-content-rule-groups.json
  format: json
  label: Zype Content Rule Groups API
  slug: content-rule-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-rule-groups.json
- filename: zype-content-rules.json
  format: json
  label: Zype Content Rule Profiles API
  slug: content-rules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-rules.json
- filename: zype-tve.json
  format: json
  label: Zype TVE API
  slug: tve
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-tve.json
- filename: zype-login.json
  format: json
  label: Zype Consumer Authentication API
  slug: login
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-login.json
- filename: zype-player.json
  format: json
  label: Zype Player API
  slug: player
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-player.json
- filename: zype-uploads.json
  format: json
  label: Zype Uploads API
  slug: uploads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-uploads.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Zype Trust Center
name_suffix: Trust Center
overview: Zype maintains a public trust center covering its security and compliance posture.
provider_name: Zype
provider_slug: zype
slug: zype-trust-center
source_filename: zype-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://trust.zype.com/ (HTTP 200) and https://www.zype.com/security-compliance (HTTP 200)\ntrust_center:\n  url: https://trust.zype.com\n  http_status: 200\n  platform: Laika / Thoropass Trust Center\n  machine_readable: false\n  note: trust.zype.com returns a 200 whose body is an 814-byte SPA shell (<title>Trust Center</title>, bundle served\n    from laika-app-prod.s3.amazonaws.com/static/trust-center/). The page is a genuine hosted trust center, but every\n    certificate, policy and sub-processor listing inside it is rendered client-side, so nothing on it is machine-readable\n    to a crawler or an agent. The readable substance lives on the HTML page at www.zype.com/security-compliance\n    instead.\npublic_compliance_page:\n  url: https://www.zype.com/security-compliance\n  http_status: 200\n  certifications:\n  - SOC 2 Type II\n  - PCI (self-certified)\n  - ISO 27001\n  - GDPR\n  - CCPA\n  sub_processors_disclosed: true\n\
  \  cloud_providers:\n  - Amazon Web Services\n  - Google Cloud Platform\n  payment_processors:\n  - Stripe\n  - Recurly\ndocuments_available_under_nda:\n- SOC 2 Type II report\n- PCI self-certification detail\n- Data Processing Agreement\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/security/zype-trust-center.yml
summary_line: trust center published
tags:
- Video
- Streaming
- OTT
- Video CMS
- FAST
- Linear TV
- Playout
- Monetization
- Live Streaming
- Analytics
- Media and Entertainment
- DRM
- Advertising
- Encoding
- EPG
trust_url: ''
---
