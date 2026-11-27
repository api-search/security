---
api_specs:
- filename: genko-me-contents-api-openapi.yml
  format: yaml
  label: genko.me Contents API
  slug: genko-me-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genko-me/openapi/genko-me-contents-api-openapi.yml
- filename: genko-me-schema-api-openapi.yml
  format: yaml
  label: genko.me Schema API
  slug: genko-me-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genko-me/openapi/genko-me-schema-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: genko.me
  spf: true
hosts:
- cert_expires: Jan 24 01:15:07 2027 GMT
  host: genko.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: genko.me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for genko.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: genko.me
provider_slug: genko-me
slug: genko-me-domain-security
source_filename: genko-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genko.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 01:15:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genko.me\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/genko-me/security/genko-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Headless CMS
- Content Management
- Japanese
- Software-as-a-Service
---
