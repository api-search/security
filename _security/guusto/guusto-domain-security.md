---
api_specs:
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Gifts API
  slug: guusto-gifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Account Budget API
  slug: guusto-account-budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Reports API
  slug: guusto-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: guusto.com
  spf: true
hosts:
- cert_expires: Sep 21 01:31:54 2026 GMT
  host: guusto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 12:13:49 2026 GMT
  host: docs.guusto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 18:36:16 2026 GMT
  host: api.guusto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guusto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guusto, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Guusto
provider_slug: guusto
slug: guusto-domain-security
source_filename: guusto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guusto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:31:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.guusto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 12:13:49 2026 GMT\n  hsts: null\n- host: api.guusto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:36:16 2026 GMT\n  hsts: null\ndomains:\n- domain: guusto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/security/guusto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Employee Recognition
- Rewards
- Gifting
- Gift Cards
- HR
- Rewards and Recognition
---
