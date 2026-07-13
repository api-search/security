---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openservicemesh.io
  spf: false
hosts:
- cert_expires: Sep 16 17:06:41 2026 GMT
  host: openservicemesh.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Service Mesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Service Mesh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Service Mesh
provider_slug: open-service-mesh
slug: open-service-mesh-domain-security
source_filename: open-service-mesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openservicemesh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 17:06:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openservicemesh.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-service-mesh/refs/heads/main/security/open-service-mesh-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Envoy
- Kubernetes
- Microservices
- Service Mesh
- SMI
---
