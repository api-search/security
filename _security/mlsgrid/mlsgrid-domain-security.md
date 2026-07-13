---
api_specs:
- filename: mlsgrid-reso-web-api-openapi.yml
  format: yaml
  label: MLS Grid RESO Web API
  slug: mlsgrid-reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-reso-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mlsgrid.com
  spf: true
hosts:
- cert_expires: Sep 29 04:32:43 2026 GMT
  host: www.mlsgrid.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:03:47 2026 GMT
  host: docs.mlsgrid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.mlsgrid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mlsgrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mlsgrid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mlsgrid
provider_slug: mlsgrid
slug: mlsgrid-domain-security
source_filename: mlsgrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mlsgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:32:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.mlsgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mlsgrid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mlsgrid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/security/mlsgrid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
