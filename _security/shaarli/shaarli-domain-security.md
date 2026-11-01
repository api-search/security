---
api_specs:
- filename: shaarli-shaarli-api-openapi.yml
  format: yaml
  label: Shaarli API
  slug: shaarli-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shaarli/openapi/shaarli-shaarli-api-openapi.yml
- filename: shaarli-openapi-generated.yml
  format: yaml
  label: Shaarli API
  slug: shaarli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shaarli/openapi/_ae-authored/shaarli-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shaarli.org
  spf: false
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Jan  6 14:06:19 2027 GMT
  host: demo.shaarli.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 14:03:01 2026 GMT
  host: shaarli.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Shaarli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shaarli, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Shaarli
provider_slug: shaarli
slug: shaarli-domain-security
source_filename: shaarli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: demo.shaarli.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 14:06:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shaarli.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 14:03:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shaarli.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/shaarli/security/shaarli-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Bookmarking
- Self-hosted
- Open-source
- PHP
- Minimalist
---
