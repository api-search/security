---
api_specs:
- filename: depthfeed-com-openapi-generated.yml
  format: yaml
  label: DepthFeed API
  slug: depthfeed-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depthfeed-com/openapi/_ae-authored/depthfeed-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: depthfeed.com
  spf: false
hosts:
- cert_expires: Jan 15 22:51:22 2027 GMT
  host: depthfeed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Depthfeed Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DepthFeed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DepthFeed
provider_slug: depthfeed-com
slug: depthfeed-com-domain-security
source_filename: depthfeed-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: depthfeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 22:51:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: depthfeed.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/depthfeed-com/security/depthfeed-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Data
- Market Data
- Prediction Markets
---
