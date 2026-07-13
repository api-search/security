---
api_specs:
- filename: authentication-openapi.yml
  format: yaml
  label: Vantor Hub Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/authentication-openapi.yml
- filename: discovery-openapi.yml
  format: yaml
  label: Vantor Hub Discovery API
  slug: discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/discovery-openapi.yml
- filename: admin-openapi.yml
  format: yaml
  label: Vantor Hub Account Services API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/admin-openapi.yml
- filename: streaming-openapi.yml
  format: yaml
  label: Maxar Geospatial Platform Streaming API
  slug: streaming
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/streaming-openapi.yml
- filename: ordering-openapi.yml
  format: yaml
  label: Maxar Geospatial Platform Ordering API
  slug: ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/ordering-openapi.yml
- filename: tasking-openapi.yml
  format: yaml
  label: Maxar Geospatial Platform Tasking API
  slug: tasking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/tasking-openapi.yml
- filename: monitoring-openapi.yml
  format: yaml
  label: Maxar Geospatial Platform Monitoring API
  slug: monitoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/monitoring-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vantor.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maxar.com
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: vantor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: hub.vantor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.maxar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maxar Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maxar Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Maxar Technologies
provider_slug: maxar-technologies
slug: maxar-technologies-domain-security
source_filename: maxar-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vantor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hub.vantor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.maxar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vantor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: maxar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/security/maxar-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Satellite Imagery
- Earth Observation
- Geospatial
- Remote Sensing
- Spatial Intelligence
- Defense
- Intelligence
- WorldView
- STAC
- OGC
- WMS
- WMTS
- WFS
- Tasking
- Basemaps
- Vantor
- Lanteris
- Advent International
- Private Equity
---
