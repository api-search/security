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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: videoamp.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: videoamp.dev
  spf: false
hosts:
- cert_expires: Sep 28 17:58:04 2026 GMT
  host: videoamp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: docs.videoamp.dev
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: api.videoamp.dev
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Videoamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VideoAmp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VideoAmp
provider_slug: videoamp
slug: videoamp-domain-security
source_filename: videoamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: videoamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:58:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.videoamp.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\n- host: api.videoamp.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: videoamp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: videoamp.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/security/videoamp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
---
