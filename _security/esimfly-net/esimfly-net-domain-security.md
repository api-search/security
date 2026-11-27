---
api_specs:
- filename: esimfly-net-openapi-generated.yml
  format: yaml
  label: eSIMfly API
  slug: esimfly-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimfly-net/openapi/_ae-authored/esimfly-net-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: esimfly.net
  spf: true
hosts:
- cert_expires: Dec 28 16:42:42 2026 GMT
  host: esimfly.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eSIMfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eSIMfly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: eSIMfly
provider_slug: esimfly-net
slug: esimfly-net-domain-security
source_filename: esimfly-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esimfly.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 16:42:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: esimfly.net\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/esimfly-net/security/esimfly-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- eSIM
- Travel
- Connectivity
- Telecommunications
---
