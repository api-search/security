---
api_specs:
- filename: monday-com-webhooks-asyncapi.yml
  format: yaml
  label: Monday.com API
  slug: monday-com
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/monday-com/refs/heads/main/asyncapi/monday-com-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: monday.com
  spf: true
hosts:
- cert_expires: Aug 19 00:27:42 2026 GMT
  host: developer.monday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 15:06:09 2026 GMT
  host: api.monday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monday Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monday.com, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Monday.com
provider_slug: monday-com
slug: monday-com-domain-security
source_filename: monday-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.monday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 00:27:42 2026 GMT\n  hsts: null\n- host: api.monday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:06:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monday-com/refs/heads/main/security/monday-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Work Management
- CRM
- Automation
- GraphQL
---
