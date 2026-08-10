---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clockworksanalytics.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: buildingsapi.net
  spf: true
hosts:
- cert_expires: Oct 12 17:02:57 2026 GMT
  host: clockworksanalytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 19:07:32 2027 GMT
  host: cw.clockworksanalytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 12:06:32 2026 GMT
  host: rest.buildingsapi.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clockworks Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clockworks Analytics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clockworks Analytics
provider_slug: clockworks-analytics
slug: clockworks-analytics-domain-security
source_filename: clockworks-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clockworksanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 17:02:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cw.clockworksanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 19:07:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.buildingsapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 12:06:32 2026 GMT\n  hsts: null\ndomains:\n- domain: clockworksanalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: buildingsapi.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clockworks-analytics/refs/heads/main/security/clockworks-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Building Analytics
- Fault Detection and Diagnostics
- HVAC
- Energy Management
- Facilities Management
- Smart Buildings
- CMMS Integration
- Analytics
- Internet of Things
---
