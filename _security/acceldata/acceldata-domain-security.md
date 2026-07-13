---
api_specs:
- filename: acceldata-adoc-api.yaml
  format: yaml
  label: Acceldata Data Observability Cloud API
  slug: adoc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-adoc-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acceldata.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: acceldata.app
  spf: false
hosts:
- cert_expires: Aug 16 23:33:50 2026 GMT
  host: www.acceldata.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: accounts.acceldata.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:22:21 2026 GMT
  host: docs.acceldata.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Acceldata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acceldata, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acceldata
provider_slug: acceldata
slug: acceldata-domain-security
source_filename: acceldata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acceldata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: accounts.acceldata.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.acceldata.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 08:22:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acceldata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: acceldata.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/security/acceldata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
---
