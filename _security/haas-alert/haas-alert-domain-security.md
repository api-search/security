---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: haasalert.com
  spf: true
hosts:
- cert_expires: Sep 28 05:24:35 2026 GMT
  host: haasalert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Haas Alert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HAAS Alert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HAAS Alert
provider_slug: haas-alert
slug: haas-alert-domain-security
source_filename: haas-alert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haasalert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:24:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: haasalert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haas-alert/refs/heads/main/security/haas-alert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Connected Vehicle
- Road Safety
- Emergency Response
- Fleet Telematics
- V2X
- Automotive
- Public Safety
---
