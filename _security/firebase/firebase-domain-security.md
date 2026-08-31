---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 21 08:37:24 2026 GMT
  host: firebase.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:39:19 2026 GMT
  host: firebase.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:42:48 2026 GMT
  host: firestore.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firebase, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Firebase
provider_slug: firebase
slug: firebase-domain-security
source_filename: firebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firebase.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:37:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: firebase.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:39:19 2026 GMT\n  hsts: null\n- host: firestore.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:42:48 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firebase/refs/heads/main/security/firebase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Backend as a Service
- Application Development
- Mobile
- Web
- Authentication
- Database
- Cloud Functions
- Messaging
- Google
---
