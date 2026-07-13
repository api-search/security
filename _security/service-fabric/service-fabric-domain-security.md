---
api_specs:
- filename: service-fabric-cluster-openapi.yml
  format: yaml
  label: Service Fabric Cluster Management API
  slug: service-fabric-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-fabric/refs/heads/main/openapi/service-fabric-cluster-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Service Fabric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Service Fabric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Service Fabric
provider_slug: service-fabric
slug: service-fabric-domain-security
source_filename: service-fabric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-fabric/refs/heads/main/security/service-fabric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Distributed Systems
- Microservices
- Containers
- Cloud Native
- Kubernetes
- Azure
- Open Source
---
