---
api_specs:
- filename: halo-h5pc-api-openapi.yml
  format: yaml
  label: Halo H5pc API
  slug: halo-h5pc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/halo/openapi/halo-h5pc-api-openapi.yml
- filename: halo-h5-api-openapi.yml
  format: yaml
  label: Halo H5 API
  slug: halo-h5-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/halo/openapi/halo-h5-api-openapi.yml
- filename: halo-hw2-api-openapi.yml
  format: yaml
  label: Halo Hw2 API
  slug: halo-hw2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/halo/openapi/halo-hw2-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: haloapi.com
  spf: false
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Jan 21 20:00:42 2027 GMT
  host: developer.haloapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 09:10:12 2027 GMT
  host: s3publicapis.azure-api.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Halo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Halo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Halo
provider_slug: halo
slug: halo-domain-security
source_filename: halo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.haloapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:00:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: s3publicapis.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 09:10:12 2027 GMT\n  hsts: null\ndomains:\n- domain: haloapi.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/halo/security/halo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Game Data
- Gaming
- Halo
- Microsoft
- Player Statistics
- Public APIs
- Video Games
- Xbox
---
