---
api_specs:
- filename: openapi.json
  format: json
  label: Veritas Cluster Server REST API
  slug: veritas-cluster-server-rest-api
  spec_type: OpenAPI
  url: https://vcs-server:14150/api/docs/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: veritas.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: my.veritas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.veritas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veritas Cluster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veritas Cluster Server, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Veritas Cluster Server
provider_slug: veritas-cluster
slug: veritas-cluster-domain-security
source_filename: veritas-cluster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: my.veritas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.veritas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: veritas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritas-cluster/refs/heads/main/security/veritas-cluster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Clustering
- Containers
- Disaster Recovery
- Failover
- High Availability
- InfoScale
- Infrastructure Management
- Kubernetes
- Storage Management
- Veritas
---
