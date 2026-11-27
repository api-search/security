---
api_specs:
- filename: applivery-com-openapi-generated.yml
  format: yaml
  label: Applivery API
  slug: applivery-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applivery-com/openapi/_ae-authored/applivery-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "security@applivery.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: applivery.com
  spf: true
hosts:
- cert_expires: Jan 23 23:04:59 2027 GMT
  host: applivery.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Applivery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Applivery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Applivery
provider_slug: applivery-com
slug: applivery-com-domain-security
source_filename: applivery-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: applivery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:04:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: applivery.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"security@applivery.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/applivery-com/security/applivery-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Unified Endpoint Management
- Mobile Device Management
- App Distribution
- Patch Management
- Remote Support
---
