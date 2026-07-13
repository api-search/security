---
api_specs:
- filename: perfectscale-perfectscale-openapi.yml
  format: yaml
  label: PerfectScale Public API
  slug: perfectscale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perfectscale/refs/heads/main/openapi/perfectscale-perfectscale-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perfectscale.io
  spf: true
hosts:
- cert_expires: Sep 24 06:25:24 2026 GMT
  host: www.perfectscale.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: api.app.perfectscale.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perfectscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PerfectScale, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PerfectScale
provider_slug: perfectscale
slug: perfectscale-domain-security
source_filename: perfectscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perfectscale.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:25:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.app.perfectscale.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: perfectscale.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perfectscale/refs/heads/main/security/perfectscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinOps
- Kubernetes
- Cost Optimization
---
