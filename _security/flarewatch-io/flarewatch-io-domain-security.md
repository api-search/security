---
api_specs:
- filename: flarewatch-io-openapi-generated.yml
  format: yaml
  label: FlareWatch API
  slug: flarewatch-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flarewatch-io/openapi/_ae-authored/flarewatch-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: true
  domain: flarewatch.io
  spf: true
hosts:
- cert_expires: Jan 31 02:30:20 2027 GMT
  host: flarewatch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlareWatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlareWatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: FlareWatch
provider_slug: flarewatch-io
slug: flarewatch-io-domain-security
source_filename: flarewatch-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flarewatch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 02:30:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flarewatch.io\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flarewatch-io/security/flarewatch-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Staking
- Dashboards
- Validator
- Tax
- DeFi
---
