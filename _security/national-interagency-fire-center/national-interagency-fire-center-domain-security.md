---
api_specs:
- filename: national-interagency-fire-center-openapi.yml
  format: yaml
  label: NIFC ArcGIS REST Services API
  slug: nifc-arcgis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-interagency-fire-center/main/openapi/national-interagency-fire-center-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nifc.gov
  spf: true
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:vkeymaster@esri.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  spf: true
hosts:
- cert_expires: Oct  1 13:44:16 2026 GMT
  host: www.nifc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: data-nifc.opendata.arcgis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: services3.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Interagency Fire Center Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Interagency Fire Center, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Interagency Fire Center
provider_slug: national-interagency-fire-center
slug: national-interagency-fire-center-domain-security
source_filename: national-interagency-fire-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nifc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 13:44:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data-nifc.opendata.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services3.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nifc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:vkeymaster@esri.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-interagency-fire-center/refs/heads/main/security/national-interagency-fire-center-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Emergency Management
- Federal Government
- Geospatial
- Wildfire
---
