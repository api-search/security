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
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zype.com
  spf: true
hosts:
- cert_expires: Nov  7 05:54:04 2026 GMT
  host: www.zype.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 10:46:48 2026 GMT
  host: analytics.zype.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 11:16:06 2026 GMT
  host: api.zype.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zype Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zype, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zype
provider_slug: zype
slug: zype-domain-security
source_filename: zype-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zype.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 05:54:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: analytics.zype.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 10:46:48 2026 GMT\n  hsts: null\n- host: api.zype.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:16:06 2026 GMT\n  hsts: null\ndomains:\n- domain: zype.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/security/zype-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
---
