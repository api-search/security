---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Azure DevOps Services REST API
  slug: azure-devops-services-rest-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/rest/api/azure/devops/
- filename: azure-devops-work-items-api-openapi.yml
  format: yaml
  label: Azure DevOps Boards API
  slug: azure-devops-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-work-items-api-openapi.yml
- filename: azure-devops-git-api-openapi.yml
  format: yaml
  label: Azure DevOps Repos API
  slug: azure-devops-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-git-api-openapi.yml
- filename: azure-devops-pipelines-api-openapi.yml
  format: yaml
  label: Azure DevOps Pipelines API
  slug: azure-devops-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-pipelines-api-openapi.yml
- filename: azure-devops-builds-api-openapi.yml
  format: yaml
  label: Azure DevOps Build API
  slug: azure-devops-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-builds-api-openapi.yml
- filename: azure-devops-releases-api-openapi.yml
  format: yaml
  label: Azure DevOps Release API
  slug: azure-devops-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-releases-api-openapi.yml
- filename: azure-devops-test-plans-api-openapi.yml
  format: yaml
  label: Azure DevOps Test Plans API
  slug: azure-devops-test-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-test-plans-api-openapi.yml
- filename: azure-devops-artifacts-api-openapi.yml
  format: yaml
  label: Azure DevOps Artifacts API
  slug: azure-devops-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-artifacts-api-openapi.yml
- filename: azure-devops-service-hooks-api-openapi.yml
  format: yaml
  label: Azure DevOps Service Hooks API
  slug: azure-devops-service-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-service-hooks-api-openapi.yml
- filename: azure-devops-wiki-api-openapi.yml
  format: yaml
  label: Azure DevOps Wiki API
  slug: azure-devops-wiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-wiki-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Sep 21 18:15:50 2026 GMT
  host: dev.azure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 18:32:22 2026 GMT
  host: app.vssps.visualstudio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Devops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure DevOps, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Azure DevOps
provider_slug: microsoft-azure-devops
slug: microsoft-azure-devops-domain-security
source_filename: microsoft-azure-devops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:15:50 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.vssps.visualstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:32:22 2026 GMT\n  hsts: null\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/security/microsoft-azure-devops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agile
- CI/CD
- DevOps
- Project Management
- Version Control
---
