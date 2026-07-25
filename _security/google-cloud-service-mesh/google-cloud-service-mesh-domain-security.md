---
api_specs:
- filename: google-cloud-service-mesh-endpointpolicies-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh EndpointPolicies API
  slug: google-cloud-service-mesh-endpointpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-endpointpolicies-api-openapi.yml
- filename: google-cloud-service-mesh-gateways-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh Gateways API
  slug: google-cloud-service-mesh-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-gateways-api-openapi.yml
- filename: google-cloud-service-mesh-google-cloud-network-services-api-service-mesh-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh Google Cloud Network Services API (Service Mesh) API
  slug: google-cloud-service-mesh-google-cloud-network-services-api-service-mesh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-google-cloud-network-services-api-service-mesh-api-openapi.yml
- filename: google-cloud-service-mesh-grpcroutes-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh GrpcRoutes API
  slug: google-cloud-service-mesh-grpcroutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-grpcroutes-api-openapi.yml
- filename: google-cloud-service-mesh-httproutes-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh HttpRoutes API
  slug: google-cloud-service-mesh-httproutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-httproutes-api-openapi.yml
- filename: google-cloud-service-mesh-locations-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh Locations API
  slug: google-cloud-service-mesh-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-locations-api-openapi.yml
- filename: google-cloud-service-mesh-meshes-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh Meshes API
  slug: google-cloud-service-mesh-meshes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-meshes-api-openapi.yml
- filename: google-cloud-service-mesh-operations-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh Operations API
  slug: google-cloud-service-mesh-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-operations-api-openapi.yml
- filename: google-cloud-service-mesh-servicelbpolicies-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh ServiceLbPolicies API
  slug: google-cloud-service-mesh-servicelbpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-servicelbpolicies-api-openapi.yml
- filename: google-cloud-service-mesh-tcproutes-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh TcpRoutes API
  slug: google-cloud-service-mesh-tcproutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-tcproutes-api-openapi.yml
- filename: google-cloud-service-mesh-tlsroutes-api-openapi.yml
  format: yaml
  label: Google Cloud Service Mesh TlsRoutes API
  slug: google-cloud-service-mesh-tlsroutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/openapi/google-cloud-service-mesh-tlsroutes-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: networkservices.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: networksecurity.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Cloud Service Mesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Service Mesh, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Service Mesh
provider_slug: google-cloud-service-mesh
slug: google-cloud-service-mesh-domain-security
source_filename: google-cloud-service-mesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: networkservices.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: networksecurity.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-service-mesh/refs/heads/main/security/google-cloud-service-mesh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Google Cloud
- Istio
- Kubernetes
- Microservices
- Service Mesh
---
