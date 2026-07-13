---
api_specs:
- filename: chaos-mesh-dashboard-api-openapi.yml
  format: yaml
  label: Chaos Mesh API
  slug: chaos-mesh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/openapi/chaos-mesh-dashboard-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chaos-mesh.org
  spf: false
hosts:
- cert_expires: Sep 25 11:30:22 2026 GMT
  host: chaos-mesh.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chaos Mesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chaos Mesh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Chaos Mesh
provider_slug: chaos-mesh
slug: chaos-mesh-domain-security
source_filename: chaos-mesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaos-mesh.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: chaos-mesh.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaos-mesh/refs/heads/main/security/chaos-mesh-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Chaos Engineering
- Cloud Native
- CNCF
- Fault Injection
- Kubernetes
- Observability
- Open Source
- Reliability
- Resilience
- Testing
---
