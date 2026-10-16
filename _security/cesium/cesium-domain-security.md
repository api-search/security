---
api_specs:
- filename: cesium-api-openapi.yml
  format: yaml
  label: Cesium ion Api API
  slug: cesium-ion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesium/refs/heads/main/openapi/_original/cesium-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cesium.com
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: cesium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cesium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cesium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cesium
provider_slug: cesium
slug: cesium-domain-security
source_filename: cesium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cesium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cesium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cesium/refs/heads/main/security/cesium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geospatial
- 3D
- Platform
- OpenSource
---
