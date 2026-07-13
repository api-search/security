---
api_specs:
- filename: rest
  format: yaml
  label: Android Management API
  slug: android-management-api
  spec_type: OpenAPI
  url: https://androidmanagement.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Play Developer API
  slug: google-play-developer-api
  spec_type: OpenAPI
  url: https://androidpublisher.googleapis.com/$discovery/rest?version=v3
- filename: rest
  format: yaml
  label: Firebase Cloud Messaging API
  slug: firebase-cloud-messaging-api
  spec_type: OpenAPI
  url: https://fcm.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Play Games Services API
  slug: google-play-games-services-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/games/v1/rest
- filename: rest
  format: yaml
  label: Android Over the Air API
  slug: android-over-the-air-api
  spec_type: OpenAPI
  url: https://androidovertheair.googleapis.com/$discovery/rest?version=v1
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
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.android.com
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
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: androidmanagement.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Android Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Android, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Android
provider_slug: google-android
slug: google-android-domain-security
source_filename: google-android-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.android.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: androidmanagement.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: android.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/security/google-android-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Android
- Google
- Mobile Development
- Mobile Operating System
- Open Source
---
