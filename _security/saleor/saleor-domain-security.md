---
api_specs:
- filename: saleor-openapi.yml
  format: yaml
  label: Saleor GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saleor/refs/heads/main/openapi/saleor-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:saleor-cloud@saleor.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saleor.io
  spf: true
hosts:
- cert_expires: Sep 26 10:54:13 2026 GMT
  host: saleor.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 22:46:28 2026 GMT
  host: docs.saleor.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: cloud.saleor.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saleor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saleor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Saleor
provider_slug: saleor
slug: saleor-domain-security
source_filename: saleor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saleor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:54:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.saleor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:46:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.saleor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: saleor.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:saleor-cloud@saleor.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saleor/refs/heads/main/security/saleor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Headless
- eCommerce
- GraphQL
- Open Source
- Python
- TypeScript
---
