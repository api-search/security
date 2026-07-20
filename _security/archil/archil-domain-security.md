---
api_specs:
- filename: archil-openapi-original.yml
  format: yaml
  label: Archil Control Plane API
  slug: archil-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archil/refs/heads/main/openapi/archil-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: archil.com
  spf: true
hosts:
- cert_expires: Aug 19 20:46:33 2026 GMT
  host: archil.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:21:43 2026 GMT
  host: docs.archil.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: control.green.us-east-1.aws.prod.archil.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Archil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archil, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Archil
provider_slug: archil
slug: archil-domain-security
source_filename: archil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: archil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 20:46:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.archil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:21:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: control.green.us-east-1.aws.prod.archil.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: archil.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archil/refs/heads/main/security/archil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Storage
- Filesystem
- Object Storage
- Artificial Intelligence
- Infrastructure
- Developer Tools
- Serverless
- Data
- S3
---
