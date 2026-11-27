---
api_specs:
- filename: azure-health-collection-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Collection API
  slug: azure-health-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-collection-api-openapi.yml
- filename: azure-health-dicomservices-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services DicomServices API
  slug: azure-health-dicomservices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-dicomservices-api-openapi.yml
- filename: azure-health-fhirservices-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services FhirServices API
  slug: azure-health-fhirservices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-fhirservices-api-openapi.yml
- filename: azure-health-iotconnectors-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services IotConnectors API
  slug: azure-health-iotconnectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-iotconnectors-api-openapi.yml
- filename: azure-health-privatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services PrivateLinkResources API
  slug: azure-health-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-privatelinkresources-api-openapi.yml
- filename: azure-health-proxy-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Proxy API
  slug: azure-health-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-proxy-api-openapi.yml
- filename: azure-health-resource-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Resource API
  slug: azure-health-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-resource-api-openapi.yml
- filename: azure-health-workspaceprivateendpointconnections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services WorkspacePrivateEndpointConnections API
  slug: azure-health-workspaceprivateendpointconnections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-workspaceprivateendpointconnections-api-openapi.yml
- filename: azure-health-workspaceprivatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services WorkspacePrivateLinkResources API
  slug: azure-health-workspaceprivatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-workspaceprivatelinkresources-api-openapi.yml
- filename: azure-health-workspaces-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Workspaces API
  slug: azure-health-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-workspaces-api-openapi.yml
- filename: azure-health-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Private Endpoint Connections API
  slug: azure-health-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-health/openapi/azure-health-private-endpoint-connections-api-openapi.yml
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
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 09:41:22 2027 GMT
  host: management.azure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Health Data Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure Health Data Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Azure Health Data Services
provider_slug: azure-health
slug: azure-health-domain-security
source_filename: azure-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 09:41:22 2027 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azure-health/security/azure-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- FHIR
- DICOM
- IoMT
- Health Data
- HIPAA
- HITRUST
- Cloud
- Microsoft Azure
- Microsoft
---
