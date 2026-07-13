---
api_specs:
- filename: openapi.json
  format: json
  label: National Weather Service API (api.weather.gov)
  slug: weather-gov-api
  spec_type: OpenAPI
  url: https://api.weather.gov/openapi.json
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: noaa.gov
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.noaa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 13:06:37 2026 GMT
  host: data.noaa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 15:38:49 2026 GMT
  host: www.nesdis.noaa.gov
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noaa Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NOAA — National Oceanic and Atmospheric Administration, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NOAA — National Oceanic and Atmospheric Administration
provider_slug: noaa-gov
slug: noaa-gov-domain-security
source_filename: noaa-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noaa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: data.noaa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:06:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.nesdis.noaa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:38:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: noaa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/security/noaa-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Weather
- Climate
- Ocean
- Space Weather
- Government
- Open Data
- Forecast
- Marine
- Atmospheric
- Hydrology
- Satellite
- Fisheries
- Aviation
- Emergency Management
---
