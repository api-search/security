---
api_specs:
- filename: gnews-openapi.yml
  format: yaml
  label: GNews
  slug: gnews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnews/refs/heads/main/openapi/gnews-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gnews.io
  spf: true
hosts:
- cert_expires: Sep 14 14:40:56 2026 GMT
  host: gnews.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gnews Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GNews, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GNews
provider_slug: gnews
slug: gnews-domain-security
source_filename: gnews-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gnews.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:40:56 2026 GMT\n  hsts: false\ndomains:\n- domain: gnews.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gnews/refs/heads/main/security/gnews-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Articles
- Headlines
- News
- Search
---
