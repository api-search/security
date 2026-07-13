---
api_specs:
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Connections API
  slug: rutter-io-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Accounting API
  slug: rutter-io-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Commerce API
  slug: rutter-io-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Payments API
  slug: rutter-io-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Webhooks API
  slug: rutter-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rutter.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rutterapi.com
  spf: true
hosts:
- cert_expires: Oct  1 16:55:23 2026 GMT
  host: www.rutter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 10:48:13 2026 GMT
  host: docs.rutterapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 05:35:06 2026 GMT
  host: production.rutterapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rutter Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rutter, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rutter
provider_slug: rutter-io
slug: rutter-io-domain-security
source_filename: rutter-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rutter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 16:55:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rutterapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:48:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: production.rutterapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 05:35:06 2026 GMT\n  hsts: null\ndomains:\n- domain: rutter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rutterapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/security/rutter-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Unified API
- Accounting
- Commerce
- Payments
- Business Data
- Integrations
---
