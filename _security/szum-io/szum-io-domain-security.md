---
api_specs:
- filename: szum-io-openapi-generated.yml
  format: yaml
  label: Szum API
  slug: szum-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/szum-io/openapi/_ae-authored/szum-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: szum.io
  spf: false
hosts:
- cert_expires: Feb 23 00:12:55 2027 GMT
  host: szum.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Szum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Szum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Szum
provider_slug: szum-io
slug: szum-io-domain-security
source_filename: szum-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: szum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 00:12:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: szum.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/szum-io/security/szum-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Visualization
- API
- Charting
- AI Integration
---
