---
api_specs:
- filename: frankfurter-v2-openapi.yml
  format: yaml
  label: Frankfurter API v2
  slug: frankfurter-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankfurter/refs/heads/main/openapi/frankfurter-v2-openapi.yml
- filename: frankfurter-v1-openapi.yml
  format: yaml
  label: Frankfurter API v1
  slug: frankfurter-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankfurter/refs/heads/main/openapi/frankfurter-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frankfurter.dev
  spf: false
hosts:
- cert_expires: Aug 24 16:27:24 2026 GMT
  host: frankfurter.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:27:24 2026 GMT
  host: api.frankfurter.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frankfurter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frankfurter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Frankfurter
provider_slug: frankfurter
slug: frankfurter-domain-security
source_filename: frankfurter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frankfurter.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:27:24 2026 GMT\n  hsts: false\n- host: api.frankfurter.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:27:24 2026 GMT\n  hsts: false\ndomains:\n- domain: frankfurter.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frankfurter/refs/heads/main/security/frankfurter-domain-security.yml
summary_line: TLSv1.3
tags:
- Currency Exchange
- Foreign Exchange
- FX
- Open Source
- MIT
- Self-Hosted
- Public APIs
---
