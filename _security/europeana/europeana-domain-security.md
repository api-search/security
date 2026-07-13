---
api_specs:
- filename: europeana-openapi.yml
  format: yaml
  label: Europeana Search and Record API
  slug: europeana-search-and-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/europeana/refs/heads/main/openapi/europeana-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: europeana.eu
  spf: true
hosts:
- cert_expires: Aug 20 00:16:31 2026 GMT
  host: pro.europeana.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 00:16:31 2026 GMT
  host: api.europeana.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Europeana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Europeana, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Europeana
provider_slug: europeana
slug: europeana-domain-security
source_filename: europeana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pro.europeana.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:16:31 2026 GMT\n  hsts: null\n- host: api.europeana.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:16:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: europeana.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/europeana/refs/heads/main/security/europeana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Archives
- Cultural Heritage
- Europe
- Libraries
- Museums
- Search
---
