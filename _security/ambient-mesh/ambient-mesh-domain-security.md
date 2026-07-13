---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ambientmesh.io
  spf: false
hosts:
- cert_expires: Sep 15 14:03:46 2026 GMT
  host: ambientmesh.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambient Mesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambient Mesh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ambient Mesh
provider_slug: ambient-mesh
slug: ambient-mesh-domain-security
source_filename: ambient-mesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ambientmesh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:03:46 2026 GMT\n  hsts: false\ndomains:\n- domain: ambientmesh.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambient-mesh/refs/heads/main/security/ambient-mesh-domain-security.yml
summary_line: TLSv1.3
tags:
- Service Mesh
- Istio
- Kubernetes
- Zero Trust
- Observability
- Traffic Management
- Microservices
---
