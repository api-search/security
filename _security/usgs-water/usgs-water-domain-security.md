---
api_specs:
- filename: openapi
  format: yaml
  label: USGS OGC Continuous Values API
  slug: ogc-continuous-values
  spec_type: OpenAPI
  url: https://api.waterdata.usgs.gov/ogcapi/v0/openapi?f=json
- filename: openapi
  format: yaml
  label: USGS OGC Daily Values API
  slug: ogc-daily-values
  spec_type: OpenAPI
  url: https://api.waterdata.usgs.gov/ogcapi/v0/openapi?f=json
- filename: openapi
  format: yaml
  label: USGS OGC Monitoring Locations API
  slug: ogc-monitoring-locations
  spec_type: OpenAPI
  url: https://api.waterdata.usgs.gov/ogcapi/v0/openapi?f=json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usgs.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: waterqualitydata.us
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: waterservices.usgs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 15 21:20:52 2026 GMT
  host: api.waterdata.usgs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.waterqualitydata.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usgs Water Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USGS Water Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USGS Water Services
provider_slug: usgs-water
slug: usgs-water-domain-security
source_filename: usgs-water-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waterservices.usgs.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.waterdata.usgs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:20:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.waterqualitydata.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usgs.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: waterqualitydata.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usgs-water/refs/heads/main/security/usgs-water-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Water
- Streamflow
- Groundwater
- Water Quality
- Hydrology
- Environmental
- USGS
- NWIS
- Government
- Open Data
- OGC
---
