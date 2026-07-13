---
api_specs:
- filename: fumadocs-search-openapi.yml
  format: yaml
  label: Fumadocs Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fumadocs/refs/heads/main/openapi/fumadocs-search-openapi.yml
- filename: fumadocs-openapi-proxy-openapi.yml
  format: yaml
  label: Fumadocs OpenAPI Proxy API
  slug: openapi-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fumadocs/refs/heads/main/openapi/fumadocs-openapi-proxy-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: fumadocs.dev
  spf: false
hosts:
- cert_expires: Sep 27 00:19:01 2026 GMT
  host: fumadocs.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fumadocs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fumadocs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fumadocs
provider_slug: fumadocs
slug: fumadocs-domain-security
source_filename: fumadocs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fumadocs.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fumadocs.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fumadocs/refs/heads/main/security/fumadocs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Documentation
- Framework
- Next.js
- React
---
