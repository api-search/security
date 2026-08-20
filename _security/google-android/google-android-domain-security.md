---
api_specs:
- filename: google-android-android-management-api-api-openapi.yml
  format: yaml
  label: Google Android Android Management API API
  slug: google-android-android-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-android-management-api-api-openapi.yml
- filename: google-android-device-api-openapi.yml
  format: yaml
  label: Google Android Device API
  slug: google-android-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-device-api-openapi.yml
- filename: google-android-devices-api-openapi.yml
  format: yaml
  label: Google Android Devices API
  slug: google-android-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-devices-api-openapi.yml
- filename: google-android-enrollmenttokens-api-openapi.yml
  format: yaml
  label: Google Android EnrollmentTokens API
  slug: google-android-enrollmenttokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-enrollmenttokens-api-openapi.yml
- filename: google-android-enterprises-api-openapi.yml
  format: yaml
  label: Google Android Enterprises API
  slug: google-android-enterprises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-enterprises-api-openapi.yml
- filename: google-android-policies-api-openapi.yml
  format: yaml
  label: Google Android Policies API
  slug: google-android-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-policies-api-openapi.yml
- filename: google-android-policy-api-openapi.yml
  format: yaml
  label: Google Android Policy API
  slug: google-android-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-policy-api-openapi.yml
- filename: google-android-webapps-api-openapi.yml
  format: yaml
  label: Google Android WebApps API
  slug: google-android-webapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-webapps-api-openapi.yml
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
- Open-Source
---
