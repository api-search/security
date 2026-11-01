---
api_specs:
- filename: sealgate-jp-openapi-generated.yml
  format: yaml
  label: sealgate-jp API
  slug: sealgate-jp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sealgate-jp/openapi/_ae-authored/sealgate-jp-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sealgate.jp
  spf: false
hosts:
- cert_expires: Jan 16 13:12:06 2027 GMT
  host: sealgate.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sealgate Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sealgate-jp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: sealgate-jp
provider_slug: sealgate-jp
slug: sealgate-jp-domain-security
source_filename: sealgate-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sealgate.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 13:12:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sealgate.jp\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sealgate-jp/security/sealgate-jp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- WebAuthn
- FIDO2
- Security
- Japan
---
