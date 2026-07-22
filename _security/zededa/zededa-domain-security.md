---
api_specs:
- filename: zededa-node_service-openapi.json
  format: json
  label: ZEDEDA Edge Node Service
  slug: zededa-edge-node-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-node_service-openapi.json
- filename: zededa-app_service-openapi.json
  format: json
  label: ZEDEDA Edge Application Service
  slug: zededa-edge-application-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-app_service-openapi.json
- filename: zededa-app_profile_service-openapi.json
  format: json
  label: ZEDEDA App Profiles Service
  slug: zededa-app-profiles-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-app_profile_service-openapi.json
- filename: zededa-network_service-openapi.json
  format: json
  label: ZEDEDA Edge Network Service
  slug: zededa-edge-network-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-network_service-openapi.json
- filename: zededa-storage_service-openapi.json
  format: json
  label: ZEDEDA Storage Service
  slug: zededa-storage-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-storage_service-openapi.json
- filename: zededa-kubernetes_service-openapi.json
  format: json
  label: ZEDEDA Kubernetes Service (ZKS)
  slug: zededa-kubernetes-service-zks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-kubernetes_service-openapi.json
- filename: zededa-node_cluster_service-openapi.json
  format: json
  label: ZEDEDA Edge-Node Cluster Service
  slug: zededa-edge-node-cluster-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-node_cluster_service-openapi.json
- filename: zededa-user_service-openapi.json
  format: json
  label: ZEDEDA IAM Service
  slug: zededa-iam-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-user_service-openapi.json
- filename: zededa-job_service-openapi.json
  format: json
  label: ZEDEDA Job Service
  slug: zededa-job-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-job_service-openapi.json
- filename: zededa-diag_service-openapi.json
  format: json
  label: ZEDEDA Diagnostics Service
  slug: zededa-diagnostics-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-diag_service-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zededa.com
  spf: true
hosts:
- cert_expires: Sep 15 10:44:24 2026 GMT
  host: zededa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zededa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zededa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zededa
provider_slug: zededa
slug: zededa-domain-security
source_filename: zededa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zededa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:44:24 2026 GMT\n  hsts: false\ndomains:\n- domain: zededa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/security/zededa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Edge Computing
- Edge Intelligence
- IoT
- Kubernetes
- Device Management
- Orchestration
- AI at the Edge
---
