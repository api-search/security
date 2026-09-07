---
api_specs:
- filename: worklittle-job-boards-api-openapi.yml
  format: yaml
  label: Worklittle Job Boards API
  slug: worklittle-job-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-job-boards-api-openapi.yml
- filename: worklittle-jobs-api-openapi.yml
  format: yaml
  label: Worklittle Jobs API
  slug: worklittle-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-jobs-api-openapi.yml
- filename: worklittle-platform-api-openapi.yml
  format: yaml
  label: Worklittle Business Platform API
  slug: worklittle-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: worklittle.com
  spf: true
hosts:
- cert_expires: Oct 27 12:29:25 2026 GMT
  host: worklittle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 02:12:14 2026 GMT
  host: docs.worklittle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 02:11:08 2026 GMT
  host: api.worklittle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Worklittle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worklittle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Worklittle
provider_slug: worklittle
slug: worklittle-domain-security
source_filename: worklittle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: worklittle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 12:29:25 2026 GMT\n  hsts: false\n- host: docs.worklittle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 02:12:14 2026 GMT\n  hsts: false\n- host: api.worklittle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 02:11:08 2026 GMT\n  hsts: null\ndomains:\n- domain: worklittle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/security/worklittle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Job Search
- ATS
- Recruiting
- Workforce Intelligence
- Job Boards
- Webhooks
- MCP
---
