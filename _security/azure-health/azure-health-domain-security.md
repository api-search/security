---
api_specs:
- filename: azure-health-collection-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Collection API
  slug: azure-health-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-collection-api-openapi.yml
- filename: azure-health-deid-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Deid API
  slug: azure-health-deid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-deid-api-openapi.yml
- filename: azure-health-dicomservices-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services DicomServices API
  slug: azure-health-dicomservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-dicomservices-api-openapi.yml
- filename: azure-health-fhirservices-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services FhirServices API
  slug: azure-health-fhirservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-fhirservices-api-openapi.yml
- filename: azure-health-iotconnectors-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services IotConnectors API
  slug: azure-health-iotconnectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-iotconnectors-api-openapi.yml
- filename: azure-health-jobs-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Jobs API
  slug: azure-health-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-jobs-api-openapi.yml
- filename: azure-health-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services PrivateEndpointConnections API
  slug: azure-health-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-privateendpointconnections-api-openapi.yml
- filename: azure-health-privatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services PrivateLinkResources API
  slug: azure-health-privatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-privatelinkresources-api-openapi.yml
- filename: azure-health-proxy-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Proxy API
  slug: azure-health-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-proxy-api-openapi.yml
- filename: azure-health-resource-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Resource API
  slug: azure-health-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-resource-api-openapi.yml
- filename: azure-health-workspaceprivateendpointconnections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services WorkspacePrivateEndpointConnections API
  slug: azure-health-workspaceprivateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaceprivateendpointconnections-api-openapi.yml
- filename: azure-health-workspaceprivatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services WorkspacePrivateLinkResources API
  slug: azure-health-workspaceprivatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaceprivatelinkresources-api-openapi.yml
- filename: azure-health-workspaces-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Workspaces API
  slug: azure-health-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaces-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Sep 24 22:04:48 2026 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:36:21 2026 GMT
  host: management.azure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Azure Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure Health Data Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Azure Health Data Services
provider_slug: azure-health
slug: azure-health-domain-security
source_filename: azure-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:36:21 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/security/azure-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- FHIR
- DICOM
- MedTech
- IoMT
- Health Data
- HIPAA
- HITRUST
- Cloud
- Azure
- Microsoft
---
