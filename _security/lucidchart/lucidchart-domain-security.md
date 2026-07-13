---
api_specs:
- filename: lucidchart-openapi.yml
  format: yaml
  label: Lucid REST API
  slug: lucid-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidchart/refs/heads/main/openapi/lucidchart-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucidchart.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucid.co
  spf: true
hosts:
- cert_expires: Aug 25 07:09:13 2026 GMT
  host: www.lucidchart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 03:57:52 2026 GMT
  host: developer.lucid.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  5 19:02:32 2026 GMT
  host: api.lucid.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lucidchart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucidchart, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lucidchart
provider_slug: lucidchart
slug: lucidchart-domain-security
source_filename: lucidchart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lucidchart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 07:09:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lucid.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:57:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lucid.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 19:02:32 2026 GMT\n  hsts: null\ndomains:\n- domain: lucidchart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lucid.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidchart/refs/heads/main/security/lucidchart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Diagramming
- Visualization
- Visual Workspace
- SaaS
---
