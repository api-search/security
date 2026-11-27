---
api_specs:
- filename: google-firebase-availableprojects-api-openapi.yml
  format: yaml
  label: Google Firebase Available Projects API
  slug: google-firebase-availableprojects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-firebase/openapi/google-firebase-availableprojects-api-openapi.yml
- filename: google-firebase-jwks-api-openapi.yml
  format: yaml
  label: Google Firebase Jwks API
  slug: google-firebase-jwks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-firebase/openapi/google-firebase-jwks-api-openapi.yml
- filename: google-firebase-media-api-openapi.yml
  format: yaml
  label: Google Firebase Media API
  slug: google-firebase-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-firebase/openapi/google-firebase-media-api-openapi.yml
- filename: google-firebase-oauthclients-api-openapi.yml
  format: yaml
  label: Google Firebase OAUTH Clients API
  slug: google-firebase-oauthclients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-firebase/openapi/google-firebase-oauthclients-api-openapi.yml
- filename: google-firebase-operations-api-openapi.yml
  format: yaml
  label: Google Firebase Operations API
  slug: google-firebase-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-firebase/openapi/google-firebase-operations-api-openapi.yml
- filename: google-firebase-projects-api-openapi.yml
  format: yaml
  label: Google Firebase Projects API
  slug: google-firebase-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-firebase/openapi/google-firebase-projects-api-openapi.yml
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
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: firebase.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: identitytoolkit.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Firebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Firebase, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Firebase
provider_slug: google-firebase
slug: google-firebase-domain-security
source_filename: google-firebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: firebase.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: identitytoolkit.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-firebase/security/google-firebase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Authentication
- Backend-as-a-Service
- Cloud Messaging
- Google Cloud
- Hosting
- Mobile
- Real-Time Database
- Identity Federation
---
