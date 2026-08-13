---
api_specs:
- filename: freewheel-media-advertiser-buzz-openapi-original.json
  format: json
  label: FreeWheel Advertiser (Buzz) API
  slug: freewheel-media-advertiser-buzz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/openapi/freewheel-media-advertiser-buzz-openapi-original.json
- filename: freewheel-media-demand-audience-management-openapi-original.json
  format: json
  label: FreeWheel Demand Audience Management API
  slug: freewheel-media-demand-audience-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/openapi/freewheel-media-demand-audience-management-openapi-original.json
- filename: freewheel-media-demand-deal-sync-openapi-original.json
  format: json
  label: FreeWheel Demand Deal Sync API
  slug: freewheel-media-demand-deal-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/openapi/freewheel-media-demand-deal-sync-openapi-original.json
- filename: freewheel-media-demand-creative-management-openapi-original.json
  format: json
  label: FreeWheel Demand Creative Management API
  slug: freewheel-media-demand-creative-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/openapi/freewheel-media-demand-creative-management-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freewheel.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freewheel.tv
  spf: true
hosts:
- cert_expires: Oct  3 20:16:05 2026 GMT
  host: www.freewheel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 02:16:46 2026 GMT
  host: partners.freewheel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 06:58:51 2026 GMT
  host: api-docs.freewheel.tv
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freewheel Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeWheel Media, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FreeWheel Media
provider_slug: freewheel-media
slug: freewheel-media-domain-security
source_filename: freewheel-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freewheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:16:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: partners.freewheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:16:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.freewheel.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:58:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freewheel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: freewheel.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/security/freewheel-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Streaming TV
- Video Advertising
- Programmatic
- Media
- Publisher Monetization
- Comcast
---
