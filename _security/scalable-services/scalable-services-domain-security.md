---
api_specs:
- filename: scalable-services-configmaps-api-openapi.yml
  format: yaml
  label: Scalable Services ConfigMaps API
  slug: scalable-services-configmaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-configmaps-api-openapi.yml
- filename: scalable-services-namespaces-api-openapi.yml
  format: yaml
  label: Scalable Services Namespaces API
  slug: scalable-services-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-namespaces-api-openapi.yml
- filename: scalable-services-nodes-api-openapi.yml
  format: yaml
  label: Scalable Services Nodes API
  slug: scalable-services-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-nodes-api-openapi.yml
- filename: scalable-services-persistentvolumes-api-openapi.yml
  format: yaml
  label: Scalable Services PersistentVolumes API
  slug: scalable-services-persistentvolumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-persistentvolumes-api-openapi.yml
- filename: scalable-services-pods-api-openapi.yml
  format: yaml
  label: Scalable Services Pods API
  slug: scalable-services-pods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-pods-api-openapi.yml
- filename: scalable-services-secrets-api-openapi.yml
  format: yaml
  label: Scalable Services Secrets API
  slug: scalable-services-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-secrets-api-openapi.yml
- filename: scalable-services-services-api-openapi.yml
  format: yaml
  label: Scalable Services Services API
  slug: scalable-services-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-services-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: kubernetes.io
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: envoyproxy.io
  spf: true
hosts:
- cert_expires: Sep 11 09:13:55 2026 GMT
  host: kubernetes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 12:53:48 2026 GMT
  host: www.envoyproxy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 03:23:54 2026 GMT
  host: istio.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalable Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalable Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Scalable Services
provider_slug: scalable-services
slug: scalable-services-domain-security
source_filename: scalable-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubernetes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:13:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.envoyproxy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: istio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:23:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubernetes.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n- domain: envoyproxy.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/security/scalable-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- API Gateway
- Cloud-Native
- Containers
- Distributed Systems
- High Availability
- Kubernetes
- Load Balancing
- Microservices
- Scalable Architecture
- Serverless
- Service Mesh
---
