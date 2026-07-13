---
api_specs:
- filename: spanning-google-workspace-api-openapi.yml
  format: yaml
  label: Spanning Backup for Google Workspace API
  slug: spanning-google-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spanning/refs/heads/main/openapi/spanning-google-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spanning.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: spanningbackup.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: spanning.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.spanningbackup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: o365-us.spanningbackup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spanning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spanning, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spanning
provider_slug: spanning
slug: spanning-domain-security
source_filename: spanning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spanning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.spanningbackup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: o365-us.spanningbackup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spanning.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spanningbackup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spanning/refs/heads/main/security/spanning-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Protection
- SaaS Backup
- Cloud Backup
- Microsoft 365
- Google Workspace
- Salesforce
---
