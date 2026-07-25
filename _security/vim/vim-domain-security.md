---
api_specs:
- filename: vim-data-source-openapi-original.json
  format: json
  label: Vim Data Source
  slug: vim-data-source
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-data-source-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getvim.com
  spf: true
hosts:
- cert_expires: Sep 30 00:42:58 2026 GMT
  host: getvim.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 19:21:32 2026 GMT
  host: docs.getvim.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 17:25:55 2026 GMT
  host: api.getvim.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vim, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vim
provider_slug: vim
slug: vim-domain-security
source_filename: vim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getvim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:42:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.getvim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.getvim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:25:55 2026 GMT\n  hsts: null\ndomains:\n- domain: getvim.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/security/vim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United States
- Clinical AI
- EHR Integration
- Point of Care
- Interoperability
- Value-Based Care
- Care Gaps
- OAuth
---
