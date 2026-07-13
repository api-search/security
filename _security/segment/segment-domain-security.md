---
api_specs:
- filename: segment-public-api-openapi.yml
  format: yaml
  label: Segment Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-public-api-openapi.yml
- filename: segment-http-tracking-api-openapi.yml
  format: yaml
  label: Segment HTTP Tracking API
  slug: http-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-http-tracking-api-openapi.yml
- filename: segment-profile-api-openapi.yml
  format: yaml
  label: Segment Profile API
  slug: profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-profile-api-openapi.yml
- filename: segment-config-api-openapi.yml
  format: yaml
  label: Segment Config API
  slug: config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-config-api-openapi.yml
- filename: segment-pixel-tracking-api-openapi.yml
  format: yaml
  label: Segment Pixel Tracking API
  slug: pixel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-pixel-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: segmentapis.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: twilio.com
  spf: true
hosts:
- cert_expires: Sep  7 12:19:25 2026 GMT
  host: docs.segmentapis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.segmentapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: www.twilio.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Segment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for segment, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: segment
provider_slug: segment
slug: segment-domain-security
source_filename: segment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.segmentapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:19:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.segmentapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\n- host: www.twilio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: segmentapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: twilio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/security/segment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
