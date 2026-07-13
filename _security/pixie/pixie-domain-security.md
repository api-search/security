---
api_specs:
- filename: pixie-openapi.yml
  format: yaml
  label: Pixie API
  slug: pixie
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixie/refs/heads/main/openapi/pixie-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: px.dev
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: withpixie.ai
  spf: false
hosts:
- cert_expires: Sep 24 05:28:21 2026 GMT
  host: px.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 05:28:21 2026 GMT
  host: docs.px.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:08:26 2026 GMT
  host: work.withpixie.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixie, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pixie
provider_slug: pixie
slug: pixie-domain-security
source_filename: pixie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: px.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.px.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: work.withpixie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:08:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: px.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: withpixie.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixie/refs/heads/main/security/pixie-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- eBPF
- Kubernetes
- Monitoring
- Observability
---
