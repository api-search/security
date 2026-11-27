---
api_specs:
- filename: iminify-com-openapi-generated.yml
  format: yaml
  label: Iminify API
  slug: iminify-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iminify-com/openapi/_ae-authored/iminify-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iminify.com
  spf: true
hosts:
- cert_expires: Jan  3 17:46:25 2027 GMT
  host: iminify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iminify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iminify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Iminify
provider_slug: iminify-com
slug: iminify-com-domain-security
source_filename: iminify-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iminify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 17:46:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iminify.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/iminify-com/security/iminify-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Image Compression
- Free
- Online Tool
- Formats
---
