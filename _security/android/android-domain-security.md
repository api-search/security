---
api_specs:
- filename: google-play-developer-api.yml
  format: yaml
  label: Google Play Developer APIs
  slug: google-play-developer-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/openapi/google-play-developer-api.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: android.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Sep 14 08:37:12 2026 GMT
  host: developer.android.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: firebase.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Android Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Android, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Android
provider_slug: android
slug: android-domain-security
source_filename: android-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.android.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: firebase.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: android.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/security/android-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
---
