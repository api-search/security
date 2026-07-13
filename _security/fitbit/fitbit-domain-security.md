---
api_specs:
- filename: fitbit-activity-api-openapi.yml
  format: yaml
  label: Fitbit Activity API
  slug: fitbit-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-activity-api-openapi.yml
- filename: fitbit-heart-rate-api-openapi.yml
  format: yaml
  label: Fitbit Heart Rate API
  slug: fitbit-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-heart-rate-api-openapi.yml
- filename: fitbit-sleep-api-openapi.yml
  format: yaml
  label: Fitbit Sleep API
  slug: fitbit-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-sleep-api-openapi.yml
- filename: fitbit-body-api-openapi.yml
  format: yaml
  label: Fitbit Body API
  slug: fitbit-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-body-api-openapi.yml
- filename: fitbit-nutrition-api-openapi.yml
  format: yaml
  label: Fitbit Nutrition API
  slug: fitbit-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-nutrition-api-openapi.yml
- filename: fitbit-user-api-openapi.yml
  format: yaml
  label: Fitbit User API
  slug: fitbit-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-user-api-openapi.yml
- filename: fitbit-devices-api-openapi.yml
  format: yaml
  label: Fitbit Devices API
  slug: fitbit-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-devices-api-openapi.yml
- filename: fitbit-subscriptions-api-openapi.yml
  format: yaml
  label: Fitbit Subscriptions API
  slug: fitbit-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-subscriptions-api-openapi.yml
- filename: fitbit-friends-api-openapi.yml
  format: yaml
  label: Fitbit Friends API
  slug: fitbit-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-friends-api-openapi.yml
- filename: fitbit-spo2-breathing-temperature-api-openapi.yml
  format: yaml
  label: Fitbit SpO2, Breathing Rate, Temperature, HRV, and Cardio Fitness API
  slug: fitbit-spo2-breathing-temperature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-spo2-breathing-temperature-api-openapi.yml
- filename: fitbit-ecg-irn-api-openapi.yml
  format: yaml
  label: Fitbit ECG and Irregular Rhythm Notifications API
  slug: fitbit-ecg-irn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-ecg-irn-api-openapi.yml
- filename: fitbit-authorization-api-openapi.yml
  format: yaml
  label: Fitbit Authorization API
  slug: fitbit-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-authorization-api-openapi.yml
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
