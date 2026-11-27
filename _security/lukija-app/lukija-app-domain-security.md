---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lukija.app
  spf: false
hosts:
- cert_expires: Feb  6 08:03:26 2027 GMT
  host: lukija.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lukija Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lukija, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Lukija
provider_slug: lukija-app
slug: lukija-app-domain-security
source_filename: lukija-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lukija.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 08:03:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lukija.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lukija-app/security/lukija-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Language Learning
- Education
- Finnish
- Software-as-a-Service
- Reading
---
