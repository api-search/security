---
api_specs:
- filename: azure-devops-health-availabilitystatuses-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Availability Statuses API
  slug: azure-devops-health-availabilitystatuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-availabilitystatuses-api-openapi.yml
- filename: azure-devops-health-childavailabilitystatuses-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Child Availability Statuses API
  slug: azure-devops-health-childavailabilitystatuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml
- filename: azure-devops-health-childresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Child Resources API
  slug: azure-devops-health-childresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-childresources-api-openapi.yml
- filename: azure-devops-health-emergingissues-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Emerging Issues API
  slug: azure-devops-health-emergingissues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-emergingissues-api-openapi.yml
- filename: azure-devops-health-event-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Event API
  slug: azure-devops-health-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-event-api-openapi.yml
- filename: azure-devops-health-eventimpactedresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Event Impacted Resources API
  slug: azure-devops-health-eventimpactedresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-eventimpactedresources-api-openapi.yml
- filename: azure-devops-health-events-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Events API
  slug: azure-devops-health-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-events-api-openapi.yml
- filename: azure-devops-health-metadata-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Metadata API
  slug: azure-devops-health-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-metadata-api-openapi.yml
- filename: azure-devops-health-operations-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Operations API
  slug: azure-devops-health-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-operations-api-openapi.yml
- filename: azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Security Advisory Impacted Resources API
  slug: azure-devops-health-securityadvisoryimpactedresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml
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
- cert_expires: Apr  7 23:37:09 2027 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 09:41:22 2027 GMT
  host: management.azure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Azure Resource Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Resource Health, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Resource Health
provider_slug: azure-devops-health
slug: azure-devops-health-domain-security
source_filename: azure-devops-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  7 23:37:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 09:41:22 2027 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azure-devops-health/security/azure-devops-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Continuous Integration
- Developer Tools
- Public APIs
- Microsoft Azure
- Microsoft
- Monitoring
- Service Health
---
