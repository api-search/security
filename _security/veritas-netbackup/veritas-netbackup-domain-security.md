---
api_specs:
- filename: veritas-netbackup-rest-api-openapi.yml
  format: yaml
  label: Veritas NetBackup REST API
  slug: veritas-netbackup-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/openapi/veritas-netbackup-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: veritas.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.veritas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veritas Netbackup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veritas NetBackup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
slug: veritas-netbackup-domain-security
source_filename: veritas-netbackup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veritas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: veritas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/security/veritas-netbackup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
---
