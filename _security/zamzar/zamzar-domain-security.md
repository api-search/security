---
api_specs:
- filename: spec.yaml
  format: yaml
  label: Zamzar File Conversion API
  slug: zamzar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/zamzar/zamzar-spec/main/openapi/spec.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zamzar.com
  spf: true
hosts:
- cert_expires: Oct 30 13:42:47 2026 GMT
  host: www.zamzar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 30 13:42:47 2026 GMT
  host: developers.zamzar.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 30 13:42:47 2026 GMT
  host: api.zamzar.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zamzar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zamzar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zamzar
provider_slug: zamzar
slug: zamzar-domain-security
source_filename: zamzar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zamzar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 13:42:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.zamzar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 13:42:47 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.zamzar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 13:42:47 2026 GMT\n  hsts: null\ndomains:\n- domain: zamzar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zamzar/refs/heads/main/security/zamzar-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- File Conversion
- Documents
- Video
- Audio
- Images
- CAD
- REST API
---
