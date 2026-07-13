---
api_specs:
- filename: volcano-job-openapi.yml
  format: yaml
  label: Volcano Batch Scheduling API
  slug: volcano-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volcano/refs/heads/main/openapi/volcano-job-openapi.yml
- filename: volcano-queue-openapi.yml
  format: yaml
  label: Volcano Queue API
  slug: volcano-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volcano/refs/heads/main/openapi/volcano-queue-openapi.yml
- filename: volcano-podgroup-openapi.yml
  format: yaml
  label: Volcano PodGroup API
  slug: volcano-podgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volcano/refs/heads/main/openapi/volcano-podgroup-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: volcano.sh
  spf: true
hosts:
- cert_expires: Sep 16 05:56:59 2026 GMT
  host: volcano.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Volcano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volcano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Volcano
provider_slug: volcano
slug: volcano-domain-security
source_filename: volcano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volcano.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:56:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: volcano.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volcano/refs/heads/main/security/volcano-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Batch Processing
- Cloud Native
- HPC
- Incubating
- Kubernetes
- Scheduling
- Machine Learning
---
