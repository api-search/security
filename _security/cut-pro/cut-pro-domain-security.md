---
api_specs:
- filename: cut-pro-openapi-generated.yml
  format: yaml
  label: Cut.Pro API
  slug: cut-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cut-pro/openapi/_ae-authored/cut-pro-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cut.pro
  spf: true
hosts:
- cert_expires: Jan 16 17:42:20 2027 GMT
  host: cut.pro
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cut Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cut.Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cut.Pro
provider_slug: cut-pro
slug: cut-pro-domain-security
source_filename: cut-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cut.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 17:42:20 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cut.pro\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cut-pro/security/cut-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Video
- Clipping
- Social Media
- Brazil
---
