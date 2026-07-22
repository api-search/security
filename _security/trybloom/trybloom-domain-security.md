---
api_specs:
- filename: trybloom-api-openapi.json
  format: json
  label: Bloom API
  slug: bloom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/openapi/trybloom-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trybloom.ai
  spf: true
hosts:
- cert_expires: Aug 31 11:14:19 2026 GMT
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
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trybloom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:14:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trybloom.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/security/trybloom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Brand Management
- Image Generation
- Artificial Intelligence
- Agents
- MCP
- Marketing
- Creative
---
