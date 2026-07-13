---
api_specs:
- filename: hotglue-openapi.yml
  format: yaml
  label: Hotglue API V2
  slug: hotglue-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotglue/refs/heads/main/openapi/hotglue-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hotglue.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: hotglue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 18:51:37 2026 GMT
  host: docs.hotglue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.hotglue.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hotglue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hotglue, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hotglue
provider_slug: hotglue
slug: hotglue-domain-security
source_filename: hotglue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotglue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n- host: docs.hotglue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:51:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hotglue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hotglue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotglue/refs/heads/main/security/hotglue-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Connectors
- Embedded Integrations
- ETL
- Integration Platform
- iPaaS
---
