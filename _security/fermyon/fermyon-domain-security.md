---
api_specs:
- filename: fermyon-openapi.yml
  format: yaml
  label: Fermyon Wasm Functions
  slug: fermyon
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fermyon.com
  spf: true
hosts:
- cert_expires: Sep 10 20:42:46 2026 GMT
  host: developer.fermyon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 19:11:40 2026 GMT
  host: www.fermyon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 20:52:52 2026 GMT
  host: cloud.fermyon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fermyon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fermyon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fermyon
provider_slug: fermyon
slug: fermyon-domain-security
source_filename: fermyon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.fermyon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:42:46 2026 GMT\n  hsts: false\n- host: www.fermyon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:11:40 2026 GMT\n  hsts: null\n- host: cloud.fermyon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:52:52 2026 GMT\n  hsts: false\ndomains:\n- domain: fermyon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/security/fermyon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Compute
- Functions
- WebAssembly
- Serverless
---
