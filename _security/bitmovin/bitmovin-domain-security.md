---
api_specs:
- filename: bitmovin-config-api-openapi.yml
  format: yaml
  label: Bitmovin Config API
  slug: bitmovin-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-config-api-openapi.yml
- filename: bitmovin-configurations-api-openapi.yml
  format: yaml
  label: Bitmovin Configurations API
  slug: bitmovin-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-configurations-api-openapi.yml
- filename: bitmovin-emails-api-openapi.yml
  format: yaml
  label: Bitmovin Emails API
  slug: bitmovin-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-emails-api-openapi.yml
- filename: bitmovin-encodings-api-openapi.yml
  format: yaml
  label: Bitmovin Encodings API
  slug: bitmovin-encodings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-encodings-api-openapi.yml
- filename: bitmovin-filters-api-openapi.yml
  format: yaml
  label: Bitmovin Filters API
  slug: bitmovin-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-filters-api-openapi.yml
- filename: bitmovin-infrastructure-api-openapi.yml
  format: yaml
  label: Bitmovin Infrastructure API
  slug: bitmovin-infrastructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-infrastructure-api-openapi.yml
- filename: bitmovin-inputs-api-openapi.yml
  format: yaml
  label: Bitmovin Inputs API
  slug: bitmovin-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-inputs-api-openapi.yml
- filename: bitmovin-live-api-openapi.yml
  format: yaml
  label: Bitmovin Live API
  slug: bitmovin-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-live-api-openapi.yml
- filename: bitmovin-manifests-api-openapi.yml
  format: yaml
  label: Bitmovin Manifests API
  slug: bitmovin-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-manifests-api-openapi.yml
- filename: bitmovin-notifications-api-openapi.yml
  format: yaml
  label: Bitmovin Notifications API
  slug: bitmovin-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-notifications-api-openapi.yml
- filename: bitmovin-outputs-api-openapi.yml
  format: yaml
  label: Bitmovin Outputs API
  slug: bitmovin-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-outputs-api-openapi.yml
- filename: bitmovin-search-api-openapi.yml
  format: yaml
  label: Bitmovin Search API
  slug: bitmovin-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-search-api-openapi.yml
- filename: bitmovin-signing-keys-api-openapi.yml
  format: yaml
  label: Bitmovin Signing-keys API
  slug: bitmovin-signing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-signing-keys-api-openapi.yml
- filename: bitmovin-templates-api-openapi.yml
  format: yaml
  label: Bitmovin Templates API
  slug: bitmovin-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-templates-api-openapi.yml
- filename: bitmovin-video-api-openapi.yml
  format: yaml
  label: Bitmovin Video API
  slug: bitmovin-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-video-api-openapi.yml
- filename: bitmovin-webhooks-api-openapi.yml
  format: yaml
  label: Bitmovin Webhooks API
  slug: bitmovin-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitmovin.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: bitmovin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 02:54:23 2026 GMT
  host: developer.bitmovin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:30:54 2026 GMT
  host: api.bitmovin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitmovin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitmovin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bitmovin
provider_slug: bitmovin
slug: bitmovin-domain-security
source_filename: bitmovin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitmovin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: developer.bitmovin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:54:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bitmovin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:30:54 2026 GMT\n  hsts: null\ndomains:\n- domain: bitmovin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/security/bitmovin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Encoding
- Streaming
- Live Streaming
- VOD
- Adaptive Bitrate
- HLS
- DASH
- DRM
- Player
- Analytics
- Media
- Cloud
---
