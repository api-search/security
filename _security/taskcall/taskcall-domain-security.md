---
api_specs:
- filename: taskcall-openapi.yml
  format: yaml
  label: TaskCall Incidents API
  slug: incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskcall/refs/heads/main/openapi/taskcall-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: taskcallapp.com
  spf: true
hosts:
- cert_expires: Oct  2 06:21:47 2026 GMT
  host: taskcallapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 06:21:47 2026 GMT
  host: docs.taskcallapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 19:06:43 2026 GMT
  host: incidents-api.taskcallapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taskcall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaskCall, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TaskCall
provider_slug: taskcall
slug: taskcall-domain-security
source_filename: taskcall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taskcallapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:21:47 2026 GMT\n  hsts: null\n- host: docs.taskcallapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:21:47 2026 GMT\n  hsts: null\n- host: incidents-api.taskcallapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:06:43 2026 GMT\n  hsts: null\ndomains:\n- domain: taskcallapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskcall/refs/heads/main/security/taskcall-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Incident Management
- On-Call
- Alerting
- DevOps
- SRE
- ITSM
---
