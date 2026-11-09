---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brickandmortar.dev
  spf: true
hosts:
- cert_expires: Dec 11 11:00:42 2026 GMT
  host: brickandmortar.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brickandmortar Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brick & Mortar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brick & Mortar
provider_slug: brickandmortar-dev
slug: brickandmortar-dev-domain-security
source_filename: brickandmortar-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brickandmortar.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 11:00:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brickandmortar.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/brickandmortar-dev/security/brickandmortar-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Public Records
- Twin Cities
- Tools
- Open Data
- Minnesota
---
