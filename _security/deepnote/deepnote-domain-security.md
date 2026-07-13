---
api_specs:
- filename: deepnote-openapi.yml
  format: yaml
  label: Deepnote Execution API (Notebooks/Projects)
  slug: execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-openapi.yml
- filename: deepnote-openapi.yml
  format: yaml
  label: Deepnote Projects API
  slug: projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepnote.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: deepnote.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 15:38:27 2026 GMT
  host: api.deepnote.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepnote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepnote, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deepnote
provider_slug: deepnote
slug: deepnote-domain-security
source_filename: deepnote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.deepnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:38:27 2026 GMT\n  hsts: null\ndomains:\n- domain: deepnote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/security/deepnote-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Science
- Notebooks
- Analytics
- Collaboration
- Data Apps
---
