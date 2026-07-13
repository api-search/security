---
api_specs:
- filename: trpc-openapi.yml
  format: yaml
  label: tRPC HTTP Protocol
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trpc/refs/heads/main/openapi/trpc-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: trpc.io
  spf: false
hosts:
- cert_expires: Aug 13 23:40:53 2026 GMT
  host: trpc.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trpc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tRPC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: tRPC
provider_slug: trpc
slug: trpc-domain-security
source_filename: trpc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trpc.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:40:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trpc.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trpc/refs/heads/main/security/trpc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- API Composition
- API Framework
- BFF
- End-to-End Type Safety
- RPC
- TypeScript
---
