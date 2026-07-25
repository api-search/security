---
api_specs:
- filename: kubernetes-services-endpointslices-api-openapi.yml
  format: yaml
  label: Kubernetes Services EndpointSlices API
  slug: kubernetes-services-endpointslices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-endpointslices-api-openapi.yml
- filename: kubernetes-services-gateway-api-openapi.yml
  format: yaml
  label: Kubernetes Services Gateway API
  slug: kubernetes-services-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-gateway-api-openapi.yml
- filename: kubernetes-services-gatewayclass-api-openapi.yml
  format: yaml
  label: Kubernetes Services GatewayClass API
  slug: kubernetes-services-gatewayclass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-gatewayclass-api-openapi.yml
- filename: kubernetes-services-grpcroute-api-openapi.yml
  format: yaml
  label: Kubernetes Services GRPCRoute API
  slug: kubernetes-services-grpcroute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-grpcroute-api-openapi.yml
- filename: kubernetes-services-httproute-api-openapi.yml
  format: yaml
  label: Kubernetes Services HTTPRoute API
  slug: kubernetes-services-httproute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-httproute-api-openapi.yml
- filename: kubernetes-services-ingress-api-openapi.yml
  format: yaml
  label: Kubernetes Services Ingress API
  slug: kubernetes-services-ingress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-ingress-api-openapi.yml
- filename: kubernetes-services-ingressclass-api-openapi.yml
  format: yaml
  label: Kubernetes Services IngressClass API
  slug: kubernetes-services-ingressclass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-ingressclass-api-openapi.yml
- filename: kubernetes-services-ingressstatus-api-openapi.yml
  format: yaml
  label: Kubernetes Services IngressStatus API
  slug: kubernetes-services-ingressstatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-ingressstatus-api-openapi.yml
- filename: kubernetes-services-namespaces-api-openapi.yml
  format: yaml
  label: Kubernetes Services Namespaces API
  slug: kubernetes-services-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-namespaces-api-openapi.yml
- filename: kubernetes-services-networkpolicy-api-openapi.yml
  format: yaml
  label: Kubernetes Services NetworkPolicy API
  slug: kubernetes-services-networkpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-networkpolicy-api-openapi.yml
- filename: kubernetes-services-services-api-openapi.yml
  format: yaml
  label: Kubernetes Services Services API
  slug: kubernetes-services-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-services-api-openapi.yml
- filename: kubernetes-services-servicestatus-api-openapi.yml
  format: yaml
  label: Kubernetes Services ServiceStatus API
  slug: kubernetes-services-servicestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/openapi/kubernetes-services-servicestatus-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: kubernetes.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: default.svc
  spf: false
hosts:
- cert_expires: Sep 11 09:13:55 2026 GMT
  host: kubernetes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: kubernetes.default.svc
  https: false
kind: domain-security
layout: security
method: probed
name: Kubernetes Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubernetes Services, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kubernetes Services
provider_slug: kubernetes-services
slug: kubernetes-services-domain-security
source_filename: kubernetes-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubernetes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:13:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kubernetes.default.svc\n  https: false\ndomains:\n- domain: kubernetes.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n- domain: default.svc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubernetes-services/refs/heads/main/security/kubernetes-services-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Container Orchestration
- Kubernetes
- Load Balancing
- Networking
- Service Discovery
---
