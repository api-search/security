---
api_specs:
- filename: usda-snap-openapi.yml
  format: yaml
  label: SNAP Retailer Location Data API
  slug: usda-snap-retailer-location-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usda-snap/refs/heads/main/openapi/usda-snap-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:vkeymaster@esri.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.fna.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: services1.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usda Snap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USDA SNAP Retailer Locator, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USDA SNAP Retailer Locator
provider_slug: usda-snap
slug: usda-snap-domain-security
source_filename: usda-snap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fna.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services1.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:vkeymaster@esri.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usda-snap/refs/heads/main/security/usda-snap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SNAP
- USDA
- Food and Nutrition Administration
- FNA
- FNS
- Retailer Locator
- Open Data
- ArcGIS
- GIS
- Government Data
- Food Assistance
---
