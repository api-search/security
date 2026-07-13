---
api_specs:
- filename: hive-openapi.yml
  format: yaml
  label: Hive Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hive.com
  spf: true
hosts:
- cert_expires: Sep  3 17:19:59 2026 GMT
  host: hive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:10:16 2026 GMT
  host: developers.hive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: app.hive.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hive
provider_slug: hive
slug: hive-domain-security
source_filename: hive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 17:19:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.hive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:10:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.hive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: hive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/security/hive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Project Management
- Task Management
- Team Collaboration
- Productivity
- Workflow Automation
- Time Tracking
---
