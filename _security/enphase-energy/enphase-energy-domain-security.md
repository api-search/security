---
api_specs:
- filename: enphase-enlighten-v4-monitoring-openapi.yml
  format: yaml
  label: Enphase Enlighten Systems API v4 (Monitoring)
  slug: enphase-enlighten-systems-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-enlighten-v4-monitoring-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enphase.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enphaseenergy.com
  spf: true
hosts:
- cert_expires: Jul 30 06:36:52 2026 GMT
  host: enphase.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 11 08:03:02 2026 GMT
  host: developer-v4.enphase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: api.enphaseenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enphase Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enphase Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Enphase Energy
provider_slug: enphase-energy
slug: enphase-energy-domain-security
source_filename: enphase-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enphase.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 30 06:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer-v4.enphase.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 08:03:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.enphaseenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: enphase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: enphaseenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/security/enphase-energy-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Solar
- Energy
- Microinverters
- Battery Storage
- IQ Battery
- IQ Microinverter
- IQ EV Charger
- Enlighten
- Home Energy Management
- Renewable Energy
- Grid Services
- Cleantech
- IoT
- Telemetry
---
