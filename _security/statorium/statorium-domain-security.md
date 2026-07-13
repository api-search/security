---
api_specs:
- filename: statorium-football-api-openapi.yml
  format: yaml
  label: Statorium Football API
  slug: football-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-football-api-openapi.yml
- filename: statorium-basketball-api-openapi.yml
  format: yaml
  label: Statorium Basketball API
  slug: basketball-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-basketball-api-openapi.yml
- filename: statorium-american-football-api-openapi.yml
  format: yaml
  label: Statorium American Football API
  slug: american-football-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/openapi/statorium-american-football-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: statorium.com
  spf: false
hosts:
- cert_expires: Oct  1 05:29:32 2026 GMT
  host: statorium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 11:48:40 2026 GMT
  host: api.statorium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Statorium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Statorium, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Statorium
provider_slug: statorium
slug: statorium-domain-security
source_filename: statorium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: statorium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:29:32 2026 GMT\n  hsts: false\n- host: api.statorium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:48:40 2026 GMT\n  hsts: false\ndomains:\n- domain: statorium.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statorium/refs/heads/main/security/statorium-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports
- Sports Data
- Football
- Soccer
- Basketball
- American Football
- Live Scores
- Statistics
---
