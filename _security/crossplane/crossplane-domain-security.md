---
api_specs:
- filename: crossplane-kubernetes-api-openapi.yml
  format: yaml
  label: Crossplane Kubernetes API
  slug: crossplane-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossplane/refs/heads/main/openapi/crossplane-kubernetes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crossplane.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: default.svc
  spf: false
hosts:
- cert_expires: Sep 10 21:32:37 2026 GMT
  host: www.crossplane.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 21:32:37 2026 GMT
  host: docs.crossplane.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: kubernetes.default.svc
  https: false
kind: domain-security
layout: security
method: probed
name: Crossplane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossplane, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crossplane
provider_slug: crossplane
slug: crossplane-domain-security
source_filename: crossplane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossplane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 21:32:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.crossplane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 21:32:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kubernetes.default.svc\n  https: false\ndomains:\n- domain: crossplane.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: default.svc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossplane/refs/heads/main/security/crossplane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache 2.0
- CNCF
- Cloud Native
- Composition
- Control Plane
- Custom Resource Definitions
- Graduated
- Infrastructure as Code
- Kubernetes
- Multi-Cloud
- Open Source
- Platform Engineering
- Providers
---
