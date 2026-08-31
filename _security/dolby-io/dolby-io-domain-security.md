---
api_specs:
- filename: dolby-io-abr-ladders-api-openapi.yml
  format: yaml
  label: Dolby.io ABR Ladders API
  slug: dolby-io-abr-ladders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-abr-ladders-api-openapi.yml
- filename: dolby-io-analytics-api-openapi.yml
  format: yaml
  label: Dolby.io Analytics API
  slug: dolby-io-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-analytics-api-openapi.yml
- filename: dolby-io-channels-api-openapi.yml
  format: yaml
  label: Dolby.io Channels API
  slug: dolby-io-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-channels-api-openapi.yml
- filename: dolby-io-cluster-api-openapi.yml
  format: yaml
  label: Dolby.io Cluster API
  slug: dolby-io-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-cluster-api-openapi.yml
- filename: dolby-io-custom-endpoint-providers-api-openapi.yml
  format: yaml
  label: Dolby.io Custom Endpoint Providers API
  slug: dolby-io-custom-endpoint-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-custom-endpoint-providers-api-openapi.yml
- filename: dolby-io-custom-endpoints-api-openapi.yml
  format: yaml
  label: Dolby.io Custom Endpoints API
  slug: dolby-io-custom-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-custom-endpoints-api-openapi.yml
- filename: dolby-io-distributions-api-openapi.yml
  format: yaml
  label: Dolby.io Distributions API
  slug: dolby-io-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-distributions-api-openapi.yml
- filename: dolby-io-engines-api-openapi.yml
  format: yaml
  label: Dolby.io Engines API
  slug: dolby-io-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-engines-api-openapi.yml
- filename: dolby-io-ingests-api-openapi.yml
  format: yaml
  label: Dolby.io Ingests API
  slug: dolby-io-ingests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-ingests-api-openapi.yml
- filename: dolby-io-publishtoken-api-openapi.yml
  format: yaml
  label: Dolby.io PublishToken API
  slug: dolby-io-publishtoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-publishtoken-api-openapi.yml
- filename: dolby-io-regions-api-openapi.yml
  format: yaml
  label: Dolby.io Regions API
  slug: dolby-io-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-regions-api-openapi.yml
- filename: dolby-io-subscribetoken-api-openapi.yml
  format: yaml
  label: Dolby.io SubscribeToken API
  slug: dolby-io-subscribetoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-subscribetoken-api-openapi.yml
- filename: dolby-io-webhook-api-openapi.yml
  format: yaml
  label: Dolby.io Webhook API
  slug: dolby-io-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-webhook-api-openapi.yml
- filename: dolby-io-webhooks-api-openapi.yml
  format: yaml
  label: Dolby.io Webhooks API
  slug: dolby-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/openapi/dolby-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dolby.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dolby.io
  spf: true
hosts:
- cert_expires: Sep  2 21:41:38 2026 GMT
  host: optiview.dolby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 10:57:17 2026 GMT
  host: dolby.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: docs.dolby.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dolby Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dolby.io, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dolby.io
provider_slug: dolby-io
slug: dolby-io-domain-security
source_filename: dolby-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optiview.dolby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:41:38 2026 GMT\n  hsts: false\n- host: dolby.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:57:17 2026 GMT\n  hsts: false\n- host: docs.dolby.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dolby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dolby.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolby-io/refs/heads/main/security/dolby-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Media
- Streaming
- Real-time Streaming
- WebRTC
- Live Streaming
- Low Latency
- Video
- Audio
- Broadcast
- Player
- Advertising
- Dolby OptiView
- Millicast
- THEOlive
- THEOplayer
---
