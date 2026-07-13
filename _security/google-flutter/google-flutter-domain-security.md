---
api_specs:
- filename: flutter-pub-dev-openapi.yml
  format: yaml
  label: Pub.dev API
  slug: pubdev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-flutter/refs/heads/main/openapi/flutter-pub-dev-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flutter.dev
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pub.dev
  spf: true
hosts:
- cert_expires: Aug 25 23:13:47 2026 GMT
  host: flutter.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 21:28:38 2026 GMT
  host: pub.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Flutter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Flutter, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Flutter
provider_slug: google-flutter
slug: google-flutter-domain-security
source_filename: google-flutter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flutter.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:13:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: pub.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:28:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flutter.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pub.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-flutter/refs/heads/main/security/google-flutter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cross-Platform
- Dart
- Google
- Mobile Development
- Open Source
- UI Framework
---
