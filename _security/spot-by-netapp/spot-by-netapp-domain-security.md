---
api_specs:
- filename: spot-by-netapp-audit-service-api-openapi.yml
  format: yaml
  label: Spot by NetApp Audit Service API
  slug: spot-by-netapp-audit-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-audit-service-api-openapi.yml
- filename: spot-by-netapp-create-an-api-token-api-openapi.yml
  format: yaml
  label: Spot by NetApp Create an API Token API
  slug: spot-by-netapp-create-an-api-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-create-an-api-token-api-openapi.yml
- filename: spot-by-netapp-elastigroup-aws-api-openapi.yml
  format: yaml
  label: Spot by NetApp Elastigroup AWS API
  slug: spot-by-netapp-elastigroup-aws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-elastigroup-aws-api-openapi.yml
- filename: spot-by-netapp-elastigroup-azure-spot-vms-api-openapi.yml
  format: yaml
  label: Spot by NetApp Elastigroup Azure Spot VMs API
  slug: spot-by-netapp-elastigroup-azure-spot-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-elastigroup-azure-spot-vms-api-openapi.yml
- filename: spot-by-netapp-elastigroup-gcp-api-openapi.yml
  format: yaml
  label: Spot by NetApp Elastigroup GCP API
  slug: spot-by-netapp-elastigroup-gcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-elastigroup-gcp-api-openapi.yml
- filename: spot-by-netapp-health-check-service-api-openapi.yml
  format: yaml
  label: Spot by NetApp Health Check Service API
  slug: spot-by-netapp-health-check-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-health-check-service-api-openapi.yml
- filename: spot-by-netapp-insights-service-api-openapi.yml
  format: yaml
  label: Spot by NetApp Insights Service API
  slug: spot-by-netapp-insights-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-insights-service-api-openapi.yml
- filename: spot-by-netapp-notification-subscription-service-api-openapi.yml
  format: yaml
  label: Spot by NetApp Notification Subscription Service API
  slug: spot-by-netapp-notification-subscription-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-notification-subscription-service-api-openapi.yml
- filename: spot-by-netapp-ocean-automatic-rightsizing-api-openapi.yml
  format: yaml
  label: Spot by NetApp Ocean Automatic Rightsizing API
  slug: spot-by-netapp-ocean-automatic-rightsizing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-ocean-automatic-rightsizing-api-openapi.yml
- filename: spot-by-netapp-ocean-aws-api-openapi.yml
  format: yaml
  label: Spot by NetApp Ocean AWS API
  slug: spot-by-netapp-ocean-aws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-ocean-aws-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spot.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spotinst.io
  spf: false
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: spot.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: docs.spot.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: api.spotinst.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spot By Netapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spot by NetApp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spot by NetApp
provider_slug: spot-by-netapp
slug: spot-by-netapp-domain-security
source_filename: spot-by-netapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spot.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.spot.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spotinst.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spot.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spotinst.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/security/spot-by-netapp-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cloud Optimization
- FinOps
- Kubernetes
- Azure
- GCP
- Cost Optimization
- Auto Scaling
---
