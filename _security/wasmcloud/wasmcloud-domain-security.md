---
api_specs:
- filename: wasmcloud-control-asyncapi.yml
  format: yaml
  label: wasmCloud Control Interface API
  slug: wasmcloud-control-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmcloud/refs/heads/main/asyncapi/wasmcloud-control-asyncapi.yml
- filename: wasmcloud-wadm-asyncapi.yml
  format: yaml
  label: wasmCloud Application Deployment Manager (wadm) API
  slug: wasmcloud-wadm-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wasmcloud/refs/heads/main/asyncapi/wasmcloud-wadm-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wasmcloud.com
  spf: true
hosts:
- cert_expires: Sep 18 04:15:22 2026 GMT
  host: wasmcloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wasmcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wasmCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: wasmCloud
provider_slug: wasmcloud
slug: wasmcloud-domain-security
source_filename: wasmcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wasmcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:15:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wasmcloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wasmcloud/refs/heads/main/security/wasmcloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- CNCF
- Distributed Systems
- Incubating
- Runtime
- Wasm
- WebAssembly
- WIT
---
