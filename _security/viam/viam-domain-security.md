---
api_specs:
- filename: viam-fleet-management-api-openapi.yml
  format: yaml
  label: Viam Fleet Management API
  slug: viam-fleet-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-fleet-management-api-openapi.yml
- filename: viam-machine-management-api-openapi.yml
  format: yaml
  label: Viam Machine Management API
  slug: viam-machine-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-machine-management-api-openapi.yml
- filename: viam-data-client-api-openapi.yml
  format: yaml
  label: Viam Data Client API
  slug: viam-data-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-client-api-openapi.yml
- filename: viam-data-sync-api-openapi.yml
  format: yaml
  label: Viam Data Sync API
  slug: viam-data-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-sync-api-openapi.yml
- filename: viam-ml-training-api-openapi.yml
  format: yaml
  label: Viam ML Training API
  slug: viam-ml-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-training-api-openapi.yml
- filename: viam-ml-inference-api-openapi.yml
  format: yaml
  label: Viam ML Inference API
  slug: viam-ml-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-inference-api-openapi.yml
- filename: viam-billing-api-openapi.yml
  format: yaml
  label: Viam Billing API
  slug: viam-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-billing-api-openapi.yml
- filename: viam-motion-service-api-openapi.yml
  format: yaml
  label: Viam Motion Service API
  slug: viam-motion-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-motion-service-api-openapi.yml
- filename: viam-vision-service-api-openapi.yml
  format: yaml
  label: Viam Vision Service API
  slug: viam-vision-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-vision-service-api-openapi.yml
- filename: viam-slam-service-api-openapi.yml
  format: yaml
  label: Viam SLAM Service API
  slug: viam-slam-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-slam-service-api-openapi.yml
- filename: viam-ml-model-service-api-openapi.yml
  format: yaml
  label: Viam ML Model Service API
  slug: viam-ml-model-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-model-service-api-openapi.yml
- filename: viam-component-apis-openapi.yml
  format: yaml
  label: Viam Component APIs
  slug: viam-component-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-component-apis-openapi.yml
- filename: viam-data-pipelines-api-openapi.yml
  format: yaml
  label: Viam Data Pipelines API
  slug: viam-data-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-pipelines-api-openapi.yml
- filename: viam-provisioning-api-openapi.yml
  format: yaml
  label: Viam Provisioning API
  slug: viam-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-provisioning-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: viam.com
  spf: true
hosts:
- cert_expires: Sep 20 01:32:40 2026 GMT
  host: www.viam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 06:06:24 2026 GMT
  host: app.viam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 02:53:46 2026 GMT
  host: docs.viam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Viam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Viam
provider_slug: viam
slug: viam-domain-security
source_filename: viam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.viam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:32:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.viam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:06:24 2026 GMT\n  hsts: false\n- host: docs.viam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:53:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: viam.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/security/viam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Edge AI
- Fleet Management
- Computer Vision
- Machine Learning
- IoT
- Embedded
- gRPC
---
