---
api_specs:
- filename: todoist-openapi.yml
  format: yaml
  label: Todoist API
  slug: todoist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:aws.ops@doist.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: todoist.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: todoist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: developer.todoist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: api.todoist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Todoist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Todoist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Todoist
provider_slug: todoist
slug: todoist-domain-security
source_filename: todoist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: todoist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.todoist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: false\n- host: api.todoist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: todoist.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:aws.ops@doist.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/security/todoist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Tasks
- To-Do
- Task Management
- Collaboration
---
