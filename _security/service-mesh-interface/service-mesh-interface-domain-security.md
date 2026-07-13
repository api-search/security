---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: smi-spec.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: default.svc
  spf: false
hosts:
- cert_expires: Sep  8 11:17:02 2026 GMT
  host: smi-spec.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: kubernetes.default.svc
  https: false
kind: domain-security
layout: security
method: probed
name: Service Mesh Interface Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Service Mesh Interface (SMI), probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Service Mesh Interface (SMI)
provider_slug: service-mesh-interface
slug: service-mesh-interface-domain-security
source_filename: service-mesh-interface-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smi-spec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:17:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kubernetes.default.svc\n  https: false\ndomains:\n- domain: smi-spec.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: default.svc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-mesh-interface/refs/heads/main/security/service-mesh-interface-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Service Mesh
- Kubernetes
- Traffic Policy
- Traffic Management
- Traffic Metrics
- Standards
- CNCF
- Archived
- Specification
- Custom Resource Definitions
---
