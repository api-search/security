---
api_specs:
- filename: wasmer-openapi.yml
  format: yaml
  label: Wasmer Registry GraphQL API
  slug: wasmer-registry-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/openapi/wasmer-openapi.yml
- filename: wasmer-openapi.yml
  format: yaml
  label: Wasmer Packages and Namespaces API
  slug: wasmer-packages-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/openapi/wasmer-openapi.yml
- filename: wasmer-openapi.yml
  format: yaml
  label: Wasmer Apps and Edge Deployments API
  slug: wasmer-apps-edge-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/openapi/wasmer-openapi.yml
- filename: wasmer-openapi.yml
  format: yaml
  label: Wasmer Users and Auth API
  slug: wasmer-users-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/openapi/wasmer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wasmer.io
  spf: true
hosts:
- cert_expires: Aug 19 06:32:08 2026 GMT
  host: wasmer.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 18:10:44 2026 GMT
  host: docs.wasmer.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: registry.wasmer.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wasmer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wasmer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wasmer
provider_slug: wasmer
slug: wasmer-domain-security
source_filename: wasmer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wasmer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 06:32:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.wasmer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:10:44 2026 GMT\n  hsts: false\n- host: registry.wasmer.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wasmer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wasmer/refs/heads/main/security/wasmer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- WebAssembly
- Wasm
- Registry
- Edge
- Runtime
---
