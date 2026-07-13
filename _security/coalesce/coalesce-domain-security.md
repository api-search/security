---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Coalesce API
  slug: coalesce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coalesce.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coalescesoftware.io
  spf: true
hosts:
- cert_expires: Oct  5 09:42:43 2026 GMT
  host: coalesce.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 04:44:14 2026 GMT
  host: docs.coalesce.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 21:10:21 2026 GMT
  host: app.coalescesoftware.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coalesce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coalesce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coalesce
provider_slug: coalesce
slug: coalesce-domain-security
source_filename: coalesce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coalesce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 09:42:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.coalesce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 04:44:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.coalescesoftware.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:10:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coalesce.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: coalescesoftware.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coalesce/refs/heads/main/security/coalesce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Transformation
- Snowflake
- Data Pipelines
- Data Catalog
- Data Quality
- Analytics
- AI
---
