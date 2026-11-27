---
api_specs:
- filename: looker-projects-api-openapi.yml
  format: yaml
  label: Looker Projects API
  slug: looker-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/looker/openapi/looker-projects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: looker.com
  spf: true
hosts:
- cert_expires: Dec 30 19:11:15 2026 GMT
  host: looker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 04:22:50 2026 GMT
  host: developers.looker.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: your-instance.looker.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Looker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Looker, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Looker
provider_slug: looker
slug: looker-domain-security
source_filename: looker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: looker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:11:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.looker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 04:22:50 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: your-instance.looker.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: looker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/looker/security/looker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
---
