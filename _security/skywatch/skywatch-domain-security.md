---
api_specs:
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Archive Search API
  slug: skywatch-archive-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Pipelines API
  slug: skywatch-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Interval Results & Delivery API
  slug: skywatch-interval-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Cost Estimation API
  slug: skywatch-cost-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Outputs & Bands API
  slug: skywatch-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Locations API
  slug: skywatch-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Subscriptions & Callbacks API
  slug: skywatch-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: skywatch.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: earthcache.com
  spf: false
hosts:
- cert_expires: Nov 24 18:24:53 2026 GMT
  host: skywatch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api-docs.earthcache.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: api.skywatch.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skywatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SkyWatch, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SkyWatch
provider_slug: skywatch
slug: skywatch-domain-security
source_filename: skywatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skywatch.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 18:24:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.earthcache.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n- host: api.skywatch.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: skywatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: earthcache.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/security/skywatch-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Satellite Imagery
- Earth Observation
- Geospatial
- Remote Sensing
- EarthCache
- Imagery
---
