---
api_specs:
- filename: firebase-realtime-database-openapi.yml
  format: yaml
  label: Firebase Realtime Database API
  slug: firebase-realtime-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-firebase/refs/heads/main/openapi/firebase-realtime-database-openapi.yml
- filename: firebase-cloud-messaging-openapi.yml
  format: yaml
  label: Firebase Cloud Messaging API (FCM)
  slug: firebase-cloud-messaging-api-fcm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-firebase/refs/heads/main/openapi/firebase-cloud-messaging-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: firebaseio.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: firebase.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: firebaseio.com
  https: false
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: fcm.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Firebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Firebase, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Firebase
provider_slug: google-firebase
slug: google-firebase-domain-security
source_filename: google-firebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firebase.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: firebaseio.com\n  https: false\n- host: fcm.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: firebaseio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-firebase/refs/heads/main/security/google-firebase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Authentication
- Backend as a Service
- Cloud Messaging
- Google Cloud
- Hosting
- Mobile
- Real-Time Database
---
