---
api_specs:
- filename: monad-openapi.yml
  format: yaml
  label: Monad JSON-RPC API
  slug: json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monad/refs/heads/main/openapi/monad-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: monad.xyz
  spf: true
hosts:
- cert_expires: Aug 10 15:41:55 2026 GMT
  host: www.monad.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:42:55 2026 GMT
  host: docs.monad.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 19:36:33 2026 GMT
  host: rpc.monad.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monad, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Monad
provider_slug: monad
slug: monad-domain-security
source_filename: monad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monad.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 15:41:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.monad.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:42:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rpc.monad.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 19:36:33 2026 GMT\n  hsts: null\ndomains:\n- domain: monad.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monad/refs/heads/main/security/monad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Layer 1
- EVM
- High Performance
- Parallel Execution
- JSON-RPC
- MonadBFT
---
