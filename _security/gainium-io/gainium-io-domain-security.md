---
api_specs:
- filename: gainium-io-openapi-generated.yml
  format: yaml
  label: Gainium API
  slug: gainium-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gainium-io/openapi/_ae-authored/gainium-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "0 issue \"letsencrypt.org\""
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gainium.io
  spf: true
hosts:
- cert_expires: Jan 13 20:27:38 2027 GMT
  host: gainium.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gainium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gainium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gainium
provider_slug: gainium-io
slug: gainium-io-domain-security
source_filename: gainium-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gainium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 20:27:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gainium.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"0 issue \\\"letsencrypt.org\\\"\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gainium-io/security/gainium-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Trading
- Bots
- Open Source
- Artificial Intelligence
---
