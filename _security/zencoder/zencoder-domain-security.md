---
api_specs:
- filename: zencoder-accounts-api-openapi.yml
  format: yaml
  label: Zencoder Accounts API
  slug: zencoder-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zencoder/refs/heads/main/openapi/zencoder-accounts-api-openapi.yml
- filename: zencoder-inputs-api-openapi.yml
  format: yaml
  label: Zencoder Inputs API
  slug: zencoder-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zencoder/refs/heads/main/openapi/zencoder-inputs-api-openapi.yml
- filename: zencoder-jobs-api-openapi.yml
  format: yaml
  label: Zencoder Jobs API
  slug: zencoder-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zencoder/refs/heads/main/openapi/zencoder-jobs-api-openapi.yml
- filename: zencoder-outputs-api-openapi.yml
  format: yaml
  label: Zencoder Outputs API
  slug: zencoder-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zencoder/refs/heads/main/openapi/zencoder-outputs-api-openapi.yml
- filename: zencoder-reports-api-openapi.yml
  format: yaml
  label: Zencoder Reports API
  slug: zencoder-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zencoder/refs/heads/main/openapi/zencoder-reports-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zencoder.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightcove.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: zencoder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: zencoder.support.brightcove.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: app.zencoder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zencoder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zencoder, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zencoder
provider_slug: zencoder
slug: zencoder-domain-security
source_filename: zencoder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zencoder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n- host: zencoder.support.brightcove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\n- host: app.zencoder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zencoder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: brightcove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zencoder/refs/heads/main/security/zencoder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Video Encoding
- Transcoding
- Media
- Streaming
- Video Processing
- Cloud
- Brightcove
- Captions
- DRM
- HLS
---
