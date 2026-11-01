---
api_specs:
- filename: datasette-openapi-generated.yml
  format: yaml
  label: Datasette API
  slug: datasette-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasette/openapi/_ae-authored/datasette-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: datasette.io
  spf: false
hosts:
- cert_expires: Dec  5 23:50:25 2026 GMT
  host: datasette.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datasette Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datasette, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Datasette
provider_slug: datasette
slug: datasette-domain-security
source_filename: datasette-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datasette.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:50:25 2026 GMT\n  hsts: false\ndomains:\n- domain: datasette.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/datasette/security/datasette-domain-security.yml
summary_line: TLSv1.3
tags:
- OpenSource
- DataTools
- Publishing
- Visualization
- Community
---
