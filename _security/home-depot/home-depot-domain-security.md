---
api_specs:
- filename: home-depot-home-depot-api-openapi.yml
  format: yaml
  label: Home Depot API
  slug: home-depot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/home-depot/refs/heads/main/openapi/home-depot-home-depot-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: homedepot.com
  spf: true
hosts:
- host: developer.homedepot.com
  https: false
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.homedepot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Home Depot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for home-depot, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: home-depot
provider_slug: home-depot
slug: home-depot-domain-security
source_filename: home-depot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.homedepot.com\n  https: false\n- host: api.homedepot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: homedepot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/home-depot/refs/heads/main/security/home-depot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 100
---
