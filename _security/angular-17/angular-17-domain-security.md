---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:angular-devinfra@google.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: angular.io
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: angular.dev
  spf: false
hosts:
- cert_expires: Sep 23 06:07:03 2026 GMT
  host: v17.angular.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 05:52:38 2026 GMT
  host: angular.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:18:58 2026 GMT
  host: v17.material.angular.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Angular 17 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angular 17, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Angular 17
provider_slug: angular-17
slug: angular-17-domain-security
source_filename: angular-17-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: v17.angular.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:07:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: angular.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:52:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: v17.material.angular.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:18:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: angular.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:angular-devinfra@google.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: angular.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angular-17/refs/heads/main/security/angular-17-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Deferrable Views
- Framework
- Frontend
- JavaScript
- Open Source
- Signals
- Single Page Application
- TypeScript
- Web Development
---
