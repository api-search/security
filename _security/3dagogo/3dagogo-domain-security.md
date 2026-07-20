---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astroprint.com
  spf: true
hosts:
- host: astroprint.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''astroprint.'
kind: domain-security
layout: security
method: probed
name: 3Dagogo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3DaGoGo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 3DaGoGo
provider_slug: 3dagogo
slug: 3dagogo-domain-security
source_filename: 3dagogo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astroprint.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''astroprint.'\n  hsts: null\ndomains:\n- domain: astroprint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3dagogo/refs/heads/main/security/3dagogo-domain-security.yml
summary_line: DMARC
tags:
- Company
- 3D Printing
- Cloud
- Manufacturing
- IoT
- Developer API
- OAuth
---
