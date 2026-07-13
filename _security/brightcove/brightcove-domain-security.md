---
api_specs:
- filename: cms-api-swagger.yaml
  format: yaml
  label: Brightcove CMS API
  slug: brightcove-cms-api
  spec_type: OpenAPI
  url: https://apis.support.brightcove.com/cms/references/cms-api-swagger.yaml
- filename: ssai-openapi.yaml
  format: yaml
  label: Brightcove SSAI API
  slug: brightcove-ssai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/ssai-openapi.yaml
- filename: delivery-rules-openapi.yaml
  format: yaml
  label: Brightcove Delivery Rules API
  slug: brightcove-delivery-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/delivery-rules-openapi.yaml
- filename: social-openapi.yaml
  format: yaml
  label: Brightcove Social API
  slug: brightcove-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/social-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightcove.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.brightcove.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: apis.support.brightcove.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: cms.api.brightcove.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Brightcove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brightcove, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brightcove
provider_slug: brightcove
slug: brightcove-domain-security
source_filename: brightcove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightcove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n- host: apis.support.brightcove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: false\n- host: cms.api.brightcove.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: brightcove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/security/brightcove-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- Media
- Streaming
- Live Streaming
- Analytics
- CDN
- OTT
- Player
- Ad Insertion
---
