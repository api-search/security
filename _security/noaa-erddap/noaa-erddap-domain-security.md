---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: NOAA ERDDAP REST API
  slug: noaa-erddap-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-erddap/refs/heads/main/openapi/openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "entrust.net"
  - 0 issue "godaddy.com"
  - 0 issue "sectigo.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: noaa.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ioos.us
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: coastwatch.pfeg.noaa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 17:40:29 2026 GMT
  host: erddap.ioos.us
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Noaa Erddap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NOAA ERDDAP, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NOAA ERDDAP
provider_slug: noaa-erddap
slug: noaa-erddap-domain-security
source_filename: noaa-erddap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coastwatch.pfeg.noaa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: erddap.ioos.us\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 17:40:29 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: noaa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ioos.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noaa-erddap/refs/heads/main/security/noaa-erddap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- oceanography
- meteorology
- climate
- environmental data
- gridded data
- tabular data
- scientific data
- government
- NOAA
- open data
---
