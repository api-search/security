---
api_specs:
- filename: process
  format: yaml
  label: Sentinel Hub Process API
  slug: process
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/process
- filename: catalog
  format: yaml
  label: Sentinel Hub Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/catalog
- filename: statistical
  format: yaml
  label: Sentinel Hub Statistical API
  slug: statistical
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/statistical
- filename: batch_process
  format: yaml
  label: Sentinel Hub Batch Processing API
  slug: batch
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/batch_process
- filename: byoc
  format: yaml
  label: Sentinel Hub BYOC API
  slug: byoc
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/byoc
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sentinel-hub.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.sentinel-hub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: docs.sentinel-hub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: services.sentinel-hub.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sentinel Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentinel Hub, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sentinel Hub
provider_slug: sentinel-hub
slug: sentinel-hub-domain-security
source_filename: sentinel-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sentinel-hub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: docs.sentinel-hub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: services.sentinel-hub.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sentinel-hub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentinel-hub/refs/heads/main/security/sentinel-hub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Satellite Imagery
- Geospatial
- Remote Sensing
- Earth Observation
- NDVI
- Sentinel
- Landsat
- MODIS
- OGC
- STAC
---
