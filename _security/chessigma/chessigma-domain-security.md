---
api_specs:
- filename: chessigma-daily-puzzle-api-openapi.yml
  format: yaml
  label: Chessigma Daily Puzzle API
  slug: chessigma-daily-puzzle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chessigma/refs/heads/main/openapi/chessigma-daily-puzzle-api-openapi.yml
- filename: chessigma-elo-calculator-api-openapi.yml
  format: yaml
  label: Chessigma Elo Calculator API
  slug: chessigma-elo-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chessigma/refs/heads/main/openapi/chessigma-elo-calculator-api-openapi.yml
- filename: chessigma-game-api-openapi.yml
  format: yaml
  label: Chessigma Game API
  slug: chessigma-game-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chessigma/refs/heads/main/openapi/chessigma-game-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chessigma.com
  spf: true
hosts:
- cert_expires: Jan  1 10:42:18 2027 GMT
  host: www.chessigma.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chessigma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chessigma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chessigma
provider_slug: chessigma
slug: chessigma-domain-security
source_filename: chessigma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chessigma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 10:42:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chessigma.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chessigma/refs/heads/main/security/chessigma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Chess
- API
- Free
- NoAuth
---
