---
api_specs:
- filename: flying-sphinx-openapi-generated.yml
  format: yaml
  label: Flying Sphinx API
  slug: flying-sphinx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flying-sphinx/openapi/_ae-authored/flying-sphinx-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flying-sphinx.com
  spf: true
hosts:
- cert_expires: Jan 24 01:10:07 2027 GMT
  host: flying-sphinx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flying Sphinx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flying Sphinx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flying Sphinx
provider_slug: flying-sphinx
slug: flying-sphinx-domain-security
source_filename: flying-sphinx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flying-sphinx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 01:10:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flying-sphinx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flying-sphinx/security/flying-sphinx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Heroku
- Addon
- Sphinx
- Ruby
---
