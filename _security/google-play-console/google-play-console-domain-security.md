---
api_specs:
- filename: google-play-console-anomalies-api-openapi.yml
  format: yaml
  label: Google Play Console Developer Reporting Play Console Anomalies API
  slug: google-play-console-anomalies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-play-console/openapi/google-play-console-anomalies-api-openapi.yml
- filename: google-play-console-apps-api-openapi.yml
  format: yaml
  label: Google Play Console Developer Reporting Play Console Apps API
  slug: google-play-console-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-play-console/openapi/google-play-console-apps-api-openapi.yml
- filename: google-play-console-vitals-api-openapi.yml
  format: yaml
  label: Google Play Console Developer Reporting Play Console Vitals API
  slug: google-play-console-vitals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-play-console/openapi/google-play-console-vitals-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: play.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Play Console Developer Reporting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Play Console Developer Reporting, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Play Console Developer Reporting
provider_slug: google-play-console
slug: google-play-console-domain-security
source_filename: google-play-console-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: play.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-play-console/security/google-play-console-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Android
- Application
- Google Play Console
- Quality
- Reporting
---
