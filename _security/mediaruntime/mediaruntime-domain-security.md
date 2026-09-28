---
api_specs:
- filename: mediaruntime-discovery-api-openapi.yml
  format: yaml
  label: MediaRuntime Discovery API
  slug: mediaruntime-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-discovery-api-openapi.yml
- filename: mediaruntime-job-results-api-openapi.yml
  format: yaml
  label: MediaRuntime Job Results API
  slug: mediaruntime-job-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-job-results-api-openapi.yml
- filename: mediaruntime-jobs-api-openapi.yml
  format: yaml
  label: MediaRuntime Jobs API
  slug: mediaruntime-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-jobs-api-openapi.yml
- filename: mediaruntime-media-analysis-api-openapi.yml
  format: yaml
  label: MediaRuntime Media Analysis API
  slug: mediaruntime-media-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-media-analysis-api-openapi.yml
- filename: mediaruntime-mediaruntime-api-api-openapi.yml
  format: yaml
  label: MediaRuntime API
  slug: mediaruntime-mediaruntime-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-mediaruntime-api-api-openapi.yml
- filename: mediaruntime-moderation-api-openapi.yml
  format: yaml
  label: MediaRuntime Moderation API
  slug: mediaruntime-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-moderation-api-openapi.yml
- filename: mediaruntime-recipes-api-openapi.yml
  format: yaml
  label: MediaRuntime Recipes API
  slug: mediaruntime-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-recipes-api-openapi.yml
- filename: mediaruntime-sandbox-api-openapi.yml
  format: yaml
  label: MediaRuntime Sandbox API
  slug: mediaruntime-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sandbox-api-openapi.yml
- filename: mediaruntime-uploads-api-openapi.yml
  format: yaml
  label: MediaRuntime Uploads API
  slug: mediaruntime-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-uploads-api-openapi.yml
- filename: mediaruntime-watermarks-api-openapi.yml
  format: yaml
  label: MediaRuntime Watermarks API
  slug: mediaruntime-watermarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-watermarks-api-openapi.yml
- filename: mediaruntime-webhooks-api-openapi.yml
  format: yaml
  label: MediaRuntime Webhooks API
  slug: mediaruntime-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-webhooks-api-openapi.yml
- filename: mediaruntime-marketplace-api-openapi.yml
  format: yaml
  label: MediaRuntime Marketplace API
  slug: mediaruntime-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-marketplace-api-openapi.yml
- filename: mediaruntime-sticker-collections-api-openapi.yml
  format: yaml
  label: MediaRuntime Sticker Collections API
  slug: mediaruntime-sticker-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sticker-collections-api-openapi.yml
- filename: mediaruntime-sticker-runtime-api-openapi.yml
  format: yaml
  label: MediaRuntime Sticker Runtime API
  slug: mediaruntime-sticker-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sticker-runtime-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mediaruntime.com
  spf: true
hosts:
- cert_expires: Nov 25 10:20:12 2026 GMT
  host: mediaruntime.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mediaruntime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediaRuntime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MediaRuntime
provider_slug: mediaruntime
slug: mediaruntime-domain-security
source_filename: mediaruntime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mediaruntime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 10:20:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: mediaruntime.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/security/mediaruntime-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Media Processing
- Video
- Audio
- Runtime
- Video Encoding
- Audio Processing
- Image Processing
- Content Moderation
- Media API
- Asynchronous Processing
---
