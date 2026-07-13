---
api_specs:
- filename: apimatic-platform-api.yaml
  format: yaml
  label: APIMatic Platform API
  slug: apimatic-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-platform-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apimatic.io
  spf: true
hosts:
- cert_expires: Sep 23 02:04:05 2026 GMT
  host: www.apimatic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:25:08 2026 GMT
  host: docs.apimatic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.apimatic.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apimatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIMatic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: APIMatic
provider_slug: apimatic
slug: apimatic-domain-security
source_filename: apimatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apimatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:04:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.apimatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:25:08 2026 GMT\n  hsts: false\n- host: api.apimatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: apimatic.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/security/apimatic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Transformation
- Code Generation
- Developer Experience
- Documentation
- SDK Generation
---
