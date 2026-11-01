---
api_specs:
- filename: hardcover-openapi-generated.yml
  format: yaml
  label: Hardcover API
  slug: hardcover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hardcover/openapi/_ae-authored/hardcover-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:jules@hardcover.app"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hardcover.app
  spf: true
hosts:
- cert_expires: Dec 21 09:56:08 2026 GMT
  host: hardcover.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hardcover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hardcover, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hardcover
provider_slug: hardcover
slug: hardcover-domain-security
source_filename: hardcover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hardcover.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:56:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hardcover.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:jules@hardcover.app\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hardcover/security/hardcover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social
- Book
- Reading
- Community
- API
---
