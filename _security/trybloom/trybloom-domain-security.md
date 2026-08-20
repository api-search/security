---
api_specs:
- filename: trybloom-account-api-openapi.yml
  format: yaml
  label: Bloom Account API
  slug: trybloom-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/openapi/trybloom-account-api-openapi.yml
- filename: trybloom-brands-api-openapi.yml
  format: yaml
  label: Bloom Brands API
  slug: trybloom-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/openapi/trybloom-brands-api-openapi.yml
- filename: trybloom-images-api-openapi.yml
  format: yaml
  label: Bloom Images API
  slug: trybloom-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/openapi/trybloom-images-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trybloom.ai
  spf: true
hosts:
- cert_expires: Nov  2 04:47:13 2026 GMT
  host: www.trybloom.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trybloom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloom
provider_slug: trybloom
slug: trybloom-domain-security
source_filename: trybloom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trybloom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 04:47:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trybloom.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/security/trybloom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Brand Management
- Image-Generation
- Artificial Intelligence
- Agents
- MCP
- Marketing
- Creative
---
