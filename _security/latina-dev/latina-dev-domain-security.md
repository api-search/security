---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: latina.dev
  spf: true
hosts:
- cert_expires: Jan 21 07:51:59 2027 GMT
  host: latina.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Latina Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latina Dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Latina Dev
provider_slug: latina-dev
slug: latina-dev-domain-security
source_filename: latina-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latina.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 07:51:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: latina.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/latina-dev/security/latina-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Directory
- Community
- Open Source
- Diversity
- Engineering
---
