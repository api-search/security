---
api_specs:
- filename: bmw-cardata-customer-api-openapi.json
  format: json
  label: BMW CarData Customer API
  slug: bmw-cardata-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmw-connecteddrive/refs/heads/main/openapi/bmw-cardata-customer-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bmw.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bmwgroup.com
  spf: true
hosts:
- cert_expires: Aug 10 06:27:36 2026 GMT
  host: www.bmw.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 05:20:55 2026 GMT
  host: www.bmwgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 03:06:43 2026 GMT
  host: bmw-cardata.bmwgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bmw Connecteddrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BMW ConnectedDrive, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BMW ConnectedDrive
provider_slug: bmw-connecteddrive
slug: bmw-connecteddrive-domain-security
source_filename: bmw-connecteddrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bmw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 06:27:36 2026 GMT\n  hsts: null\n- host: www.bmwgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:20:55 2026 GMT\n  hsts: null\n- host: bmw-cardata.bmwgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 03:06:43 2026 GMT\n  hsts: null\ndomains:\n- domain: bmw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bmwgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmw-connecteddrive/refs/heads/main/security/bmw-connecteddrive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Connected Vehicle
- Telematics
- Vehicle Data
- CarData
- ConnectedDrive
- Electric Vehicles
- Charging
- MQTT
- Streaming
- OAuth
- Device Code Flow
- GDPR
- Right To Repair
- Mobility
---
