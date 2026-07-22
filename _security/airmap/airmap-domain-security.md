---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airmap.com
  spf: true
hosts:
- host: airmap.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''airmap.com'''
kind: domain-security
layout: security
method: probed
name: Airmap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirMap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AirMap
provider_slug: airmap
slug: airmap-domain-security
source_filename: airmap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airmap.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''airmap.com'''\n  hsts: null\ndomains:\n- domain: airmap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airmap/refs/heads/main/security/airmap-domain-security.yml
summary_line: DMARC
tags:
- Company
- Infrastructure
- Drones
- Airspace
- Unmanned Traffic Management
- Aviation
- Geospatial
- Defunct
---
