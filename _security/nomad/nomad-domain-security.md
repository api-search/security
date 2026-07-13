---
api_specs:
- filename: nomad-http-api-openapi.yml
  format: yaml
  label: HashiCorp Nomad HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/openapi/nomad-http-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hashicorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nomadproject.io
  spf: true
hosts:
- cert_expires: Sep 21 05:45:45 2026 GMT
  host: developer.hashicorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 12:40:58 2026 GMT
  host: www.nomadproject.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:57:48 2026 GMT
  host: pkg.go.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nomad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HashiCorp Nomad, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HashiCorp Nomad
provider_slug: nomad
slug: nomad-domain-security
source_filename: nomad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.nomadproject.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:40:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: pkg.go.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:57:48 2026 GMT\n  hsts: false\ndomains:\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nomadproject.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomad/refs/heads/main/security/nomad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Workload Orchestration
- Container Orchestration
- Scheduling
- Infrastructure
- DevOps
---
