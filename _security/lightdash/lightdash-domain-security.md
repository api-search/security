---
api_specs:
- filename: openapi.json
  format: json
  label: Lightdash REST API
  slug: lightdash-rest-api
  spec_type: OpenAPI
  url: https://docs.lightdash.com/api-reference/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightdash.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightdash.cloud
  spf: true
hosts:
- cert_expires: Sep 30 12:09:26 2026 GMT
  host: www.lightdash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 04:42:20 2026 GMT
  host: docs.lightdash.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 07:00:35 2026 GMT
  host: app.lightdash.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightdash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightdash, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lightdash
provider_slug: lightdash
slug: lightdash-domain-security
source_filename: lightdash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lightdash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:09:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lightdash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 04:42:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.lightdash.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 07:00:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightdash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lightdash.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightdash/refs/heads/main/security/lightdash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Intelligence
- Analytics
- dbt
- Semantic Layer
- Open Source
- Dashboards
- Data
---
