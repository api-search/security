---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: climeworks.com
  spf: true
hosts:
- cert_expires: Sep 21 14:41:13 2026 GMT
  host: climeworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 06:52:54 2026 GMT
  host: platform.climeworks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Climeworks customer platform login, served on Salesforce Experience Cloud (siteforce); added manually because it is an apis.yml Login property rather than a Website/baseURL host.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Climeworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Climeworks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Climeworks
provider_slug: climeworks
slug: climeworks-domain-security
source_filename: climeworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: climeworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:41:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.climeworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 06:52:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Climeworks customer platform login, served on Salesforce Experience Cloud\n    (siteforce); added manually because it is an apis.yml Login property rather than\n    a Website/baseURL host.\ndomains:\n- domain: climeworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climeworks/refs/heads/main/security/climeworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Carbon Removal
- Direct Air Capture
- Carbon Dioxide Removal
- Climate Tech
- Sustainability
- Energy
- Switzerland
---
