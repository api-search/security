---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: useqr.co
  spf: false
hosts:
- cert_expires: Feb 19 11:07:13 2027 GMT
  host: useqr.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: useqr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for useqr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: useqr
provider_slug: useqr-co
slug: useqr-co-domain-security
source_filename: useqr-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useqr.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 11:07:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: useqr.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/useqr-co/security/useqr-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- QR
- Dynamic
- Packaging
- API
- SaaS
---
