---
api_specs:
- filename: gankdat-com-changes-api-openapi.yml
  format: yaml
  label: gankdat Changes API
  slug: gankdat-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gankdat-com/openapi/gankdat-com-changes-api-openapi.yml
- filename: gankdat-com-data-api-openapi.yml
  format: yaml
  label: gankdat Data API
  slug: gankdat-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gankdat-com/openapi/gankdat-com-data-api-openapi.yml
- filename: gankdat-com-platform-api-openapi.yml
  format: yaml
  label: gankdat Platform API
  slug: gankdat-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gankdat-com/openapi/gankdat-com-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gankdat.com
  spf: true
hosts:
- cert_expires: Feb  1 13:41:27 2027 GMT
  host: gankdat.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: gankdat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gankdat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: gankdat
provider_slug: gankdat-com
slug: gankdat-com-domain-security
source_filename: gankdat-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gankdat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 13:41:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gankdat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gankdat-com/security/gankdat-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Government
- United Kingdom
- EU
---
