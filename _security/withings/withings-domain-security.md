---
api_specs:
- filename: withings-answers-api-openapi.yml
  format: yaml
  label: Withings answers API
  slug: withings-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-answers-api-openapi.yml
- filename: withings-device-api-openapi.yml
  format: yaml
  label: Withings device API
  slug: withings-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-device-api-openapi.yml
- filename: withings-dropshipment-api-openapi.yml
  format: yaml
  label: Withings dropshipment API
  slug: withings-dropshipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-dropshipment-api-openapi.yml
- filename: withings-heart-api-openapi.yml
  format: yaml
  label: Withings heart API
  slug: withings-heart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-heart-api-openapi.yml
- filename: withings-measure-api-openapi.yml
  format: yaml
  label: Withings measure API
  slug: withings-measure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-measure-api-openapi.yml
- filename: withings-notify-api-openapi.yml
  format: yaml
  label: Withings notify API
  slug: withings-notify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-notify-api-openapi.yml
- filename: withings-nudge-api-openapi.yml
  format: yaml
  label: Withings nudge API
  slug: withings-nudge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-nudge-api-openapi.yml
- filename: withings-nudgecampaign-api-openapi.yml
  format: yaml
  label: Withings nudgecampaign API
  slug: withings-nudgecampaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-nudgecampaign-api-openapi.yml
- filename: withings-oauth2-api-openapi.yml
  format: yaml
  label: Withings oauth2 API
  slug: withings-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-oauth2-api-openapi.yml
- filename: withings-order-api-openapi.yml
  format: yaml
  label: Withings order API
  slug: withings-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-order-api-openapi.yml
- filename: withings-rawdata-api-openapi.yml
  format: yaml
  label: Withings rawdata API
  slug: withings-rawdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-rawdata-api-openapi.yml
- filename: withings-signature-api-openapi.yml
  format: yaml
  label: Withings signature API
  slug: withings-signature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-signature-api-openapi.yml
- filename: withings-sleep-api-openapi.yml
  format: yaml
  label: Withings sleep API
  slug: withings-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-sleep-api-openapi.yml
- filename: withings-stetho-api-openapi.yml
  format: yaml
  label: Withings stetho API
  slug: withings-stetho-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-stetho-api-openapi.yml
- filename: withings-survey-api-openapi.yml
  format: yaml
  label: Withings survey API
  slug: withings-survey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-survey-api-openapi.yml
- filename: withings-user-api-openapi.yml
  format: yaml
  label: Withings user API
  slug: withings-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: withings.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: withings.net
  spf: true
hosts:
- cert_expires: Sep 14 15:05:46 2026 GMT
  host: www.withings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:05:46 2026 GMT
  host: developer.withings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:05:46 2026 GMT
  host: wbsapi.withings.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Withings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Withings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Withings
provider_slug: withings
slug: withings-domain-security
source_filename: withings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:05:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.withings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:05:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wbsapi.withings.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:05:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: withings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: withings.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/security/withings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Wearables
- Connected Devices
- Body Composition
- Sleep Tracking
- Blood Pressure
- Activity Tracking
- Remote Patient Monitoring
- Authentication
- Webhook
---
