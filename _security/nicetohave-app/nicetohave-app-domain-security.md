---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: nicetohave.app
  spf: false
hosts:
- cert_expires: Feb 12 21:44:21 2027 GMT
  host: nicetohave.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: nice to have Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nice to have, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: nice to have
provider_slug: nicetohave-app
slug: nicetohave-app-domain-security
source_filename: nicetohave-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nicetohave.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 21:44:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nicetohave.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nicetohave-app/security/nicetohave-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Marketplace
- Toolkit
- Japanese
---
