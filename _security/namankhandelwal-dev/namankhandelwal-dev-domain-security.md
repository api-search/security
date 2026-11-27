---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: namankhandelwal.dev
  spf: false
hosts:
- cert_expires: Jan 21 20:29:46 2027 GMT
  host: namankhandelwal.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Naman Khandelwal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Naman Khandelwal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Naman Khandelwal
provider_slug: namankhandelwal-dev
slug: namankhandelwal-dev-domain-security
source_filename: namankhandelwal-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namankhandelwal.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:29:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: namankhandelwal.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/namankhandelwal-dev/security/namankhandelwal-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Developers
- Open Source
- Full-Stack
- Go
- React
---
