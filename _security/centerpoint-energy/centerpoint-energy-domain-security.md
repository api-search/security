---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centerpointenergy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smartmetertexas.com
  spf: true
hosts:
- cert_expires: Nov 19 22:49:58 2026 GMT
  host: www.centerpointenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 03:58:10 2026 GMT
  host: www.smartmetertexas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: services.smartmetertexas.net
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Centerpoint Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CenterPoint Energy, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CenterPoint Energy
provider_slug: centerpoint-energy
slug: centerpoint-energy-domain-security
source_filename: centerpoint-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centerpointenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 22:49:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.smartmetertexas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 03:58:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.smartmetertexas.net\n  https: false\ndomains:\n- domain: centerpointenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: smartmetertexas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centerpoint-energy/refs/heads/main/security/centerpoint-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EDI
- ERCOT
- Electricity
- Energy
- Fortune 500
- Green Button
- Interval Data
- NAESB ESPI
- Natural Gas
- Smart Meter
- Texas
- TxSET
- Usage Data
- Utility
---
