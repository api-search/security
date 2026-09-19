---
api_specs:
- filename: hami-robots-txt-api-openapi.yml
  format: yaml
  label: HAMi Robots.txt API
  slug: hami-robots-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hami/refs/heads/main/openapi/hami-robots-txt-api-openapi.yml
- filename: hami-well-known-api-openapi.yml
  format: yaml
  label: HAMi .well Known API
  slug: hami-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hami/refs/heads/main/openapi/hami-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: project-hami.io
  spf: false
hosts:
- cert_expires: Nov  1 11:26:42 2026 GMT
  host: www.project-hami.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 11:26:42 2026 GMT
  host: project-hami.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Hami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HAMi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HAMi
provider_slug: hami
slug: hami-domain-security
source_filename: hami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.project-hami.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 11:26:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: project-hami.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 11:26:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: project-hami.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hami/refs/heads/main/security/hami-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Computing
- CNCF
- GPU Virtualization
- Kubernetes
- GPU Sharing
- Scheduling
- Open-Source
- Infrastructure
- Observability
- Heterogeneous Computing
---
