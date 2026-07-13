---
api_specs:
- filename: patch-io-carbon-api-openapi.yml
  format: yaml
  label: Patch Carbon API
  slug: carbon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch-io/main/openapi/patch-io-carbon-api-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: patch.io
  spf: true
hosts:
- cert_expires: Aug 17 06:01:40 2026 GMT
  host: www.patch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: docs.patch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.patch.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patch Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Patch
provider_slug: patch-io
slug: patch-io-domain-security
source_filename: patch-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.patch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 06:01:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.patch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.patch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: patch.io\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patch-io/refs/heads/main/security/patch-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Climate
- Carbon Credits
- Carbon Removal
- Offsets
- API-First
- Embedded Climate
- Marketplace
- Sustainability
- OpenAPI
- SDKs
---
