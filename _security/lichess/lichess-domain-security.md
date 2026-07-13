---
api_specs:
- filename: lichess-openapi.yml
  format: yaml
  label: Lichess API
  slug: lichess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lichess/refs/heads/main/openapi/lichess-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lichess.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lichess.dev
  spf: false
hosts:
- cert_expires: Sep  1 21:48:06 2026 GMT
  host: lichess.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 18:43:58 2026 GMT
  host: lichess.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: l.org
  https: false
kind: domain-security
layout: security
method: probed
name: Lichess Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lichess, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lichess
provider_slug: lichess
slug: lichess-domain-security
source_filename: lichess-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lichess.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:48:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: lichess.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 18:43:58 2026 GMT\n  hsts: false\n- host: l.org\n  https: false\ndomains:\n- domain: lichess.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lichess.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lichess/refs/heads/main/security/lichess-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Chess
- Games
- Open Source
- Nonprofit
- Tournaments
- Puzzles
- Bots
- Streaming
- ND-JSON
- OAuth
---
