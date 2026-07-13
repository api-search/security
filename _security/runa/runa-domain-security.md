---
api_specs:
- filename: runa-payouts-api-openapi.yml
  format: yaml
  label: Runa Payouts API
  slug: runa-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runa/refs/heads/main/openapi/runa-payouts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:eng-team@runa.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: runa.io
  spf: true
hosts:
- cert_expires: Oct  2 18:56:54 2026 GMT
  host: developer.runa.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 10:12:33 2026 GMT
  host: api.runa.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 10:12:33 2026 GMT
  host: playground.runa.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Runa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Runa
provider_slug: runa
slug: runa-domain-security
source_filename: runa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.runa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:56:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.runa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:12:33 2026 GMT\n  hsts: null\n- host: playground.runa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:12:33 2026 GMT\n  hsts: null\ndomains:\n- domain: runa.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:eng-team@runa.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runa/refs/heads/main/security/runa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Gift Cards
- Rewards
- Payments
- Incentives
- Payouts
---
