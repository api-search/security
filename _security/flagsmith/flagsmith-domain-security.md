---
api_specs:
- filename: flagsmith-flags-api-openapi.yml
  format: yaml
  label: Flagsmith Flags API
  slug: flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-flags-api-openapi.yml
- filename: flagsmith-admin-api-openapi.yml
  format: yaml
  label: Flagsmith Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-admin-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flagsmith.com
  spf: true
hosts:
- cert_expires: Aug 17 21:35:17 2026 GMT
  host: docs.flagsmith.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: edge.api.flagsmith.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.flagsmith.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flagsmith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flagsmith, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: flagsmith
provider_slug: flagsmith
slug: flagsmith-domain-security
source_filename: flagsmith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.flagsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:35:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: edge.api.flagsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.flagsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: flagsmith.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/security/flagsmith-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
