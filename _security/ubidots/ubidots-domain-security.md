---
description: ''
domains:
- caa:
  - 0 iodef "mailto:tls-abuse@ubidots.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ubidots.com
  spf: true
hosts:
- cert_expires: Aug 28 01:11:59 2026 GMT
  host: ubidots.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 17:27:30 2026 GMT
  host: docs.ubidots.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 17:07:21 2026 GMT
  host: industrial.api.ubidots.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubidots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubidots, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ubidots
provider_slug: ubidots
slug: ubidots-domain-security
source_filename: ubidots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ubidots.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 28 01:11:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ubidots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:27:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: industrial.api.ubidots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 17:07:21 2026 GMT\n  hsts: null\ndomains:\n- domain: ubidots.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:tls-abuse@ubidots.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubidots/refs/heads/main/security/ubidots-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- IoT
- Internet of Things
- Telemetry
- Time Series
- MQTT
- REST
- Dashboards
- Device Management
- Analytics
- Industrial IoT
- AIoT
---
