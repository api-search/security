---
api_specs:
- filename: trefle-openapi.yml
  format: yaml
  label: Trefle API
  slug: trefle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trefle.io
  spf: true
hosts:
- cert_expires: Aug 10 22:36:09 2026 GMT
  host: trefle.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trefle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trefle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trefle
provider_slug: trefle
slug: trefle-domain-security
source_filename: trefle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trefle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 22:36:09 2026 GMT\n  hsts: false\ndomains:\n- domain: trefle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/security/trefle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agriculture
- Botany
- Open Data
- Plants
- Science
---
