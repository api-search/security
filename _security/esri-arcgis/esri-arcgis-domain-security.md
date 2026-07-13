---
api_specs:
- filename: esri-arcgis-platform-openapi.yml
  format: yaml
  label: ESRI ArcGIS Platform API
  slug: esri-arcgis-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-platform-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:vkeymaster@esri.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: developers.arcgis.com
  hsts: true
  hsts_max_age: 6307200
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: js.arcgis.com
  hsts: true
  hsts_max_age: 6307200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Esri Arcgis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ESRI ArcGIS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ESRI ArcGIS
provider_slug: esri-arcgis
slug: esri-arcgis-domain-security
source_filename: esri-arcgis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 6307200\n- host: www.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: js.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 6307200\ndomains:\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:vkeymaster@esri.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/security/esri-arcgis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GIS
- Geospatial
- Mapping
- Location
- Spatial Analysis
---
