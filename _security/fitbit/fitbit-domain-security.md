---
api_specs:
- filename: fitbit-user-api-openapi.yml
  format: yaml
  label: Fitbit User API
  slug: fitbit-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-user-api-openapi.yml
- filename: fitbit-foods-api-openapi.yml
  format: yaml
  label: Fitbit Foods API
  slug: fitbit-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-foods-api-openapi.yml
- filename: fitbit-oauth2-api-openapi.yml
  format: yaml
  label: Fitbit Oauth2 API
  slug: fitbit-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-oauth2-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dnssec: false
  domain: fitbit.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: about.google
  spf: true
hosts:
- cert_expires: Aug 23 19:41:11 2026 GMT
  host: www.fitbit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 19:41:11 2026 GMT
  host: dev.fitbit.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:56 2026 GMT
  host: about.google
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fitbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fitbit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Fitbit
provider_slug: fitbit
slug: fitbit-domain-security
source_filename: fitbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fitbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:41:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.fitbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:41:11 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: about.google\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fitbit.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n- domain: about.google\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/security/fitbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Wearable
- Health
- Fitness
- Activity Tracking
- Heart Rate
- Sleep
- Google
- IoT
---
