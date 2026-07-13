---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:angular-devinfra@google.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: angular.io
  spf: true
hosts:
- cert_expires: Sep 14 12:43:49 2026 GMT
  host: v14.angular.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 15:44:43 2026 GMT
  host: angular.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:18:58 2026 GMT
  host: v14.material.angular.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Angular 14 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angular 14, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Angular 14
provider_slug: angular-14
slug: angular-14-domain-security
source_filename: angular-14-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: v14.angular.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: angular.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:44:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: v14.material.angular.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:18:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: angular.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:angular-devinfra@google.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angular-14/refs/heads/main/security/angular-14-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Framework
- Frontend
- JavaScript
- Open Source
- Single Page Application
- TypeScript
- Web Development
---
