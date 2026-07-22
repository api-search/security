---
api_specs:
- filename: perchwell-json-api-openapi.yml
  format: yaml
  label: Perchwell JSON API
  slug: perchwell-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-json-api-openapi.yml
- filename: perchwell-reso-web-api-openapi.yml
  format: yaml
  label: Perchwell RESO Web API
  slug: perchwell-reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-reso-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: perchwell.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: perchwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: docs.perchwell.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.perchwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Perchwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perchwell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Perchwell
provider_slug: perchwell
slug: perchwell-domain-security
source_filename: perchwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perchwell.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.perchwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\n- host: www.perchwell.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: perchwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/security/perchwell-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Real Estate
- MLS
- Listings
- Property Data
- RESO
- RETS
- OData
- Real Estate Data
---
