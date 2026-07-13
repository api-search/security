---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Withings Data API
  slug: withings-data-api
  spec_type: OpenAPI
  url: https://developer.withings.com/api-reference/
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
- OAuth2
- Webhooks
---
