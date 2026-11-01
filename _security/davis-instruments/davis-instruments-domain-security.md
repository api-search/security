---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: davisinstruments.com
  spf: true
hosts:
- cert_expires: Dec 30 23:51:33 2026 GMT
  host: davisinstruments.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Davis Instruments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Davis Instruments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Davis Instruments
provider_slug: davis-instruments
slug: davis-instruments-domain-security
source_filename: davis-instruments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: davisinstruments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:51:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: davisinstruments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/davis-instruments/security/davis-instruments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Weather
- Instruments
- Sensors
- Environmental
---
