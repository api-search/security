---
api_specs:
- filename: index.html
  format: yaml
  label: Patch API
  slug: patch-api
  spec_type: OpenAPI
  url: https://api.patch.io/api-docs/index.html
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
name: Patch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Patch
provider_slug: patch
slug: patch-domain-security
source_filename: patch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.patch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 06:01:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.patch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.patch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: patch.io\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patch/refs/heads/main/security/patch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carbon
- Carbon Credits
- Carbon Removal
- Carbon Offsets
- Sustainability
- Climate Tech
- Net Zero
- ESG
---
