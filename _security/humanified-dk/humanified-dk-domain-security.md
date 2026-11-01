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
  domain: humanified.dk
  spf: true
hosts:
- cert_expires: Dec  5 17:20:28 2026 GMT
  host: humanified.dk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Humanified Dk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for humanified-dk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: humanified-dk
provider_slug: humanified-dk
slug: humanified-dk-domain-security
source_filename: humanified-dk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanified.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 17:20:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: humanified.dk\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/humanified-dk/security/humanified-dk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trust
- Energy
- Cooperation
- Decision-Making
- Analytics
---
